# ROY-ForceField-PLUMED-NEST

Supporting Information for:
- P. Si and O. Valsson    
*Assessment of Force Fields for Describing Conformational Polymorphic Crystals of ROY* 

This archive contains input files used to generate the data.

## Authors
Pradip Si - pradipsi@my.unt.edu   
*Department of Chemistry*    
*University of North Texas*    
*Denton, Texas, USA*     
ORCID: [0000-0001-5337-4354](https://orcid.org/0000-0001-5337-4354)

Omar Valsson - omar.valsson@unt.edu    
*Department of Chemistry*     
*University of North Texas*    
*Denton, Texas, USA*    
ORCID: [0000-0001-7971-4767](https://orcid.org/0000-0001-7971-4767)     
Website: www.valsson.info

## Software
Files were run with the following codes:
- GROMACS 2022.5 MD code
- PLUMED 2.8.2 enhanced sampling plug-in code 
- VMD 1.9.3 for trajectory analysis

## File Overview:

- All the .gro files of ROY polymorphs are located in the `Supercells` folder.
- All GAFF and OpenFF force field topologies for different charge models are in the `Topology` folder.
- The GROMACS molecular dynamics parameters can be found in the `MD_Parameters` folder.
- The Plumed input files for SMAC, torsion angle, and distance are in the `PLUMED_Inputs` folder.
  - `create_plumed.py` script for generating specific plumed input.
- Codes for generating the KDE for different CVs are in the `Analysis-script` folder.
  - `generate_kde_numpytxt_SMAC.py`: to calculate the Gaussian kernel density approximation (KDE) of the SMAC parameters from PLUMED.
  - `generate_kde_numpytxt_torsion.py`: to calculate the periodic kernel density approximation (KDE) of the torsional angle from PLUMED using Haversine distance.
  - `generate_kde_numpytxt_distance.py`: to calculate the Gaussian kernel density approximation (KDE) of the H-bonding distance from PLUMED.

## License
Copyright (c) 2025 Pradip Si and Omar Valsson

Creative Commons Attribution 4.0 International Public License (CC BY 4.0). See `LICENSE` for more details.
