**Project ID:** [plumID:23.014]({{ '/' | absolute_url }}eggs/23/014/)  
**Name:**  Structural basis of dimerization of chemokine receptors CCR5 and CXCR4  
**Archive:** [ https://github.com/limresgrp/chemokine_receptors_oligomerization/raw/main/plumed_input.zip](https://github.com/limresgrp/chemokine_receptors_oligomerization/raw/main/plumed_input.zip)  
**Category:**  bio  
**Keywords:**  metadynamics, oligomerization, chemokine receptors, GPCR, membrane  
**PLUMED version:**  2.3  
**Contributor:**  Vittorio Limongelli  
**Submitted on:** 24 Mar 2023  
**Publication:** [D. Di Marino, P. Conflitti, S. Motta, V. Limongelli, Structural basis of dimerization of chemokine receptors CCR5 and CXCR4. Nature Communications. 14 (2023)](http://dx.doi.org/10.1038/s41467-023-42082-z)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [CCR5-CXCR4_dimer/plumed_CCR5_CXCR4.dat](./data/CCR5-CXCR4_dimer/plumed_CCR5_CXCR4.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/CCR5-CXCR4_dimer/plumed_CCR5_CXCR4.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/CCR5-CXCR4_dimer/plumed_CCR5_CXCR4.dat.plumed_master.stderr) |  
| [CCR5_dimer/plumed_CCR5_dimer.dat](./data/CCR5_dimer/plumed_CCR5_dimer.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/CCR5_dimer/plumed_CCR5_dimer.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/CCR5_dimer/plumed_CCR5_dimer.dat.plumed_master.stderr) |  
| [CXCR4_dimer/plumed_CXCR4_dimer.dat](./data/CXCR4_dimer/plumed_CXCR4_dimer.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/CXCR4_dimer/plumed_CXCR4_dimer.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/CXCR4_dimer/plumed_CXCR4_dimer.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:33:08
  
**Project description and instructions**  
MD simulations can be performed using GROMACS 5.1 or later patched with PLUMED 2.3 and using the following command. gmx mdrun -v -deffnm prod -plumed plumed_{dimer_name}.dat
  
**Submission history**  
**[v1]** 24 Mar 2023: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:23.014" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:23.014](https://www.plumed-nest.org/eggs/23/014/badge.svg)](https://www.plumed-nest.org/eggs/23/014/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/23/014/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/23/014/badge.svg" alt="plumID:23.014"&gt;&lt;/a&gt;</pre>
  </div>
</div>
