**Project ID:** [plumID:25.006]({{ '/' | absolute_url }}eggs/25/006/)  
**Name:**  Characterizing the conformational ensemble of PROTAC degraders in solutions via atomistic simulations  
**Archive:** [ https://zenodo.org/records/16416165/files/PROTACs_PBMetaD_PLUMED-NEST.zip](https://zenodo.org/records/16416165/files/PROTACs_PBMetaD_PLUMED-NEST.zip)  
**Category:**  methods  
**Keywords:**  Enhanced sampling, Atomistic simulations, Conformational ensemble, PROTACs, Targeted Protein Degradation, Chamelonic molecules  
**PLUMED version:**  2.8.2  
**Contributor:**  Shikshya Bhusal, Omar Valsson  
**Submitted on:** 11 Feb 2025  
**Publication:** [S. Bhusal, O. Valsson, Characterizing the conformational ensemble of PROTAC degraders in solutions via atomistic simulations. doi: 10.26434/chemrxiv-2025-bxf47 (2025)](http://dx.doi.org/10.26434/chemrxiv-2025-bxf47)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [...imum_conformation_extraction/plumed-dumpframes.dat](./data/Input_Files/Minimum_conformation_extraction/plumed-dumpframes.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/Input_Files/Minimum_conformation_extraction/plumed-dumpframes.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/Input_Files/Minimum_conformation_extraction/plumed-dumpframes.dat.plumed_master.stderr) |  
| [.../LastBiasReweighting_5microsec/plumed_lastbias.dat](./data/Input_Files/Reweighting-Example/LastBiasReweighting_5microsec/plumed_lastbias.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/Input_Files/Reweighting-Example/LastBiasReweighting_5microsec/plumed_lastbias.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/Input_Files/Reweighting-Example/LastBiasReweighting_5microsec/plumed_lastbias.dat.plumed_master.stderr) |  
| [...mple/LastBiasReweighting_5microsec/plumed_read.dat](./data/Input_Files/Reweighting-Example/LastBiasReweighting_5microsec/plumed_read.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/Input_Files/Reweighting-Example/LastBiasReweighting_5microsec/plumed_read.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/Input_Files/Reweighting-Example/LastBiasReweighting_5microsec/plumed_read.dat.plumed_master.stderr) |  
| [Input_Files/plumed_pbmetad.dat](./data/Input_Files/plumed_pbmetad.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/Input_Files/plumed_pbmetad.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/Input_Files/plumed_pbmetad.dat.plumed_master.stderr) |  
  
**Last tested:**  17 Jun 2026, 09:10:13
  
**Project description and instructions**  
Files were run with GROMACS 2022.5, PLUMED 2.8.2, and VMD 1.9.3 for trajectory analysis. 

  
{% raw %}
<b><a href="https://www.plumed.org/doc-master/user-doc/html/actionlist/?actions=PRINT,MOLINFO,DUMPATOMS,ENERGY,TORSION,INCLUDE,PBMETAD,GYRATION,DISTANCE,CENTER,RESTART,VOLUME,UPDATE_IF,READ,WHOLEMOLECULES" target="_blank">Click here</a> to open manual pages for actions used in this project.</b>
{% endraw %}
**Submission history**  
**[v1]** 11 Feb 2025: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:25.006" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:25.006](https://www.plumed-nest.org/eggs/25/006/badge.svg)](https://www.plumed-nest.org/eggs/25/006/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/25/006/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/25/006/badge.svg" alt="plumID:25.006"&gt;&lt;/a&gt;</pre>
  </div>
</div>
