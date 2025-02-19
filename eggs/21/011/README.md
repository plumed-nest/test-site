**Project ID:** [plumID:21.011]({{ '/' | absolute_url }}eggs/21/011/)  
**Name:**  CmuMD simulations of NaCl(aq) at graphite  
**Archive:** [ https://github.com/aaronrfinney/plumed-nest/raw/main/NaCl_at_graphite-cmumd.zip](https://github.com/aaronrfinney/plumed-nest/raw/main/NaCl_at_graphite-cmumd.zip)  
**Category:**  chemistry  
**Keywords:**  CmuMD, DFS clustering  
**PLUMED version:**  2.5.1  
**Contributor:**  Aaron Finney  
**Submitted on:** 19 Mar 2021  
**Last revised:** 04 Aug 2021  
**Publication:** [A. R. Finney, I. J. McPherson, P. R. Unwin, M. Salvalaglio, Electrochemistry, ion adsorption and dynamics in the double layer: a study of NaCl(aq) on graphite. Chemical Science. 12, 11166–11180 (2021)](http://dx.doi.org/10.1039/D1SC02289J)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [NaCl_at_graphite-cmumd/clusters.plmd](./data/NaCl_at_graphite-cmumd/clusters.plmd.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/NaCl_at_graphite-cmumd/clusters.plmd.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/NaCl_at_graphite-cmumd/clusters.plmd.plumed_master.stderr) |  
| [NaCl_at_graphite-cmumd/cmumd.plmd](./data/NaCl_at_graphite-cmumd/cmumd.plmd.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-failed-red.svg)](data/NaCl_at_graphite-cmumd/cmumd.plmd.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/NaCl_at_graphite-cmumd/cmumd.plmd.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
| [NaCl_at_graphite-cmumd/coordination-profiles.plmd](./data/NaCl_at_graphite-cmumd/coordination-profiles.plmd.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/NaCl_at_graphite-cmumd/coordination-profiles.plmd.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/NaCl_at_graphite-cmumd/coordination-profiles.plmd.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
  
**Last tested:**  19 Feb 2025, 14:30:55
  
**Project description and instructions**  
Run using GROMACS (2018.6) according to e.g., *gmx mdrun -deffnm cmumd -cpi md.cpt -plumed cmumd.plmd*. The files *coordination-profiles.plmd* and *clusters.plmd* are PLUMED driver files for post-processing of MD trajectory files. They generate average coordination number profiles and information regarding ion clusters in solution. More info can be found [here](https://github.com/mme-ucl/CmuMD).

  
**Submission history**  
**[v1]** 19 Mar 2021: original submission  
**[v2]** 04 Aug 2021: updated doi  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:21.011" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:21.011](https://www.plumed-nest.org/eggs/21/011/badge.svg)](https://www.plumed-nest.org/eggs/21/011/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/21/011/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/21/011/badge.svg" alt="plumID:21.011"&gt;&lt;/a&gt;</pre>
  </div>
</div>
