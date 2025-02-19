**Project ID:** [plumID:24.008]({{ '/' | absolute_url }}eggs/24/008/)  
**Name:**  yCD Metadynamics  
**Archive:** [ https://github.com/mccartygroup/yCD_Metadynamics/raw/main/yCD_Metadynamics.zip](https://github.com/mccartygroup/yCD_Metadynamics/raw/main/yCD_Metadynamics.zip)  
**Category:**  bio  
**Keywords:**  volume-based MetaD, path CVs, infrequent MetaD, product release  
**PLUMED version:**  2.4  
**Contributor:**  James McCarty  
**Submitted on:** 19 Mar 2024  
**Publication:** [K. A. Croney, J. McCarty, Exploring Product Release from Yeast Cytosine Deaminase with Metadynamics. The Journal of Physical Chemistry B. 128, 3102–3112 (2024)](http://dx.doi.org/10.1021/acs.jpcb.3c07972)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [5FU/Volume_MetaD_Input/plumed_run.dat](./data/5FU/Volume_MetaD_Input/plumed_run.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/5FU/Volume_MetaD_Input/plumed_run.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/5FU/Volume_MetaD_Input/plumed_run.dat.plumed_master.stderr) |  
| [5FU/iMetaD_Input/plumed_imetad.dat](./data/5FU/iMetaD_Input/plumed_imetad.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/5FU/iMetaD_Input/plumed_imetad.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/5FU/iMetaD_Input/plumed_imetad.dat.plumed_master.stderr) |  
| [Reweighting/plumed_get_weights.dat](./data/Reweighting/plumed_get_weights.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-failed-red.svg)](data/Reweighting/plumed_get_weights.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/Reweighting/plumed_get_weights.dat.plumed_master.stderr) |  
| [Reweighting/plumed_reweight.dat](./data/Reweighting/plumed_reweight.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-failed-red.svg)](data/Reweighting/plumed_reweight.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/Reweighting/plumed_reweight.dat.plumed_master.stderr) |  
| [Uracil/Volume_MetaD_Input/plumed_run.dat](./data/Uracil/Volume_MetaD_Input/plumed_run.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/Uracil/Volume_MetaD_Input/plumed_run.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/Uracil/Volume_MetaD_Input/plumed_run.dat.plumed_master.stderr) |  
| [Uracil/iMetaD/plumed_imetad.dat](./data/Uracil/iMetaD/plumed_imetad.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/Uracil/iMetaD/plumed_imetad.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/Uracil/iMetaD/plumed_imetad.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:29:04
  
**Project description and instructions**  
All input files to simulate yCD with 5-FU bound or uracil bound are provided in the Structure folder. In the Volume_MetaD_Input is the plumed input for running volume based metadynamics. All the necessary files are in the Structure folder. In the iMetaD folder is the plumed input for running unbinding simulations used to estimate k_off from infrequent metadynamics. Plumed inputs for post-processing and reweighting are in the Reweighting directory. 

  
**Submission history**  
**[v1]** 19 Mar 2024: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:24.008" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:24.008](https://www.plumed-nest.org/eggs/24/008/badge.svg)](https://www.plumed-nest.org/eggs/24/008/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/24/008/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/24/008/badge.svg" alt="plumID:24.008"&gt;&lt;/a&gt;</pre>
  </div>
</div>
