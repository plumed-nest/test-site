**Project ID:** [plumID:22.013]({{ '/' | absolute_url }}eggs/22/013/)  
**Name:**  Ligand dissociation from PreQ1 riboswitch  
**Archive:** [ https://github.com/yhwang17/Prave-PreQ1_riboswitch/raw/main/plumed.zip](https://github.com/yhwang17/Prave-PreQ1_riboswitch/raw/main/plumed.zip)  
**Category:**  bio  
**Keywords:**  ligand, RNA, metadynamics, pRAVE  
**PLUMED version:**  2.5  
**Contributor:**  Yihang Wang  
**Submitted on:** 25 Mar 2022  
**Publication:** [Y. Wang, S. Parmar, J. S. Schneekloth, P. Tiwary, Interrogating RNA–Small Molecule Interactions with Structure Probing and Artificial Intelligence-Augmented Molecular Simulations. ACS Central Science. 8, 741–748 (2022)](http://dx.doi.org/10.1021/acscentsci.2c00149)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [plumed/6e1u/analysis/plumed.c-c_distance.dat](./data/plumed/6e1u/analysis/plumed.c-c_distance.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed/6e1u/analysis/plumed.c-c_distance.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed/6e1u/analysis/plumed.c-c_distance.dat.plumed_master.stderr) |  
| [plumed/6e1u/production/plumed.production.dat](./data/plumed/6e1u/production/plumed.production.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed/6e1u/production/plumed.production.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed/6e1u/production/plumed.production.dat.plumed_master.stderr) |  
| [plumed/6e1w/analysis/plumed.c-c_distance.dat](./data/plumed/6e1w/analysis/plumed.c-c_distance.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed/6e1w/analysis/plumed.c-c_distance.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed/6e1w/analysis/plumed.c-c_distance.dat.plumed_master.stderr) |  
| [plumed/6e1w/production/plumed.production.dat](./data/plumed/6e1w/production/plumed.production.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed/6e1w/production/plumed.production.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed/6e1w/production/plumed.production.dat.plumed_master.stderr) |  
| [plumed/apo/analysis/plumed.c-c_distance.dat](./data/plumed/apo/analysis/plumed.c-c_distance.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed/apo/analysis/plumed.c-c_distance.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed/apo/analysis/plumed.c-c_distance.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:34:02
  
**Project description and instructions**  
The PLUMED files in the production folder can be run with GROMACS 2018.3 using "gmx mdrun md_0_1 -plumed plumed.production.dat". Please refer to the README file [here](https://github.com/yhwang17/Prave-PreQ1_riboswitch) about how to generate the MD files.  The PLUMED files in the analysis folders can be run with "plumed driver --plumed.c-c_distance.dat --mf_xtc md_0_1.xtc".

  
**Submission history**  
**[v1]** 25 Mar 2022: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:22.013" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:22.013](https://www.plumed-nest.org/eggs/22/013/badge.svg)](https://www.plumed-nest.org/eggs/22/013/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/22/013/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/22/013/badge.svg" alt="plumID:22.013"&gt;&lt;/a&gt;</pre>
  </div>
</div>
