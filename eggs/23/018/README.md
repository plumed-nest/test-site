**Project ID:** [plumID:23.018]({{ '/' | absolute_url }}eggs/23/018/)  
**Name:**  Anisotropic Gold Nanomaterial Synthesis Using Peptide Facet Specificity and Timed Intervention  
**Archive:** [ https://github.com/katorke/Au_Facet_Selectivity/raw/main/plumed_nest.zip](https://github.com/katorke/Au_Facet_Selectivity/raw/main/plumed_nest.zip)  
**Category:**  materials  
**Keywords:**  metadynamics, surface binding, peptide adsorption  
**PLUMED version:**  2.8  
**Contributor:**  Kaylyn Torkelson  
**Submitted on:** 11 May 2023  
**Publication:** [K. J. Lachowski, H. T. Chiang, K. Torkelson, W. Zhou, S. Zhang, J. Pfaendtner, L. D. Pozzo, Anisotropic Gold Nanomaterial Synthesis Using Peptide Facet Specificity and Timed Intervention. Langmuir. 39, 15878–15888 (2023)](http://dx.doi.org/10.1021/acs.langmuir.3c01577)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [Z2M246I_Au100/plumed.dat](./data/Z2M246I_Au100/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/Z2M246I_Au100/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/Z2M246I_Au100/plumed.dat.plumed_master.stderr) |  
| [Z2M246I_Au111/plumed.dat](./data/Z2M246I_Au111/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/Z2M246I_Au111/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/Z2M246I_Au111/plumed.dat.plumed_master.stderr) |  
| [Z2_Au100/plumed.dat](./data/Z2_Au100/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/Z2_Au100/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/Z2_Au100/plumed.dat.plumed_master.stderr) |  
| [Z2_Au111/plumed.dat](./data/Z2_Au111/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/Z2_Au111/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/Z2_Au111/plumed.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:23:18
  
**Project description and instructions**  
Each directory (Z2_Au100, Z2_Au111, Z2M246I_Au100, Z2M246I_Au111) contains an initial gro file (system.gro) for the system, a corresponding index file (system.ndx), a reference PDB for each peptide, the files necessary for the topology of the system (topol.top/*.itp), and the plumed file (plumed.dat) that was used to run each metadynamics calculation in Gromacs 2020.5. The main directory contains an example MDP file, the forcefield that was used for Au interactions, and the ndx files corresponding to the Au(111) and Au(100) surfaces.
  
**Submission history**  
**[v1]** 11 May 2023: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:23.018" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:23.018](https://www.plumed-nest.org/eggs/23/018/badge.svg)](https://www.plumed-nest.org/eggs/23/018/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/23/018/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/23/018/badge.svg" alt="plumID:23.018"&gt;&lt;/a&gt;</pre>
  </div>
</div>
