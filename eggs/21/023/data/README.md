# MRSE PLUMED Egg (version 1.0.0)
Archive with PLUMED input files supporting the results of *Multiscale Reweighted Stochastic Embedding (MRSE): Deep Learning of Collective Variables for Enhanced Sampling*.

arXiv: [2007.06377](https://arxiv.org/abs/2007.06377)  
Full Dataset -- Zenodo: [4756093](https://zenodo.org/record/4756093)

## Authors
Jakub Rydzewski  <<jr@fizyka.umk.pl>>  
*Institute of Physics, Nicolaus Copernicus University,*    
*Grudziadzka 5, 87-100 Torun, Poland*  
ORCID: [0000-0003-4325-4177](https://orcid.org/0000-0003-4325-4177)  

Omar Valsson <<valsson@mpip-mainz.mpg.de>>  
*Max Planck Institute for Polymer Research,*  
*Ackermannweg 10, D-55128 Mainz, Germany*  
ORCID: [0000-0001-7971-4767](https://orcid.org/0000-0001-7971-4767)  

## Software
The data was originally obtained using the following codes:
* PLUMED version 2.7.0-dev (git: a09d8e6). Private development version with the additional lowlearner module (compiled with: `--enable-module=lowlearner` or `--enable-module=all`).
* LibTorch (git commit 89d6e88) library linked to PLUMED.
* GROMACS 2019.0 patched with PLUMED.
* Note: See below for information about the LowLearner code and how to compile it.

## Full Dataset with Output Files
This dataset only includes GROMACS and PLUMED input fill needed to reproduce the results.
The full dataset, including all output files, can be downloaded from Zenodo under [4756093](https://zenodo.org/record/4756093).

## Simulations to Generated Datasets
`Data-*/` -- input files for simulations to generate datasets. Includes parallel tempering (PT) and well-tempered metadynamics (WT-MetaD) simulations for the investigated systems: the Mueller-Brown potential (`mb`), alanine dipeptide (`ala1`), and alanine tetrapeptide (`ala3`). See below.

### `./Data-mb/` path (simulations for the Mueller-Brown potential):
* Directories `mb-wtm-bf__BIAS_FACTOR__` -- WT-MetaD simulations with a Gaussian width of 0.1 and a bias factor as given by `__BIAS_FACTOR__`.

### `./Data-ala1/` path (simulations for alanine dipeptide):
* Directories `ala1-vacuum-wtm-rct-ustride-1-bf__BIAS_FACTOR__` -- WT-MetaD simulations with c(t) calculated every 1 step and a bias factor as given by `__BIAS_FACTOR__`.
* Directory `ala1-vacuum-pt` -- a PT simulation with four replicas. We used only `repl-0/colvar.data` (300 K) to train or evaluate MRSE.

### `./Data-ala3/` path (simulations for alanine tetrapeptide):
* Directory `ala3-vacuum-wtm-rct-ustride-50-bf5` -- WT-MetaD simulation with c(t) calculated every 50 steps and a bias factor of 5. The features used to train embeddings are stored in `colvar.data`.
* Directory `ala3-vacuum-pt` -- a PT simulation with eight replicas. We used only `repl-0/colvar.data` (300 K) to train MRSE.

## MRSE Embeddings
`MRSE-*/` -- input files for MRSE embeddings trained and evaluated on the datasets.

### `./MRSE-mb/` path (embeddings for the Mueller-Brown potential):
* Directories `MRSE-wtm-bf__BIAS_FACTOR__` -- WT-MetaD embeddings trained and evaluated on the WT-MetaD datasets in `mb-wtm-bf__BIAS_FACTOR__`, each indicated by the value of bias factor as `__BIAS_FACTOR__`.

### `./MRSE-ala1/` path (embeddings for alanine dipeptide):
* Directories `MRSE-ala1-vacuum-wtm-bf__BIAS_FACTOR__` -- WT-MetaD embeddings trained on the WT-MetaD datasets in `Data-ala1/ala1-vacuum-wtm-rct-ustride-1-bf__BIAS_FACTOR__` and evaluated on the PT dataset (`MRSE-ala1-vacuum-wtm-bf__BIAS_FACTOR__/colvar-pt.data`), each indicated by the value of bias factor `__BIAS_FACTOR__`.
* Directory `MRSE-ala1-vacuum-pt` -- PT embedding trained and evaluated on the PT dataset from `Data-ala1/ala1-vacuum-pt`.

### `./MRSE-ala3/` path (embeddings for alanine tetrapeptide):
* Directory `MRSE-ala3-vacuum-wtm-bf5` -- WT-MetaD embeddings trained and evaluated on the WT-MetaD dataset in `Data-ala3/ala3-vacuum-wtm-rct-ustride-50-bf5`.
* Directory `MRSE-ala3-vacuum-pt` -- PT embedding trained and evaluated on the PT dataset in `Data-ala3/ala3-vacuum-pt`.

## Workflow
To generate the embeddings in `MRSE-*/__NAME__`, we use the following workflow:
* Copy a dataset `colvar.data` from the corresponding simulation directory.
* For the WT-MetaD simulations, we remove the initial 20% of the simulation. We run `fix-time.sh` to generate another file `colvar-tf.data`, where the time starts at 0 ps.
* Prepare a PLUMED input file `plumed.gen-nn.dat` to train a low-dimensional embedding.
* Prepare a PLUMED input file `plumed.calc-nn.dat` to evaluate the embedding. Depending on what dataset you want to evaluate the obtained neural network, provide the corresponding file. For instance, the WT-MetaD embeddings for alanine dipeptide are evaluated on the PT dataset, so in every directory, a file `colvar-pt.data` is provided.
* Note: for alanine dipeptide, we use standardized features. The transformation are obtained by using the `check-features.sh` script that you can run using `run-check-features.sh`. This script gives PLUMED commands (`CUSTOM` actions) for the standardized feature transformations that you can include in `plumed.gen-nn.dat` and `plumed.calc-nn.dat`. (Warning: the transformations currently included in the PLUMED inputs are only valid for the datasets used for that embeddings. Thus, one needs to re-generate the transformations for each given dataset.)
* Run the script `nohup ./detach-job.sh &> plumed.out &`.
* The script will result in the following files:
  * `colvar.out.calc-nn.dat` -- the evaluated embedding with collective variables generated by our neural network (`nn.cv1` and `nn.cv2`).
  * `log.pt` -- a log file with output from estimating a low-dimensional embedding;
  * `network-1.pt` -- a trained neural network saved in the LibTorch format;
  * `optimizer-1.pt` -- an optimizer saved in the LibTorch format;
  * `plumed.out` -- output of the PLUMED software;
  * `training.pt` -- a log file storing the training information;
  * `weights.pt` -- a log file with the statistical weights of selected conformations using landmark selection;
* Calculate free energy surface on the evaluated embedding by running `./calculate-fes.sh` in `fes`.

## LowLearner Code
The LowLearner Code in the form of a PLUMED 2 module to generate the MRSE embeddings for the files provided here can be found in the directory `LowLearner-Code`.
* This a work-in-progress version of the code. An updated version will be added to the official PLUMED code in the future.
* No manual is included. Keywords and syntax will likely change.
* The code should work with PLUMED v2.7 or master branch but will not likely work with older versions of PLUMED.
* The code is distributed under GNU LESSER GENERAL PUBLIC LICENSE.
* The code requires PLUMED to be linked with LibTorch.
* This version of the code has been tested to work with LibTorch v1.8; previous or newer versions of LibTorch might not work.
* Instructions for linking PLUMED with LibTorch v1.8 can be found in the `LowLearner-Code` directory.
* Note: This code is not the same as used to generate the MRSE embeddings in the paper, as it has been slightly modified to work with LibTorch v1.8. However, it should give similar results though they will not be exactly the same due to randomness in LibTorch, even when using the same random seed.
* This version of the code corresponds to git commit 8c52f93340855ae872f557db25b595c0474157c5 in our private git development repository.

## Acknowledgments
J. Rydzewski gratefully acknowledges financial support from the Foundation for Polish Science (FNP).

## License
Copyright (c) 2021 Jakub Rydzewski and Omar Valsson

Jakub Rydzewski  <<jr@fizyka.umk.pl>>  
*Institute of Physics, Nicolaus Copernicus University,*  
*Grudziadzka 5, 87-100 Torun, Poland*  
ORCID: [0000-0003-4325-4177](https://orcid.org/0000-0003-4325-4177)  

Omar Valsson <<valsson@mpip-mainz.mpg.de>>  
*Max Planck Institute for Polymer Research,*  
*Ackermannweg 10, D-55128 Mainz, Germany*  
ORCID: [0000-0001-7971-4767](https://orcid.org/0000-0001-7971-4767)  

Creative Commons Attribution 4.0 International Public License. See `LICENSE` for more details.
