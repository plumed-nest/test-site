**Project ID:** [plumID:21.044]({{ '/' | absolute_url }}eggs/21/044/)  
**Name:**  NaCl nucleation  
**Archive:** [ https://github.com/aaronrfinney/plumed-nest/raw/main/NaCl_nucleation_nest.zip](https://github.com/aaronrfinney/plumed-nest/raw/main/NaCl_nucleation_nest.zip)  
**Category:**  chemistry  
**Keywords:**  metadynamics, DFS clustering  
**PLUMED version:**  2.5.1  
**Contributor:**  Aaron Finney  
**Submitted on:** 11 Nov 2021  
**Publication:** [A. R. Finney, M. Salvalaglio, Multiple pathways in NaCl homogeneous crystal nucleation. Faraday Discussions. 235, 56–80 (2022)](http://dx.doi.org/10.1039/D1FD00089F)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [plumed.dat](./data/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed.dat.plumed_master.stderr) |  
| [driver.dat](./data/driver.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/driver.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/driver.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:44:57
  
**Project description and instructions**  
Run metadynamics with GROMACS 2018.6 according to e.g., *gmx mdrun -deffnm md -plumed plumed.dat*.  Trajectories can be post-processed using PLUMED driver and the command *plumed driver --plumed driver.dat --mf_xtc mytrj.xtc --timestep 0.001 --trajectory-stride 100*.  For analysis using *driver.dat*. PLUMED must be configured with the crystallization and adjmat modules (see the [PLUMED documentation](https://www.plumed.org/doc)).

  
**Submission history**  
**[v1]** 11 Nov 2021: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:21.044" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:21.044](https://www.plumed-nest.org/eggs/21/044/badge.svg)](https://www.plumed-nest.org/eggs/21/044/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/21/044/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/21/044/badge.svg" alt="plumID:21.044"&gt;&lt;/a&gt;</pre>
  </div>
</div>
