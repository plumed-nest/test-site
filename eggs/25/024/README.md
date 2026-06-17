**Project ID:** [plumID:25.024]({{ '/' | absolute_url }}eggs/25/024/)  
**Name:**  Sampling glycan-glycan interactions for B22 calculations  
**Archive:** [ https://github.com/IsabellGrothaus/Data_repository/raw/main/Grothaus_et_al_2025_B22_PLUMED.zip](https://github.com/IsabellGrothaus/Data_repository/raw/main/Grothaus_et_al_2025_B22_PLUMED.zip)  
**Category:**  bio  
**Keywords:**  B22, glycan, carbohydrates, distance, REST2, metadynamics, RECT, replica exchange  
**PLUMED version:**  2.8  
**Contributor:**  Isabell Louise Grothaus  
**Submitted on:** 27 Aug 2025  
**Publication:** unpublished  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [A2G2S2_longbox.dat](./data/A2G2S2_longbox.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/A2G2S2_longbox.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/A2G2S2_longbox.dat.plumed_master.stderr) |  
| [glucose_longbox.dat](./data/glucose_longbox.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/glucose_longbox.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/glucose_longbox.dat.plumed_master.stderr) |  
  
**Last tested:**  17 Jun 2026, 09:07:57
  
**Project description and instructions**  
Example plumed.dat (glucose_longbox.dat) file to sample COM-distance between two glucose molecules from a standard MD with restraints in x and y direction. Example plumed.dat (A2G2S2_longbox.dat) file to sample COM-distances between two complex N-glycan molecules with restraints in x and y. The distance is additionally biased via a metadynamics potential across multiple replica (RECT), where the glycan molecules are defined as the solute (hot) region (REST2) for enhanced sampling of their conformational phase space. Perform REST-RECT simulations of glycans in solution or bound as substrate to their respective enzyme. GROMACS 2022 was used.

  
{% raw %}
<b><a href="https://www.plumed.org/doc-master/user-doc/html/actionlist/?actions=PRINT,POSITION,RESTRAINT,COMBINE,DISTANCE,COM,METAD" target="_blank">Click here</a> to open manual pages for actions used in this project.</b>
{% endraw %}
**Submission history**  
**[v1]** 27 Aug 2025: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:25.024" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:25.024](https://www.plumed-nest.org/eggs/25/024/badge.svg)](https://www.plumed-nest.org/eggs/25/024/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/25/024/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/25/024/badge.svg" alt="plumID:25.024"&gt;&lt;/a&gt;</pre>
  </div>
</div>
