**Project ID:** [plumID:25.003]({{ '/' | absolute_url }}eggs/25/003/)  
**Name:**  Surrogate Model CV  
**Archive:** [ https://github.com/sompriya/Surrogate_CV/archive/main.zip](https://github.com/sompriya/Surrogate_CV/archive/main.zip) [(browse)](https://github.com/sompriya/Surrogate_CV/tree/main)  
**Category:**  methods  
**Keywords:**  Metadynamics, OPES, Machine Learning, Collective Variable, Protein Folding  
**PLUMED version:**  2.10  
**Contributor:**  Sompriya Chatterjee  
**Submitted on:** 24 Jan 2025  
**Last revised:** 16 Jul 2025  
**Publication:** [S. Chatterjee, D. Ray, Acceleration with Interpretability: A Surrogate Model-Based Collective Variable for Enhanced Sampling. Journal of Chemical Theory and Computation 21, 1561–1571 (2025)](http://dx.doi.org/10.1021/acs.jctc.4c01603)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [Alanine_dipeptide/OPES/plumed_all.dat](./data/Alanine_dipeptide/OPES/plumed_all.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/Alanine_dipeptide/OPES/plumed_all.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/Alanine_dipeptide/OPES/plumed_all.dat.plumed_master.stderr) |  
| [...lanine_dipeptide/OPES_Flooding/plumed_kinetics.dat](./data/Alanine_dipeptide/OPES_Flooding/plumed_kinetics.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/Alanine_dipeptide/OPES_Flooding/plumed_kinetics.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/Alanine_dipeptide/OPES_Flooding/plumed_kinetics.dat.plumed_master.stderr) |  
| [Chignolin/OPES/plumed.dat](./data/Chignolin/OPES/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/Chignolin/OPES/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/Chignolin/OPES/plumed.dat.plumed_master.stderr) |  
| [Chignolin/OPES_Flooding/plumed_kinetics.dat](./data/Chignolin/OPES_Flooding/plumed_kinetics.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/Chignolin/OPES_Flooding/plumed_kinetics.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/Chignolin/OPES_Flooding/plumed_kinetics.dat.plumed_master.stderr) |  
  
**Last tested:**  17 Jun 2026, 09:08:57
  
**Project description and instructions**  
We used GROMACS 2024.3 with PLUMED 2.10 for performing all simulations. 

  
{% raw %}
<b><a href="https://www.plumed.org/doc-master/user-doc/html/actionlist/?actions=PYTORCH_MODEL,CUSTOM,WHOLEMOLECULES,COMBINE,MOLINFO,MATHEVAL,DISTANCE,OPES_METAD,GROUP,TORSION,ENDPLUMED,COMMITTOR,ENERGY,PRINT" target="_blank">Click here</a> to open manual pages for actions used in this project.</b>
{% endraw %}
**Submission history**  
**[v1]** 24 Jan 2025: original submission  
**[v2]** 16 Jul 2025: updated reference  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:25.003" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:25.003](https://www.plumed-nest.org/eggs/25/003/badge.svg)](https://www.plumed-nest.org/eggs/25/003/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/25/003/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/25/003/badge.svg" alt="plumID:25.003"&gt;&lt;/a&gt;</pre>
  </div>
</div>
