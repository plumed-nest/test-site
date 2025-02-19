**Project ID:** [plumID:22.004]({{ '/' | absolute_url }}eggs/22/004/)  
**Name:**  Discover, Sample and Refine. Exploring Chemistry with Enhanced Sampling Techniques  
**Archive:** [ https://github.com/uraucci/discovery_CVs/archive/master.zip](https://github.com/uraucci/discovery_CVs/archive/master.zip) [(browse)](https://github.com/uraucci/discovery_CVs/tree/master)  
**Category:**  chemistry  
**Keywords:**  reaction discovery, OPES, collective variables  
**PLUMED version:**  2.8  
**Contributor:**  Umberto Raucci  
**Submitted on:** 31 Jan 2022  
**Publication:** [U. Raucci, V. Rizzi, M. Parrinello, Discover, Sample, and Refine: Exploring Chemistry with Enhanced Sampling Techniques. The Journal of Physical Chemistry Letters. 13, 1424–1430 (2022)](http://dx.doi.org/10.1021/acs.jpclett.1c03993)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [input_files/Aldol_reaction/1_Discovery/plumed.dat](./data/input_files/Aldol_reaction/1_Discovery/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/input_files/Aldol_reaction/1_Discovery/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/input_files/Aldol_reaction/1_Discovery/plumed.dat.plumed_master.stderr) |  
| [input_files/Aldol_reaction/2_Sampling/plumed.dat](./data/input_files/Aldol_reaction/2_Sampling/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-failed-red.svg)](data/input_files/Aldol_reaction/2_Sampling/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/input_files/Aldol_reaction/2_Sampling/plumed.dat.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
| [...nput_files/Claisen_reaction/1_Discovery/plumed.dat](./data/input_files/Claisen_reaction/1_Discovery/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/input_files/Claisen_reaction/1_Discovery/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/input_files/Claisen_reaction/1_Discovery/plumed.dat.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
| [input_files/Claisen_reaction/2_Sampling/plumed.dat](./data/input_files/Claisen_reaction/2_Sampling/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/input_files/Claisen_reaction/2_Sampling/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/input_files/Claisen_reaction/2_Sampling/plumed.dat.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
  
**Last tested:**  19 Feb 2025, 14:44:35
  
**Project description and instructions**  
Molecular dynamics simulations have been carried out using the CP2K 8.1 software package patched with a development version of PLUMED 2.8. Collective variables have been computed using the Pytorch library. To import the model from Pytorch to PLUMED we have used the interface developed by Luigi Bonati. This is developed in the Python C++ API Libtorch and is available [here](https://github.com/luigibonati/datadriven-CVs/).

  
**Submission history**  
**[v1]** 31 Jan 2022: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:22.004" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:22.004](https://www.plumed-nest.org/eggs/22/004/badge.svg)](https://www.plumed-nest.org/eggs/22/004/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/22/004/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/22/004/badge.svg" alt="plumID:22.004"&gt;&lt;/a&gt;</pre>
  </div>
</div>
