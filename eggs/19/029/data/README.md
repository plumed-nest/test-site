Computational Biology Laboratory, Danish Cancer Society Research Center, Strandboulevarden 49, 2100, Copenhagen, Denmark

Repository associated to the publication:

Marinelli P, Navarro S, Graña-Montes R, Bañó-Polo M, Fernández MR, Papaleo E,  Ventura S. A single cysteine post-translational oxidation suffices to compromise  globular proteins kinetic stability and promote amyloid formation. Redox Biol.
2018;14:566-575. doi: 10.1016/j.redox.2017.10.022. 

reference person for the repository: Elena Papaleo, elenap@cancer.dk

This repository contains the input data for the metadynamics simulations 

The calculations were done with the PLUMED 1.3 plugin and Gromacs 4.6.5 but we also provide the 
input file in the version for PLUMED 2 for one of the variants as an example

We used the PDB file 2JUC for the wild-type variant - The CtoD mutation was modelled with pymol


The three main folders in the repository contain:

-WT: input files for metaD of the wild-type variant

-C57D: input files for metaD of the mutant variant 

-C57D.plumed2: corresponding input files for plumed2


NB1. the original mdp files were set for 1000 ns but we collected 550 ns per analysis, as explained in the article.
NB2. .xtc trajectories file are too big to be shared in this repository but they are available upon request.
