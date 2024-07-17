**Project ID:** [plumID:24.014]({{ '/' | absolute_url }}eggs/24/014/)  
**Name:**  Learning Collective Variables with Synthetic Data Augmentation through Physics-inspired Geodesic Interpolation  
**Archive:** [ https://github.com/learningmatter-mit/geodesic-interpolation-cv/archive/refs/tags/v0.1.0.zip](https://github.com/learningmatter-mit/geodesic-interpolation-cv/archive/refs/tags/v0.1.0.zip)  
**Category:**  methods  
**Keywords:**  data augmentation, geodesic interpolation, collective variables, protein folding  
**PLUMED version:**  2.9  
**Contributor:**  Juno Nam  
**Submitted on:** 16 Jun 2024  
**Publication:** [S. Yang, J. Nam, J. C. B. Dietschreit, R. Gómez-Bombarelli. Learning Collective Variables with Synthetic Data Augmentation through Physics-inspired Geodesic Interpolation](https://arxiv.org/abs/2402.01542)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [...ns/enhanced/plumed_files/plumed_Reg_geo_filter.dat](./data/simulations/enhanced/plumed_files/plumed_Reg_geo_filter.dat.md) |  [![tested on v2.9](https://img.shields.io/badge/v2.9-passing-green.svg)](data/simulations/enhanced/plumed_files/plumed_Reg_geo_filter.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/simulations/enhanced/plumed_files/plumed_Reg_geo_filter.dat.plumed_master.stderr) |  
| [.../enhanced/plumed_files/plumed_Reg_geo_nofilter.dat](./data/simulations/enhanced/plumed_files/plumed_Reg_geo_nofilter.dat.md) |  [![tested on v2.9](https://img.shields.io/badge/v2.9-passing-green.svg)](data/simulations/enhanced/plumed_files/plumed_Reg_geo_nofilter.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/simulations/enhanced/plumed_files/plumed_Reg_geo_nofilter.dat.plumed_master.stderr) |  
| [simulations/enhanced/plumed_files/plumed_TDA.dat](./data/simulations/enhanced/plumed_files/plumed_TDA.dat.md) |  [![tested on v2.9](https://img.shields.io/badge/v2.9-passing-green.svg)](data/simulations/enhanced/plumed_files/plumed_TDA.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/simulations/enhanced/plumed_files/plumed_TDA.dat.plumed_master.stderr) |  
| [...ns/enhanced/plumed_files/plumed_TDA_geo_filter.dat](./data/simulations/enhanced/plumed_files/plumed_TDA_geo_filter.dat.md) |  [![tested on v2.9](https://img.shields.io/badge/v2.9-passing-green.svg)](data/simulations/enhanced/plumed_files/plumed_TDA_geo_filter.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/simulations/enhanced/plumed_files/plumed_TDA_geo_filter.dat.plumed_master.stderr) |  
| [.../enhanced/plumed_files/plumed_TDA_geo_nofilter.dat](./data/simulations/enhanced/plumed_files/plumed_TDA_geo_nofilter.dat.md) |  [![tested on v2.9](https://img.shields.io/badge/v2.9-passing-green.svg)](data/simulations/enhanced/plumed_files/plumed_TDA_geo_nofilter.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/simulations/enhanced/plumed_files/plumed_TDA_geo_nofilter.dat.plumed_master.stderr) |  
| [simulations/unbiased/folded/plumed.dat](./data/simulations/unbiased/folded/plumed.dat.md) |  [![tested on v2.9](https://img.shields.io/badge/v2.9-passing-green.svg)](data/simulations/unbiased/folded/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/simulations/unbiased/folded/plumed.dat.plumed_master.stderr) |  
| [simulations/unbiased/unfolded/plumed.dat](./data/simulations/unbiased/unfolded/plumed.dat.md) |  [![tested on v2.9](https://img.shields.io/badge/v2.9-passing-green.svg)](data/simulations/unbiased/unfolded/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/simulations/unbiased/unfolded/plumed.dat.plumed_master.stderr) |  
  
**Last tested:**  17 Jul 2024, 20:18:06
  
**Project description and instructions**  
To deploy the learned CV in MD simulations, you need to build the PLUMED package with the pytorch and drr modules, and then build the GROMACS package with the PLUMED patch. We tested our code with PLUMED 2.9.0 with libtorch 2.0.1 and GROMACS 2023. 

  
**Submission history**  
**[v1]** 16 Jun 2024: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:24.014" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:24.014](https://www.plumed-nest.org/eggs/24/014/badge.svg)](https://www.plumed-nest.org/eggs/24/014/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/24/014/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/24/014/badge.svg" alt="plumID:24.014"&gt;&lt;/a&gt;</pre>
  </div>
</div>
