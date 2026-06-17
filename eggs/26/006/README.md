**Project ID:** [plumID:26.006]({{ '/' | absolute_url }}eggs/26/006/)  
**Name:**  Metadynamics simulations of buried phosphorylation sites and proline isomerisation  
**Archive:** [ https://github.com/julian-streit/PTM_MD_analyses/raw/main/PLUMED.zip](https://github.com/julian-streit/PTM_MD_analyses/raw/main/PLUMED.zip)  
**Category:**  bio  
**Keywords:**  metadynamics  
**PLUMED version:**  2.9  
**Contributor:**  Julian Streit  
**Submitted on:** 12 May 2026  
**Publication:** [B. Lang, J. O. Streit, R. W. Kriwacki, J. Christodoulou, M. M. Babu, Protein Dynamics at Different Timescales Unlock Access to Hidden Post-Translational Modification Sites. doi: 10.1101/2025.06.25.661537 (2025)](http://dx.doi.org/10.1101/2025.06.25.661537)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [FLN5_FL_METAD/plumed.dat](./data/FLN5_FL_METAD/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/FLN5_FL_METAD/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/FLN5_FL_METAD/plumed.dat.plumed_master.stderr) |  
| [FLN5_U_METAD/plumed.dat](./data/FLN5_U_METAD/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/FLN5_U_METAD/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/FLN5_U_METAD/plumed.dat.plumed_master.stderr) |  
| [FLNA21_METAD/plumed.dat](./data/FLNA21_METAD/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/FLNA21_METAD/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/FLNA21_METAD/plumed.dat.plumed_master.stderr) |  
| [FLNA21_pS2319_trans_METAD/plumed.dat](./data/FLNA21_pS2319_trans_METAD/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/FLNA21_pS2319_trans_METAD/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/FLNA21_pS2319_trans_METAD/plumed.dat.plumed_master.stderr) |  
| [FLNC24_METAD/plumed.dat](./data/FLNC24_METAD/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/FLNC24_METAD/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/FLNC24_METAD/plumed.dat.plumed_master.stderr) |  
| [FLNC24_pS2718_trans_METAD/plumed.dat](./data/FLNC24_pS2718_trans_METAD/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/FLNC24_pS2718_trans_METAD/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/FLNC24_pS2718_trans_METAD/plumed.dat.plumed_master.stderr) |  
| [PARK7_METAD_chainA/plumed.dat](./data/PARK7_METAD_chainA/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/PARK7_METAD_chainA/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/PARK7_METAD_chainA/plumed.dat.plumed_master.stderr) |  
| [PARK7_TYR_COORD_METAD_BF40/plumed.dat](./data/PARK7_TYR_COORD_METAD_BF40/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/PARK7_TYR_COORD_METAD_BF40/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/PARK7_TYR_COORD_METAD_BF40/plumed.dat.plumed_master.stderr) |  
| [PARK7_chainA_pY67_TYR_COORD_METAD_BF40/plumed.dat](./data/PARK7_chainA_pY67_TYR_COORD_METAD_BF40/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/PARK7_chainA_pY67_TYR_COORD_METAD_BF40/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/PARK7_chainA_pY67_TYR_COORD_METAD_BF40/plumed.dat.plumed_master.stderr) |  
  
**Last tested:**  17 Jun 2026, 09:06:10
  
**Project description and instructions**  
plumed.dat activates the METAD bias for a new simulation. Simulations were performed with GROMACS 2022.4 + GROMACS 2.8.2 (FLN5) and GROMACS 2020.4 + PLUMED 2.6.2 or GROMACS 2023.5 + PLUMED 2.9.3 for FLNA21, FLNC24, PARK7. 

  
{% raw %}
<b><a href="https://www.plumed.org/doc-master/user-doc/html/actionlist/?actions=WHOLEMOLECULES,COORDINATION,PRINT,MOLINFO,METAD,TORSION" target="_blank">Click here</a> to open manual pages for actions used in this project.</b>
{% endraw %}
**Submission history**  
**[v1]** 12 May 2026: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:26.006" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:26.006](https://www.plumed-nest.org/eggs/26/006/badge.svg)](https://www.plumed-nest.org/eggs/26/006/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/26/006/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/26/006/badge.svg" alt="plumID:26.006"&gt;&lt;/a&gt;</pre>
  </div>
</div>
