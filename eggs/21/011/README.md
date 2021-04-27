**Project ID:** [plumID:21.011]({{ '/' | absolute_url }}eggs/21/011/)  
**Name:**  CmuMD simulations of NaCl(aq) at graphite  
**Archive:** [ https://github.com/aaronrfinney/plumed-nest/raw/main/NaCl_at_graphite-cmumd.zip](https://github.com/aaronrfinney/plumed-nest/raw/main/NaCl_at_graphite-cmumd.zip)  
**Category:**  chemistry  
**Keywords:**  CmuMD, DFS clustering  
**PLUMED version:**  2.5.1  
**Contributor:**  Aaron Finney  
**Submitted on:** 19 Mar 2021  
**Publication:** unpublished  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [NaCl_at_graphite-cmumd/clusters.plmd](./data/NaCl_at_graphite-cmumd/clusters.plmd.md) |  [![tested on v2.7](https://img.shields.io/badge/v2.7-passing-green.svg)](data/NaCl_at_graphite-cmumd/clusters.plmd.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/NaCl_at_graphite-cmumd/clusters.plmd.plumed_master.stderr) |  
| [NaCl_at_graphite-cmumd/cmumd.plmd](./data/NaCl_at_graphite-cmumd/cmumd.plmd.md) |  [![tested on v2.7](https://img.shields.io/badge/v2.7-passing-green.svg)](data/NaCl_at_graphite-cmumd/cmumd.plmd.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/NaCl_at_graphite-cmumd/cmumd.plmd.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
| [NaCl_at_graphite-cmumd/coordination-profiles.plmd](./data/NaCl_at_graphite-cmumd/coordination-profiles.plmd.md) |  [![tested on v2.7](https://img.shields.io/badge/v2.7-passing-green.svg)](data/NaCl_at_graphite-cmumd/coordination-profiles.plmd.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/NaCl_at_graphite-cmumd/coordination-profiles.plmd.plumed_master.stderr) |  
  
**Last tested:**  27 Apr 2021, 22:18:44
  
**Project description and instructions**  
Run using GROMACS (2018.6) according to e.g., *gmx mdrun -deffnm cmumd -cpi md.cpt -plumed cmumd.plmd*. The files *coordination-profiles.plmd* and *clusters.plmd* are PLUMED driver files for post-processing of MD trajectory files. They generate average coordination number profiles and information regarding ion clusters in solution. More info can be found [here](https://github.com/mme-ucl/CmuMD).

  
**Submission history**  
**[v1]** 19 Mar 2021: original submission  
  
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
