**Project ID:** [plumID:22.030]({{ '/' | absolute_url }}eggs/22/030/)  
**Name:**  Mixing physics across temperatures with generative artificial intelligence  
**Archive:** [ https://github.com/yhwang17/Plumed_DDPM_REMD/raw/main/plumed.zip](https://github.com/yhwang17/Plumed_DDPM_REMD/raw/main/plumed.zip)  
**Category:**  methods  
**Keywords:**  REMD, Generative AI, DDPM  
**PLUMED version:**  2.4  
**Contributor:**  Yihang Wang  
**Submitted on:** 21 Jul 2022  
**Publication:** [Y. Wang, L. Herron, P. Tiwary, From data to noise to data for mixing physics across temperatures with generative artificial intelligence. Proceedings of the National Academy of Sciences. 119 (2022)](http://dx.doi.org/10.1073/pnas.2203656119)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [plumed/AIB9/plumed.dat](./data/plumed/AIB9/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed/AIB9/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed/AIB9/plumed.dat.plumed_master.stderr) |  
| [plumed/GACC/plumed.dat](./data/plumed/GACC/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed/GACC/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed/GACC/plumed.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:31:31
  
**Project description and instructions**  
The PLUMED files are used to calculate the dihedral angles of the systems, which are later used to train the generative models. They can be run with  GROMACS/2016.5 using “gmx mdrun md_0_1 -plumed plumed.dat".

  
**Submission history**  
**[v1]** 21 Jul 2022: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:22.030" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:22.030](https://www.plumed-nest.org/eggs/22/030/badge.svg)](https://www.plumed-nest.org/eggs/22/030/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/22/030/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/22/030/badge.svg" alt="plumID:22.030"&gt;&lt;/a&gt;</pre>
  </div>
</div>
