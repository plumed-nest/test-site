**Project ID:** [plumID:23.027]({{ '/' | absolute_url }}eggs/23/027/)  
**Name:**  CmuMD simulations of NaCl(aq) at NaCl  
**Archive:** [ https://github.com/aaronrfinney/plumed-nest/raw/main/NaCl_charged_graphite.zip](https://github.com/aaronrfinney/plumed-nest/raw/main/NaCl_charged_graphite.zip)  
**Category:**  chemistry  
**Keywords:**  CmuMD, DFS, Q3, Pair Entropy  
**PLUMED version:**  2.5.1  
**Contributor:**  Aaron Finney  
**Submitted on:** 04 Jul 2023  
**Publication:** [A. R. Finney, M. Salvalaglio, Properties of aqueous electrolyte solutions at carbon electrodes: effects of concentration and surface charge on solution structure, ion clustering and thermodynamics in the electric double layer. Faraday Discussions. 249, 334–362 (2024)](http://dx.doi.org/10.1039/D3FD00133D)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [water-structure-driver.dat](./data/water-structure-driver.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/water-structure-driver.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/water-structure-driver.dat.plumed_master.stderr) |  
| [ion-structure-driver.dat](./data/ion-structure-driver.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/ion-structure-driver.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/ion-structure-driver.dat.plumed_master.stderr) |  
| [plumed.dat](./data/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-failed-red.svg)](data/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/plumed.dat.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
  
**Last tested:**  19 Feb 2025, 14:33:46
  
**Project description and instructions**  
Run using GROMACS (2018.6) according to e.g., gmx mdrun -deffnm cmumd -cpi md.cpt -plumed plumed.dat. ion-structure-driver.dat and water-structure-driver.dat are PLUMED driver files to post-process the trajectories. Execute them using, plumed driver --plumed ion-structure-driver.dat --mf_xtc md.xtc.
  
**Submission history**  
**[v1]** 04 Jul 2023: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:23.027" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:23.027](https://www.plumed-nest.org/eggs/23/027/badge.svg)](https://www.plumed-nest.org/eggs/23/027/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/23/027/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/23/027/badge.svg" alt="plumID:23.027"&gt;&lt;/a&gt;</pre>
  </div>
</div>
