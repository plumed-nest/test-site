**Project ID:** [plumID:26.005]({{ '/' | absolute_url }}eggs/26/005/)  
**Name:**  Cryptic pocket discovery in Alzheimer disease risk proteins BIN1, PICALM, and CD2AP via well-tempered metadynamics  
**Archive:** [ https://zenodo.org/records/19649272/files/plumed_nest_cryptad.zip](https://zenodo.org/records/19649272/files/plumed_nest_cryptad.zip)  
**Category:**  methods  
**Keywords:**  cryptic pockets, Alzheimer disease, BIN1, PICALM, CD2AP, well-tempered metadynamics, endocytosis, clathrin-mediated trafficking, virtual screening  
**PLUMED version:**  2.9  
**Contributor:**  Cagrı Ozkurt  
**Submitted on:** 19 Apr 2026  
**Publication:** unpublished  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [plumed_S5_CD2AP_SH3-1.dat](./data/plumed_S5_CD2AP_SH3-1.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed_S5_CD2AP_SH3-1.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed_S5_CD2AP_SH3-1.dat.plumed_master.stderr) |  
| [plumed_S4_CD2AP_SH3-2.dat](./data/plumed_S4_CD2AP_SH3-2.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed_S4_CD2AP_SH3-2.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed_S4_CD2AP_SH3-2.dat.plumed_master.stderr) |  
| [plumed_S3_PICALM_ANTH.dat](./data/plumed_S3_PICALM_ANTH.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed_S3_PICALM_ANTH.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed_S3_PICALM_ANTH.dat.plumed_master.stderr) |  
| [plumed_S2_BIN1_SH3.dat](./data/plumed_S2_BIN1_SH3.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed_S2_BIN1_SH3.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed_S2_BIN1_SH3.dat.plumed_master.stderr) |  
| [plumed_S1_BIN1_BAR.dat](./data/plumed_S1_BIN1_BAR.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed_S1_BIN1_BAR.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed_S1_BIN1_BAR.dat.plumed_master.stderr) |  
  
**Last tested:**  17 Jun 2026, 09:05:27
  
**Project description and instructions**  
GROMACS 2023.3 patched with PLUMED 2.9.2 (see singularity/gromacs-plumed.def in the paper repository for a reproducible build). Run with gmx_mpi mdrun -plumed `plumed_S*.dat` -ntomp 2 -npme 4 -deffnm meta. One .dat file per system; each uses 2 distance CVs and well-tempered MetaD (SIGMA=0.05 nm, HEIGHT=1.2 kJ/mol, BIASFACTOR=15, PACE=500).

  
{% raw %}
<b><a href="https://www.plumed.org/doc-master/user-doc/html/actionlist/?actions=DISTANCE,ANGLE,METAD,WHOLEMOLECULES,PRINT" target="_blank">Click here</a> to open manual pages for actions used in this project.</b>
{% endraw %}
**Submission history**  
**[v1]** 19 Apr 2026: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:26.005" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:26.005](https://www.plumed-nest.org/eggs/26/005/badge.svg)](https://www.plumed-nest.org/eggs/26/005/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/26/005/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/26/005/badge.svg" alt="plumID:26.005"&gt;&lt;/a&gt;</pre>
  </div>
</div>
