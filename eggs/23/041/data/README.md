# EMMIVox-BENCHMARK
Data to reproduce the EMMIVox model refinement benchmark described in:

S. E. Hoff, F. E. Thomasen, K. Lindorff-Larsen, M. Bonomi. Accurate model and ensemble refinement using cryo-electron microscopy maps and Bayesian inference.
bioRxiv 2023 [doi: 10.1101/2023.10.18.562710](https://www.biorxiv.org/content/10.1101/2023.10.18.562710v1).

Details about the systems used in our benchmark are
reported in the table below. Instructions to install [GROMACS](https://www.gromacs.org) and [PLUMED](https://www.plumed.org) as well as analysis scripts and complete tutorials can be found [here](https://github.com/maxbonomi/EMMIVox).

**Details of the benchmark systems**

| ID | PDB ID | EMDB ID | resolution [Å] | # protein residues | # protein chains | # waters | # lipids | # ligands | # waters | # lipids | # buffer ions | # atoms |
| :------: |  :------:  |  :------:  | :------: | :------:  | :------:  | :------: | :------: |  :------:  |  :------:  | :------: | :------:  | :------:  |
 | 01  | 7p6a  | 13223  | 1.90  | 540  | 5  | 76  | 0  | 0  | 10,782  | 0  | 124  | 40,805 |
 | 02  | 7w9w  | 32377  | 2.02  | 810  | 3  | 144  | 24  | 0  | 17,548  | 169  | 113  | 86,452 |
 | 03  | 7n00  | 24095  | 2.27  | 806  | 2  | 0  | 0  | 0  | 43,754  | 0  | 260  | 143,124 |
 | 04  | 7t4n  | 25681  | 2.35  | 914  | 2  | 0  | 0  | 0  | 100,987  | 0  | 574  | 318,262 |
 | 05  | 7b5o  | 12042  | 2.50  | 651  | 3  | 73  | 0  | 1  | 50,944  | 0  | 289  | 163,693 |
 | 06  | 7mjs  | 23883  | 3.03  | 715  | 3  | 0  | 1  | 2  | 29,943  | 190  | 168  | 126,588 |
 | 07  | 7lq6  | 23482  | 3.28  | 717  | 1  | 0  | 0  | 0  | 80,921  | 0  | 465  | 254,485 |
 | 08  | 7nqk  | 12528  | 3.50  | 781  | 2  | 0  | 0  | 0  | 39,764  | 328  | 222  | 175,791 |
 | 09  | 6yeg  | 10792  | 4.00  | 2064  | 12  | 0  | 0  | 0  | 60,592  | 0  | 496  | 212,980 |

**Model validation**

To validate the deposited PDBs and the EMMIVox single-structure model using the metrics described in the manuscript, please:

- download the analysis scripts [here](https://github.com/maxbonomi/EMMIVox);
- download the PDB structures and cryo-EM maps using the script `get_PDB_MAP.sh`;
- run the validation of the deposited PDBs with `validate_PDB.sh`;
- run the validation of the EMMIVox models with `validate_EMMIVox.sh`. 

**Contact**

For any technical questions, please write to mbonomi_at_pasteur.fr.
