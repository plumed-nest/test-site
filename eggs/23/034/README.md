**Project ID:** [plumID:23.034]({{ '/' | absolute_url }}eggs/23/034/)  
**Name:**  Urea nucleation in water: do long-range forces matter?  
**Archive:** [ https://github.com/connorzzou/PLUMED-NEST/raw/main/LMF-UREA-AQ.zip](https://github.com/connorzzou/PLUMED-NEST/raw/main/LMF-UREA-AQ.zip)  
**Category:**  materials  
**Keywords:**  LMF theory, Metadynamics, Nucleation  
**PLUMED version:**  2.7.2  
**Contributor:**  Ziyue Zou  
**Submitted on:** 20 Aug 2023  
**Publication:** [R. Zhao, Z. Zou, J. D. Weeks, P. Tiwary, Quantifying the Relevance of Long-Range Forces for Crystal Nucleation in Water. Journal of Chemical Theory and Computation. 19, 9093–9101 (2023)](http://dx.doi.org/10.1021/acs.jctc.3c01120)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [GT_model/plumed.dat](./data/GT_model/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/GT_model/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/GT_model/plumed.dat.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
| [SS_model/plumed.dat](./data/SS_model/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/SS_model/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/SS_model/plumed.dat.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
| [full_model/plumed.dat](./data/full_model/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/full_model/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/full_model/plumed.dat.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
  
**Last tested:**  19 Feb 2025, 14:22:27
  
**Project description and instructions**  
The three folders contain the input files for the simulations with the full model, the Gaussian-truncated model, and the short solvent model, respectively. The .intl file is the initial configuration for the urea-water system. The GT_potential.table contains tabulated Gaussian-truncated electrostatic potentials. The urea_lmf.table contains tabulated renormalized long-range electrostatic potentials in the short solvent model. The ${sys}1.in file is the input script for LAMMPS-29Sep2021, where ${sys} stands for the corresponding model, and ${sys}2.in is the input script if one needs to restart the simulation continued from ${sys}1.in.
  
**Submission history**  
**[v1]** 20 Aug 2023: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:23.034" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:23.034](https://www.plumed-nest.org/eggs/23/034/badge.svg)](https://www.plumed-nest.org/eggs/23/034/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/23/034/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/23/034/badge.svg" alt="plumID:23.034"&gt;&lt;/a&gt;</pre>
  </div>
</div>
