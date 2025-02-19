**Project ID:** [plumID:22.031]({{ '/' | absolute_url }}eggs/22/031/)  
**Name:**  Rare Event Kinetics from Adaptive Bias Enhanced Sampling  
**Archive:** [ https://github.com/dhimanray/OPES-Flooding/archive/main.zip](https://github.com/dhimanray/OPES-Flooding/archive/main.zip) [(browse)](https://github.com/dhimanray/OPES-Flooding/tree/main)  
**Category:**  methods  
**Keywords:**  OPES Flooding, Kinetics, Rate, OPES, Machine Learning  
**PLUMED version:**  2.9  
**Contributor:**  Dhiman Ray  
**Submitted on:** 11 Aug 2022  
**Last revised:** 14 Nov 2022  
**Publication:** [D. Ray, N. Ansari, V. Rizzi, M. Invernizzi, M. Parrinello, Rare Event Kinetics from Adaptive Bias Enhanced Sampling. Journal of Chemical Theory and Computation. 18, 6500–6509 (2022)](http://dx.doi.org/10.1021/acs.jctc.2c00806)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [2D_Potential/s27/plumed.dat](./data/2D_Potential/s27/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/2D_Potential/s27/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/2D_Potential/s27/plumed.dat.plumed_master.stderr) |  
| [2D_Potential/s54/plumed.dat](./data/2D_Potential/s54/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/2D_Potential/s54/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/2D_Potential/s54/plumed.dat.plumed_master.stderr) |  
| [2D_Potential/s90/plumed.dat](./data/2D_Potential/s90/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/2D_Potential/s90/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/2D_Potential/s90/plumed.dat.plumed_master.stderr) |  
| [Ala2/phi/plumed.dat](./data/Ala2/phi/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/Ala2/phi/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/Ala2/phi/plumed.dat.plumed_master.stderr) |  
| [Ala2/psi/plumed.dat](./data/Ala2/psi/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/Ala2/psi/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/Ala2/psi/plumed.dat.plumed_master.stderr) |  
| [Chignolin/folding/plumed-descriptors.dat](./data/Chignolin/folding/plumed-descriptors.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/Chignolin/folding/plumed-descriptors.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/Chignolin/folding/plumed-descriptors.dat.plumed_master.stderr) |  
| [Chignolin/folding/plumed_rate.dat](./data/Chignolin/folding/plumed_rate.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/Chignolin/folding/plumed_rate.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/Chignolin/folding/plumed_rate.dat.plumed_master.stderr) |  
| [Chignolin/unfolding/plumed-descriptors.dat](./data/Chignolin/unfolding/plumed-descriptors.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/Chignolin/unfolding/plumed-descriptors.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/Chignolin/unfolding/plumed-descriptors.dat.plumed_master.stderr) |  
| [Chignolin/unfolding/plumed_rate.dat](./data/Chignolin/unfolding/plumed_rate.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/Chignolin/unfolding/plumed_rate.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/Chignolin/unfolding/plumed_rate.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:32:43
  
**Project description and instructions**  
Introducing the OPES Flooding method for calculating kinetics of rare event processes. It is tested on model systems and folding/unfolding of chignolin. The MD engine used is GROMACS 2021. The Deep-LDA and Deep-TICA CV were trained using Pytorch 1.8.2 and mlcvs package. Note. The OPES flooding method is available from PLUMED version 2.8. But the Deep-LDA and Deep-TICA CV we used in this work are implemented in PLUMED 2.9.

  
**Submission history**  
**[v1]** 11 Aug 2022: original submission  
**[v2]** 14 Nov 2022: updated doi  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:22.031" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:22.031](https://www.plumed-nest.org/eggs/22/031/badge.svg)](https://www.plumed-nest.org/eggs/22/031/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/22/031/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/22/031/badge.svg" alt="plumID:22.031"&gt;&lt;/a&gt;</pre>
  </div>
</div>
