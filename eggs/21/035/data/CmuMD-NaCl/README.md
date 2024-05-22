# CμMD Simulations of NaCl(aq) at Graphite Using GROMACS and PLUMED (v2)

__Please consider citing Perego et al. J Chem Phys 142, 144113 (2015)__
__Please consider citing Finney et al. Chemical Science, 12, 11166-11180 (2021)__

The repository hosts the input and output files to run simulations of the kind described by Finney and Salvalaglio using [GROMACS](https://www.gromacs.org) and [PLUMED 2](https://www.plumed.org).

All input files to perform CmuMD of NaCl(aq) in contact with perfectly planar and rough NaCl crystal surfaces are provided. The target concentration of ions in the bulk is 3M. The force field parameter files are contained in `./graph-NaCl-pol.ff`.

To run the simulation with Gromacs and Plumed use e.g.,
`gmx grompp -f job.mdp -c flat.gro -p flat.top -o flat`
`gmx mdrun -deffnm flat -plumed flat-plumed.dat`
