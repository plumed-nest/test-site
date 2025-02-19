**Project ID:** [plumID:23.002]({{ '/' | absolute_url }}eggs/23/002/)  
**Name:**  Critical comparison of general-purpose collective variables for crystal nucleation  
**Archive:** [ https://github.com/julienlamcnrs/2023_PhysRevE_PIVvsS/archive/refs/heads/main.zip](https://github.com/julienlamcnrs/2023_PhysRevE_PIVvsS/archive/refs/heads/main.zip)  
**Category:**  methods  
**Keywords:**  metadynamics, umbrella sampling, commitor, entropy, PIV  
**PLUMED version:**  2.5.1  
**Contributor:**  Julien Lam  
**Submitted on:** 20 Jan 2023  
**Publication:** [J. Lam, F. Pietrucci, Critical comparison of general-purpose collective variables for crystal nucleation. Physical Review E. 107 (2023)](http://dx.doi.org/10.1103/PhysRevE.107.L012601)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [1_Metadynamics/1_PIV/plumed.dat](./data/1_Metadynamics/1_PIV/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-failed-red.svg)](data/1_Metadynamics/1_PIV/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/1_Metadynamics/1_PIV/plumed.dat.plumed_master.stderr) |  
| [1_Metadynamics/2_Entropy/plumed.dat](./data/1_Metadynamics/2_Entropy/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-failed-red.svg)](data/1_Metadynamics/2_Entropy/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/1_Metadynamics/2_Entropy/plumed.dat.plumed_master.stderr) |  
| [1_Metadynamics/3_BAD_PIV/plumed.dat](./data/1_Metadynamics/3_BAD_PIV/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-failed-red.svg)](data/1_Metadynamics/3_BAD_PIV/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/1_Metadynamics/3_BAD_PIV/plumed.dat.plumed_master.stderr) |  
| [1_Metadynamics/4_Q6/plumed.dat](./data/1_Metadynamics/4_Q6/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-failed-red.svg)](data/1_Metadynamics/4_Q6/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/1_Metadynamics/4_Q6/plumed.dat.plumed_master.stderr) |  
| [2_Commitor/plumed.dat](./data/2_Commitor/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-failed-red.svg)](data/2_Commitor/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/2_Commitor/plumed.dat.plumed_master.stderr) |  
| [3_UmbrellaSampling/1_PIV/zSrc/plumed.dat](./data/3_UmbrellaSampling/1_PIV/zSrc/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-failed-red.svg)](data/3_UmbrellaSampling/1_PIV/zSrc/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/3_UmbrellaSampling/1_PIV/zSrc/plumed.dat.plumed_master.stderr) |  
| [3_UmbrellaSampling/2_Entropy/zSrc/plumed.dat](./data/3_UmbrellaSampling/2_Entropy/zSrc/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-failed-red.svg)](data/3_UmbrellaSampling/2_Entropy/zSrc/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/3_UmbrellaSampling/2_Entropy/zSrc/plumed.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:31:01
  
**Project description and instructions**  
The GitHub repository includes 3 folders that stand for each type of simulations, Metadynamics, Commitor UmbrellaSampling. Except for Commitor that does not require biasing, the other are split in 3 folders depending on which CV is employed for biasing.

  
**Submission history**  
**[v1]** 20 Jan 2023: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:23.002" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:23.002](https://www.plumed-nest.org/eggs/23/002/badge.svg)](https://www.plumed-nest.org/eggs/23/002/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/23/002/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/23/002/badge.svg" alt="plumID:23.002"&gt;&lt;/a&gt;</pre>
  </div>
</div>
