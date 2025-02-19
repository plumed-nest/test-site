**Project ID:** [plumID:21.014]({{ '/' | absolute_url }}eggs/21/014/)  
**Name:**  how to determine statistically accurate conformational ensembles  
**Archive:** [ https://zenodo.org/records/10880520/files/PLUMED-NEST_chignolin.zip](https://zenodo.org/records/10880520/files/PLUMED-NEST_chignolin.zip)  
**Category:**  bio  
**Keywords:**  metadynamics, metainference, errors, cv, SAXS, ensemble determination  
**PLUMED version:**  2.7  
**Contributor:**  Cristina Paissoni  
**Submitted on:** 09 Apr 2021  
**Last revised:** 26 Mar 2024  
**Publication:** [C. Paissoni, C. Camilloni, How to Determine Accurate Conformational Ensembles by Metadynamics Metainference: A Chignolin Study Case. Frontiers in Molecular Biosciences. 8 (2021)](http://dx.doi.org/10.3389/fmolb.2021.694130)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [...-NEST_chignolin/Part1_MetaD_PBMetaD/plumed_ME2.dat](./data/PLUMED-NEST_chignolin/Part1_MetaD_PBMetaD/plumed_ME2.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/PLUMED-NEST_chignolin/Part1_MetaD_PBMetaD/plumed_ME2.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/PLUMED-NEST_chignolin/Part1_MetaD_PBMetaD/plumed_ME2.dat.plumed_master.stderr) |  
| [...-NEST_chignolin/Part1_MetaD_PBMetaD/plumed_PB4.dat](./data/PLUMED-NEST_chignolin/Part1_MetaD_PBMetaD/plumed_PB4.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/PLUMED-NEST_chignolin/Part1_MetaD_PBMetaD/plumed_PB4.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/PLUMED-NEST_chignolin/Part1_MetaD_PBMetaD/plumed_PB4.dat.plumed_master.stderr) |  
| [...NEST_chignolin/Part1_MetaD_PBMetaD/plumed_PB20.dat](./data/PLUMED-NEST_chignolin/Part1_MetaD_PBMetaD/plumed_PB20.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/PLUMED-NEST_chignolin/Part1_MetaD_PBMetaD/plumed_PB20.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/PLUMED-NEST_chignolin/Part1_MetaD_PBMetaD/plumed_PB20.dat.plumed_master.stderr) |  
| [...LUMED-NEST_chignolin/Part2_MM/plumed_PB4_prior.dat](./data/PLUMED-NEST_chignolin/Part2_MM/plumed_PB4_prior.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/PLUMED-NEST_chignolin/Part2_MM/plumed_PB4_prior.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/PLUMED-NEST_chignolin/Part2_MM/plumed_PB4_prior.dat.plumed_master.stderr) |  
| [PLUMED-NEST_chignolin/Part2_MM/plumed_ME2_MM.dat](./data/PLUMED-NEST_chignolin/Part2_MM/plumed_ME2_MM.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/PLUMED-NEST_chignolin/Part2_MM/plumed_ME2_MM.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/PLUMED-NEST_chignolin/Part2_MM/plumed_ME2_MM.dat.plumed_master.stderr) |  
| [PLUMED-NEST_chignolin/Part2_MM/plumed_PB4_MM.dat](./data/PLUMED-NEST_chignolin/Part2_MM/plumed_PB4_MM.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/PLUMED-NEST_chignolin/Part2_MM/plumed_PB4_MM.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/PLUMED-NEST_chignolin/Part2_MM/plumed_PB4_MM.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:35:54
  
**Project description and instructions**  
These are multiple walker metadynamics and PBMetaD simulation, some coupled with Metainference. The system simulated is chignolin and the experimental data are synthetic. Simulations can be run using GROMACS 2020.x and PLUMED-ISDB. This uses multiple replica simulations i.e. -multidir  

  
**Submission history**  
**[v1]** 09 Apr 2021: original submission  
**[v2]** 26 Mar 2024: fix to keep input working with recent plumed  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:21.014" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:21.014](https://www.plumed-nest.org/eggs/21/014/badge.svg)](https://www.plumed-nest.org/eggs/21/014/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/21/014/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/21/014/badge.svg" alt="plumID:21.014"&gt;&lt;/a&gt;</pre>
  </div>
</div>
