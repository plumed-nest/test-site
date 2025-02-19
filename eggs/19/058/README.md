**Project ID:** [plumID:19.058]({{ '/' | absolute_url }}eggs/19/058/)  
**Name:**  Constrained MD for maintaining a cavity in a calculation  
**Archive:** [ https://github.com/JelfsMaterialsGroup/PLUMED_files/raw/master/ConstrainedMD.zip](https://github.com/JelfsMaterialsGroup/PLUMED_files/raw/master/ConstrainedMD.zip)  
**Category:**  chemistry  
**Keywords:**  constrained MD, porous molecules, porosity, cavity  
**PLUMED version:**  2.5  
**Contributor:**  Kim Jelfs  
**Submitted on:** 12 Jul 2019  
**Publication:** [V. Santolini, G. A. Tribello, K. E. Jelfs, Predicting solvent effects on the structure of porous organic molecules. Chemical Communications. 51, 15542–15545 (2015)](http://dx.doi.org/10.1039/C5CC05344G)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [plumed_cylinder.dat](./data/plumed_cylinder.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed_cylinder.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed_cylinder.dat.plumed_master.stderr) |  
| [plumed_sphere.dat](./data/plumed_sphere.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed_sphere.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed_sphere.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:49:49
  
**Project description and instructions**  
The files can be used with DLPOLY2.20 and a porous molecule in order to run a constrained MD simulation where none of a set of numbered atoms are allowed to go within a defined cavity of that molecule. One example is for a spherical cavity, the other for a cylindrical cavity. 

  
**Submission history**  
**[v1]** 12 Jul 2019: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:19.058" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:19.058](https://www.plumed-nest.org/eggs/19/058/badge.svg)](https://www.plumed-nest.org/eggs/19/058/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/19/058/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/19/058/badge.svg" alt="plumID:19.058"&gt;&lt;/a&gt;</pre>
  </div>
</div>
