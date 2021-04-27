**Project ID:** [plumID:19.033]({{ '/' | absolute_url }}eggs/19/033/)  
**Name:**  PMD (path-metadynamics)  
**Archive:** [ http://www.acmm.nl/ensing/software/pmd_plumednest.zip](http://www.acmm.nl/ensing/software/pmd_plumednest.zip)  
**Category:**  methods  
**Keywords:**  path-CV, metadynamics, multiple-walker, polyproline  
**PLUMED version:**  2.3  
**Contributor:**  Bernd Ensing  
**Submitted on:** 07 May 2019  
**Last revised:** 17 Jun 2019  
**Publication:** [A. Pérez de Alba Ortíz, A. Tiwari, R. C. Puthenkalathil, B. Ensing, Advances in enhanced sampling along adaptive paths of collective variables, The Journal of Chemical Physics 149, 072320 (2018)](http://dx.doi.org/10.1063/1.5027392)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [pmd_plumednest/plumed.0.dat](./data/pmd_plumednest/plumed.0.dat.md) |  [![tested on v2.7](https://img.shields.io/badge/v2.7-passing-green.svg)](data/pmd_plumednest/plumed.0.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/pmd_plumednest/plumed.0.dat.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
  
**Last tested:**  27 Apr 2021, 22:54:59
  
**Project description and instructions**  
This allows to run multiple-walker path-metadynamics on the right- to left-handed helix transition in tetrameric polyproline with a 3D CV-space. It can be easily adjusted to bigger systems with higher-dimensional CV-spaces. It requires PLUMED compiled with MPI and with the Path-CV code provided [here](http://www.acmm.nl/ensing/software/index.html). It also requires an MD engine that can run parallel replicas. We use GROMACS 5.1.4 compiled with MPI. Notice that in the PLUMED input files WALKERS_ID must be adjusted for the different walkers.

  
**Submission history**  
**[v1]** 07 May 2019: original submission  
**[v2]** 17 Jun 2019: new archive  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:19.033" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:19.033](https://www.plumed-nest.org/eggs/19/033/badge.svg)](https://www.plumed-nest.org/eggs/19/033/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/19/033/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/19/033/badge.svg" alt="plumID:19.033"&gt;&lt;/a&gt;</pre>
  </div>
</div>
