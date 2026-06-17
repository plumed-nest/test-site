This repository contains additional supporting files for the paper "Molecular Simulations Reveal an Interplay Between SHAPE Reagent Binding and RNA Flexibilty, J. Phys. Chem. Lett., 2018, 9 (2), pp 313–318" by Vojtech Mlynsky and Giovanni Bussi.
In case you find it useful, please cite that paper.

- folder `pdb-s_all-clusters` contains coordinates (pdb format) of SRP-RNA with BzCN reagent for all clusters
- files `SRP-RNA_BzCN` are GROMACS input files for enhanced sampling simulations of SRP-RNA with BzCN reagent
- files `GNRA_BzCN` are GROMACS input files (converted from AMBER using acpype) of gccGUAAggc GNRA simulation with BzCN reagent
- other GROMACS input files (converted from AMBER using acpype) of simulations with nucleotide analogs (cAMP, cCMP) with NMIA
- `plumed_g3.dat` is the example of input file for one particular nucleotide from SRP-RNA used in enhanced sampling simulation with BzCN reagent
