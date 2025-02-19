# Molecular Dynamics simulations of RBD/hACE2 complexes 
Repository of the data needed to reproduce the Molecular Dynamics simulations of 3 different RBD/hACE2 complexes reported in:

[S. Temmam *et al.*, Discovery of bat coronaviruses close to SARS-CoV-2 and infectious for human cells. Nature 604 (2022) 330](https://www.nature.com/articles/s41586-022-04532-4).


This repository is organized in the following directories:
* `SARS-CoV-2`: data related to the simulations of the SARS-CoV-2 RBD/hACE2 complex;
* `BANAL-236-CoV`: data related to the simulations of the BANAL-236 RBD/hACE2 complex;
* `BANAL-52-103-CoV`: data related to the simulations of the BANAL-52-103 RBD/hACE2 complex;
* `DATA`: various protocols, python/bash scripts and GROMACS mdp files.

Inside the first 3 directories, you will find 3 subdirectories, one for each independent run (replicate) of the RBD/hACE2 complex
under study. The naming scheme along with some basic information about the simulations is reported in the table at the bottom of this page.
Each of the directories in the table is organized as follows:
* `0-TOPO`: initial conformation and topology files in GROMACS format;
* `1-EQUIL`: run energy minimization and equilibration here. Please refer to `README.md` for instructions;
* `2-PRODUCTION`: run production simulations here. Please refer to `README.md` for instructions; 
* `3-ANALYSIS`: analyze production simulations here. Please refer to `README.md` for instructions.

**Software requirements**

Make sure you install the following software before performing and analyzing the simulations. Information about
how to install the software can be found by following the corresponding link.  

* [GROMACS 2020.4](https://www.gromacs.org)
* [PLUMED 2.7](https://www.plumed.org)
* [MDAnalysis 1.0.0](https://www.mdanalysis.org)
* [MDTraj 1.9.5](https://www.mdtraj.org/1.9.5/index.html)
* [ROSETTA 3.11](https://www.rosettacommons.org)
* [FoldX 4](http://foldxsuite.crg.eu)

**Summary of all the simulations performed**

|   RUN ID	   |  Construct	| Initial model	| # K/Cl ions |	 # waters | Total # atoms | Production time [ns] |
| :------: |  :------:  |     :------:  | :------:    | :------:  | :------:      | :------:             |
| SARS-CoV-2.1 | SARS-CoV-2 RBD/hACE2 | X-ray (PDB code [6M0J](https://www.rcsb.org/structure/6M0J)) | 121/97 | 30621 | 104592 | 1000 |
| SARS-CoV-2.2 | SARS-CoV-2 RBD/hACE2 | X-ray (PDB code [6M0J](https://www.rcsb.org/structure/6M0J)) | 121/97 | 30621 | 104592 | 1000 |
| SARS-CoV-2.3 | SARS-CoV-2 RBD/hACE2 | X-ray (PDB code [6M0J](https://www.rcsb.org/structure/6M0J)) | 121/97 | 30621 | 104592 | 1000 |
| BANAL-236-CoV.1 | BANAL-236 RBD/hACE2 | Homology model (top1) | 121/97 | 30502 | 104228 | 1000 |
| BANAL-236-CoV.2 | BANAL-236 RBD/hACE2 | Homology model (top2) | 120/96 | 30140 | 103140 | 1000 |
| BANAL-236-CoV.3 | BANAL-236 RBD/hACE2 | Homology model (top3) | 120/96 | 30090 | 102990 | 1000 |
| BANAL-52-103-CoV.1 | BANAL-52-103 RBD/hACE2 |	Homology model (top1) |	123/98	| 30808	| 105144 | 1000 |
| BANAL-52-103-CoV.2 | BANAL-52-103 RBD/hACE2 |	Homology model (top2) |	121/96	| 30135	| 103121 | 1000 |
| BANAL-52-103-CoV.3 | BANAL-52-103 RBD/hACE2 |	Homology model (top3) |	124/99	| 31307	| 106643 | 1000 |

**Contact**

For any technical questions, please write to mbonomi_at_pasteur.fr.
