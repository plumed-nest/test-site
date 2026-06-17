# EMMI-ASCT2
Repository of the data needed to reproduce the Metainference simulations of ASCT2 described in:
Rachel-Ann A. Garibsingh et al, Structural basis for stereospecific inhibition of ASCT2 from rational design, doi: [10.1101/2020.05.29.124305](https://doi.org/10.1101/2020.05.29.124305).
Simulations have been performed using GROMACS 2019.6 and PLUMED [GitHub ISDB branch](https://github.com/plumed/plumed2/tree/isdb).

The repository is organized in the following directories:
- **0-TOPO**: topology files in GROMACS format
- **1-EQUIL**: protocol to perform equilibration of the system. Detailed instructions are contained in *do_equilibration.sh*.
- **2-EMMI**:  Metainference production simulation. Detailed instructions are contained in *do_production.sh*.
- **3-ANALYSIS**: Scripts and codes to perform analysis of the Metainference simulation.    
- **4-PDBs**: Final models reported in the paper.
