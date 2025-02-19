**Project ID:** [plumID:19.029]({{ '/' | absolute_url }}eggs/19/029/)  
**Name:**  WTE-metaD of FF domain of URNF1 C57D variant  
**Archive:** [ https://github.com/ELELAB/URNF1_FF_publication/raw/master/archive_URNF1_FF_plumed_nest.zip](https://github.com/ELELAB/URNF1_FF_publication/raw/master/archive_URNF1_FF_plumed_nest.zip)  
**Category:**  bio  
**Keywords:**  metadynamics, mutations, post-translational modification, ff domain  
**PLUMED version:**  2.2  
**Contributor:**  Elena Papaleo  
**Submitted on:** 06 May 2019  
**Publication:** [P. Marinelli, S. Navarro, R. Graña-Montes, M. Bañó-Polo, M. R. Fernández, E. Papaleo, S. Ventura, A single cysteine post-translational oxidation suffices to compromise globular proteins kinetic stability and promote amyloid formation. Redox Biology. 14, 566–575 (2018)](http://dx.doi.org/10.1016/j.redox.2017.10.022)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [C57D.plumed2/plumed.dat](./data/C57D.plumed2/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/C57D.plumed2/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/C57D.plumed2/plumed.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:43:05
  
**Project description and instructions**  
This repository contains the input data for the wte metadynamics simulations of our publication. The calculations were originally performed with the PLUMED 1.3 plugin and Gromacs 4.6.5 but we also provide an input file in the version for PLUMED 2 for one of the variants as an example (to be found in the folder C57D_plumed2). The three main folders in the repository contain (WT) input files for metaD of the wild-type variant (C57D) input files for metaD of the mutant variant (C57D.plumed2) corresponding input files for PLUMED 2. NB. the original mdp files were set for 1000 ns but we collected 550 ns per analysis, as explained in the article.

  
**Submission history**  
**[v1]** 06 May 2019: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:19.029" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:19.029](https://www.plumed-nest.org/eggs/19/029/badge.svg)](https://www.plumed-nest.org/eggs/19/029/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/19/029/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/19/029/badge.svg" alt="plumID:19.029"&gt;&lt;/a&gt;</pre>
  </div>
</div>
