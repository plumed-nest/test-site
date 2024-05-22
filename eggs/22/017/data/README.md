# LigandBinding_Trypsin_FES_RATE

The role of water in host-guest interaction 

This archive contains all the input files needed to reproduce the results of the paper.
In the FES folder the following files are available:
- production.mdp, nosolv_GMX.top and prd.tpr are the GROMACS input.
- B.pdb and B1.pdb contain two binding pose configurations.
- plumed.dat is the PLUMED input, fit_tem.pdb is a coordinate alignment file and the *.pt files contain the Deep-LDA and Deep-TICA neural network model CVs.

The RATE folder contains the files for rate simulations.

More information about using PLUMED with Pytorch can be found at https://github.com/luigibonati/data-driven-CVs.
More information about OPES can be found at https://github.com/invemichele/opes.

The simulations were performed with PLUMED 2.8, Pytorch 1.4, and GROMACS 2020.4. 
