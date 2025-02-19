**Project ID:** [plumID:24.025]({{ '/' | absolute_url }}eggs/24/025/)  
**Name:**  Correlating Enzymatic Reactivity for Different Substrates using Transferable Data-Driven Collective Variables  
**Archive:** [ https://github.com/sudipdas789/Transferable_DeepCVs/archive/refs/heads/main.zip](https://github.com/sudipdas789/Transferable_DeepCVs/archive/refs/heads/main.zip)  
**Category:**  bio  
**Keywords:**  enzymatic reactivity, k_cat, transfer learning, data-driven CVs, catalysis, ligand-binding modes, water, alpha-amylase, sugar, classical MD, OPES, machine learning, Deep TDA CV, path CV  
**PLUMED version:**  2.9  
**Contributor:**  Sudip Das  
**Submitted on:** 26 Oct 2024  
**Publication:** [S. Das, U. Raucci, R. P. P. Neves, M. J. Ramos, M. Parrinello, Correlating enzymatic reactivity for different substrates using transferable data-driven collective variables. Proceedings of the National Academy of Sciences. 121 (2024)](http://dx.doi.org/10.1073/pnas.2416621121)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [..._pathCV_allcontacts1+torsion+Z_waterCV_align2z.dat](./data/maltohexaose/biased_MD/plumed_pathCV_allcontacts1+torsion+Z_waterCV_align2z.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/maltohexaose/biased_MD/plumed_pathCV_allcontacts1+torsion+Z_waterCV_align2z.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/maltohexaose/biased_MD/plumed_pathCV_allcontacts1+torsion+Z_waterCV_align2z.dat.plumed_master.stderr) |  
| [..._pathCV_allcontacts1+torsion+Z_waterCV_align2z.dat](./data/maltotetraose/biased_MD/plumed_pathCV_allcontacts1+torsion+Z_waterCV_align2z.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/maltotetraose/biased_MD/plumed_pathCV_allcontacts1+torsion+Z_waterCV_align2z.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/maltotetraose/biased_MD/plumed_pathCV_allcontacts1+torsion+Z_waterCV_align2z.dat.plumed_master.stderr) |  
| [..._pathCV_allcontacts1+torsion+Z_waterCV_align2z.dat](./data/maltotriose/biased_MD/plumed_pathCV_allcontacts1+torsion+Z_waterCV_align2z.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/maltotriose/biased_MD/plumed_pathCV_allcontacts1+torsion+Z_waterCV_align2z.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/maltotriose/biased_MD/plumed_pathCV_allcontacts1+torsion+Z_waterCV_align2z.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:27:49
  
**Project description and instructions**  
This egg contains the input files for replicating the unbiased classical MD simulations and enhanced sampling OPES simulations using Deep TDA CVs, and path CV for alpha-amylase enzyme with four different sugar substrates. The path CV used in OPES simulations enhances the sampling (in the Deep TDA CVs’ space) of different substrate-binding modes within the enzyme’s active site. For more information about Deep TDA, we refer to plumID:21.028. The CVs were trained with Pytorch version 1.8 and the simulations were run with GROMACS 2021.5, and PLUMED 2.9.

  
**Submission history**  
**[v1]** 26 Oct 2024: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:24.025" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:24.025](https://www.plumed-nest.org/eggs/24/025/badge.svg)](https://www.plumed-nest.org/eggs/24/025/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/24/025/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/24/025/badge.svg" alt="plumID:24.025"&gt;&lt;/a&gt;</pre>
  </div>
</div>
