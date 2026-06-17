**Project ID:** [plumID:24.001]({{ '/' | absolute_url }}eggs/24/001/)  
**Name:**  A Kinetic View of Enzyme Catalysis from Enhanced Sampling QM/MM Simulations  
**Archive:** [ https://github.com/dhimanray/Enzyme_Kinetics_OPES_flooding/archive/main.zip](https://github.com/dhimanray/Enzyme_Kinetics_OPES_flooding/archive/main.zip) [(browse)](https://github.com/dhimanray/Enzyme_Kinetics_OPES_flooding/tree/main)  
**Category:**  bio  
**Keywords:**  OPES, OPES-Flooding, QM/MM, Kinetics, Enzyme Catalysis  
**PLUMED version:**  2.9  
**Contributor:**  Dhiman Ray  
**Submitted on:** 30 Jan 2024  
**Publication:** [D. Ray, S. Das, U. Raucci, Kinetic View of Enzyme Catalysis from Enhanced Sampling QM/MM Simulations. Journal of Chemical Information and Modeling 64, 3953–3958 (2024)](http://dx.doi.org/10.1021/acs.jcim.4c00475)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [amylase/opes_flooding_qmmm/plumed.dat](./data/amylase/opes_flooding_qmmm/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/amylase/opes_flooding_qmmm/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/amylase/opes_flooding_qmmm/plumed.dat.plumed_master.stderr) |  
| [chorismate_mutase/opes_flooding_qmmm/plumed.dat](./data/chorismate_mutase/opes_flooding_qmmm/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/chorismate_mutase/opes_flooding_qmmm/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/chorismate_mutase/opes_flooding_qmmm/plumed.dat.plumed_master.stderr) |  
| [chorismate_mutase/opes_mm/plumed.dat](./data/chorismate_mutase/opes_mm/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/chorismate_mutase/opes_mm/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/chorismate_mutase/opes_mm/plumed.dat.plumed_master.stderr) |  
  
**Last tested:**  17 Jun 2026, 09:13:15
  
**Project description and instructions**  
To perform OPES simulation at MM level we used GROMACS v2022. For OPES flooding simulation at QM/MM level we used CP2K v9.1. Python scripts have been used for rescaling transition times and for KS tests.

  
{% raw %}
<b><a href="https://www.plumed.org/doc-master/user-doc/html/actionlist/?actions=UPPER_WALLS,COMBINE,TORSION,CUSTOM,COMMITTOR,LOWER_WALLS,UNITS,OPES_METAD,FLUSH,PRINT,DISTANCE" target="_blank">Click here</a> to open manual pages for actions used in this project.</b>
{% endraw %}
**Submission history**  
**[v1]** 30 Jan 2024: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:24.001" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:24.001](https://www.plumed-nest.org/eggs/24/001/badge.svg)](https://www.plumed-nest.org/eggs/24/001/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/24/001/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/24/001/badge.svg" alt="plumID:24.001"&gt;&lt;/a&gt;</pre>
  </div>
</div>
