# Data efficient machine learning potentials for modeling catalytic reactivity via active learning and enhanced sampling

This repository contains the code needed to reproduce the workflow presented in:

Perego S. and Bonati L., "Data efficient machine learning potentials for modeling catalytic reactivity via active learning and enhanced sampling", _npj Computational Materials_ 10, 291 (2024), doi:[10.26434/chemrxiv-2024-nsp7n](https://doi.org/10.1038/s41524-024-01481-6)

> [!NOTE]  
> We are preparing tutorials to illustrate more generally the different steps of our protocol (including DEAL) beyond the specific examples addressed in the manuscript (which require, e.g., running Quantum Espresso). If you are interested, turn on notifications! 

## Contents:
```
├── notebooks           # notebooks describing the different stages of the MLP construction 
│   ├── 0_preliminary
│   ├── 1_exploration
│   └── 2_convergence
├── configs             # configuration files for the different tasks
│   ├── deal
│   ├── flare
│   ├── lammps
│   ├── mace
│   ├── plumed
│   └── qe
└── mlputils            # python module containing the necessary functions
```

## Requirements

The following software and versions have been used:

* ASE (v3.22.1-fix from [luigibonati/ase](https://github.com/luigibonati/flare/tree/3.2.1-fix)) $\rightarrow$ modified ASE version with small fixes to espresso input/outputs. Note that version 3.23 is not compatible.
* FLARE (v1.3.3-fix from [luigibonati/flare](https://github.com/luigibonati/flare/tree/1.3.3-fix)) $\rightarrow$ modified FLARE version with small fixes to ensure it work correctly with LAMMPS & PLUMED simulations as well as for the DEAL active learning selection scheme
* MACE (v0.35 from [ACEsuit/mace](https://github.com/ACEsuit/mace))
* LAMMPS with support of:
    * MACE (patched version from [ACEsuit/lammps](https://github.com/ACEsuit/lammps))
    * FLARE (pair style from [mir-group](https://github.com/mir-group/flare))
    * PLUMED (v2.9 from [plumed/plumed2](https://github.com/plumed/plumed2))
