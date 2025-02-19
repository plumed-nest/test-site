# BANAL-236
Data needed to reproduce the Molecular Dynamics simulations of WT and mutant BANAL-236 RBD/hACE2 complexes reported in:

Temmam et al. SARS-CoV-2-related bat virus behavior in human-relevant models sheds light on the origin of COVID-19.
EMBO Rep. 2023 Apr 5;24(4):e56055. doi: 10.15252/embr.202256055.

This repository is organized in the following directories:
* `WT`: data related to the simulations of the wild type BANAL-236 RBD/hACE2 complex;
* `V391I`: data related to the simulations of the V391I mutant;
* `DATA`: various protocols, python/bash scripts and GROMACS mdp files.

Inside the first 2 directories, you will find subdirectories for system setup and equilibration, plus one subdirectory for each independent 
production simulation (replicate) of the RBD/hACE2 complex under study. 
The naming scheme along with some basic information about the simulations is reported in the table at the bottom of this page.
Each of the directories in the table is organized as follows:
* `0-TOPO`: initial conformation and topology files in GROMACS format;
* `1-EQUIL`: run energy minimization and equilibration here. Please refer to `README.md` for instructions;
* `2-PRODUCTION`: run production simulations here. Please refer to `README.md` for instructions; 
* `3-ANALYSIS`: analyze production simulations here. Please refer to `README.md` for instructions.

**Software requirements**

Make sure you install the following software before performing and analyzing the simulations. Information about
how to install the software can be found by following the corresponding link.  

* [GROMACS 2021.4](https://www.gromacs.org)
* [PLUMED 2.7](https://www.plumed.org)
* [MDAnalysis 2.1.0](https://www.mdanalysis.org)
* [MDTraj 1.9.5](https://www.mdtraj.org/1.9.5/index.html)
* [FoldX 4](http://foldxsuite.crg.eu)

**Summary of all the simulations performed**

|   RUN ID	   |  Construct	| Initial model	| # K/Cl ions |	 # waters | Total # atoms | Production time [ns] |
| :------: |  :------:  |     :------:  | :------:    | :------:  | :------:      | :------:             |
| WT.1 | WT BANAL-236 RBD/hACE2 | X-ray (PDB code [7PKI](https://www.rcsb.org/structure/7PKI)) | 113/91 | 27990 | 96937 | 1000 |
| WT.2 | WT BANAL-236 RBD/hACE2 | X-ray (PDB code [7PKI](https://www.rcsb.org/structure/7PKI)) | 113/91 | 27990 | 96937 | 1000 |
| WT.3 | WT BANAL-236 RBD/hACE2 | X-ray (PDB code [7PKI](https://www.rcsb.org/structure/7PKI)) | 113/91 | 27990 | 96937 | 1000 |
| V391I.1 | V391I BANAL-236 RBD/hACE2 |	Homology model  | 113/91 | 27955 | 96835 | 1000 |
| V391I.2 | V391I BANAL-236 RBD/hACE2 |	Homology model  | 113/91 | 27955 | 96835 | 1000 |
| V391I.3 | V391I BANAL-236 RBD/hACE2 |	Homology model  | 113/91 | 27955 | 96835 | 1000 |

**Contact**

For any technical questions, please write to mbonomi_at_pasteur.fr.
