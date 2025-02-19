**Project ID:** [plumID:22.039]({{ '/' | absolute_url }}eggs/22/039/)  
**Name:**  Driving and characterizing nucleation of urea and glycine polymorphs in water  
**Archive:** [ https://github.com/tiwarylab/Driving-and-characterizing-nucleation-of-urea-and-glycine-polymorphs-in-water/raw/main/plumed.zip](https://github.com/tiwarylab/Driving-and-characterizing-nucleation-of-urea-and-glycine-polymorphs-in-water/raw/main/plumed.zip)  
**Category:**  bio  
**Keywords:**  metadynamics, nucleation, amino acids, polymorphism  
**PLUMED version:**  2.6.1  
**Contributor:**  Eric Beyerle  
**Submitted on:** 02 Nov 2022  
**Publication:** [Z. Zou, E. R. Beyerle, S.-T. Tsai, P. Tiwary, Driving and characterizing nucleation of urea and glycine polymorphs in water. Proceedings of the National Academy of Sciences. 120 (2023)](http://dx.doi.org/10.1073/pnas.2216099120)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [urea_plumed.dat](./data/urea_plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/urea_plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/urea_plumed.dat.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
| [glycine_plumed.dat](./data/glycine_plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/glycine_plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/glycine_plumed.dat.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
  
**Last tested:**  19 Feb 2025, 14:27:39
  
**Project description and instructions**  
Run using PLUMED driver. plumed driver --mf_xtc ${sys}.xtc --plumed ${sys}_plumed.dat, where ${sys} is one of urea or glycine and ${sys}.xtc is the XTC file generated from a GROMACS trajectory. Of course, any other PLUMED driver supported trajectories should work, and the flag changed appropriately.

  
**Submission history**  
**[v1]** 02 Nov 2022: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:22.039" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:22.039](https://www.plumed-nest.org/eggs/22/039/badge.svg)](https://www.plumed-nest.org/eggs/22/039/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/22/039/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/22/039/badge.svg" alt="plumID:22.039"&gt;&lt;/a&gt;</pre>
  </div>
</div>
