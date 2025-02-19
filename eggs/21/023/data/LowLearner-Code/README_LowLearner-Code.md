## LowLearner Code
J. Rydzewski, O. Valsson, *Multiscale Reweighted Stochastic Embedding (MRSE): Deep Learning of Collective Variables for Enhanced Sampling*, [arXiv:2007.06377]((https://arxiv.org/abs/2007.06377)) (2021).

The LowLearner Code in the form of a PLUMED 2 module that can be used to generate the MRSE embeddings for the files here.
* This a work-in-progress version of the code. An updated version will be added to the official PLUMED code in the future.
* No manual is included. Keywords and syntax will likely change.
* The code should work with PLUMED v2.7 or master branch but will not likely work with older versions of PLUMED.
* The code is distributed under GNU LESSER GENERAL PUBLIC LICENSE   
* The code requires PLUMED to be linked with LibTorch.
* This version of the code been tested to work with LibTorch v1.8, previous or newer versions of LibTorch might not work.
* Note: This code is not exactly the same as used to generate the MRSE embeddings in the paper as it has been slightly modified to work with LibTorch v1.8. However, it should give similar results though they will not be exactly the same due to randomness in LibTorch, even when using the same random seed.
* This version of the code corresponds to git commit 8c52f93340855ae872f557db25b595c0474157c5 in our private git development repository.

## Installation Instructions
* Download LibTorch (v1.8 tested and recommended) binaries from https://pytorch.org/ and install them.
* Copy the `lowlearner` folder to the `src` folder of the main PLUMED directory.
* The `config-plumed.sh` script can used to configure PLUMED compilation to include linking with LibTorch.
  * Update the `LIBTORCH_DIR` to point to the folder where LibTorch is installed
  * See further information within the `config-plumed.sh` script.
* The `config-plumed.sh` script should be run with PLUMED folder.
* Then run `make` or `make -j N` to compile PLUMED.
* Afterwards, you can then use `source sourceme.sh` to set the paths for the compiled PLUMED binaries.
* If you want, you can install PLUMED using `make install`.
  * The binaries will be installed into the folder given by `PLUMED_INSTALL_DIR` or the folder `install` within the PLUMED folder.
  * You can use the generated `source-install.sh` script to set the paths for the installed version using `source source-install.sh`.
