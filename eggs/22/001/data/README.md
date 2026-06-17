# Input files for paper "Enhanced Sampling with Wavelet-Based Bias Potentials"
This archive contains input files used to generate the data


## Authors
Omar Valsson <<valsson@mpip-mainz.mpg.de>>
*Max Planck Institute for Polymer Research,*
*Ackermannweg 10, D-55128 Mainz, Germany*
ORCID: [0000-0001-7971-4767](https://orcid.org/0000-0001-7971-4767)

Benjamin Pampel <<pampel@mpip-mainz.mpg.de>>
*Max Planck Institute for Polymer Research,*
*Ackermannweg 10, D-55128 Mainz, Germany*
ORCID: [0000-0002-1652-6918](https://orcid.org/0000-0002-1652-6918)


## Software
The files were run with the following codes:
- PLUMED version 2.7.0-dev. Private development version with the localized basis functions and the adam optimizer. Needs to be compiled with the VES module. The custom parts required for the simulations are contained in PLUMED from version 2.8.0 and greater.
- Lammps (5 Jun 2019 version)
- packmol and VMD (for the creation of the initial geometry of the CaCO3 system)


## Folders

### Simulations of artificial potentials with the `ves_md_linearexpansion` tool of `plumed`
Each subdirectory contains a different potential that was simulated with 4 different VES basis sets.
These contain a `shared_input` folder with the potential and simulation parameters, as well as custom `plumed.dat` files for each basis set.

The potentials are
- `1d_double_well`: a simple 1D double well potential
- `2d_wolfe_quapp`: the 2D Wolfe-Quapp potential
- `2d_wolfe_quapp_rotated`: a rotated and scaled version of the Wolfe-Quapp potential, where only one CV is biased

#### Simulation of calcium carbonate association with `lammps` and `plumed`
The CaCO3 system was simulated with 3 different biasing methods: two different VES basis sets (`chebyshev`, `sym10`) and metadynamics (`metad`).
The folder also contains the scripts to generate the initial configurations of this simulations (`setup`) which can be found in the `initial_configuration` folder.

The simulation folders contain the plumed file(s) as well as the lammps input file for each type of biased simulation.


## Workflow

### `ves_md_linearexpansion` simulations
Modify the variables in the `start_simulations.sh` script and run it.
This then copies the required input files into subfolders and runs the requested number of analog simulations via the `run_multisim.sh` script.

### `lammps` simulations
Run the `create_input.sh` script to create directories with the input files for all simulations.
These were submitted to the SLURM queue of the cluster with the `run_simulation.sh` script, which likely needs to be adjusted on a different system.


## License
Copyright (c) 2022 Omar Valsson and Benjamin Pampel

Omar Valsson <<valsson@mpip-mainz.mpg.de>>
*Max Planck Institute for Polymer Research,*
*Ackermannweg 10, D-55128 Mainz, Germany*
ORCID: [0000-0001-7971-4767](https://orcid.org/0000-0001-7971-4767)

Benjamin Pampel <<pampel@mpip-mainz.mpg.de>>
*Max Planck Institute for Polymer Research,*
*Ackermannweg 10, D-55128 Mainz, Germany*
ORCID: [0000-0002-1652-6918](https://orcid.org/0000-0002-1652-6918)


Creative Commons Attribution 4.0 International Public License. See `LICENSE` for more details.
