**Project ID:** [plumID:24.020]({{ '/' | absolute_url }}eggs/24/020/)  
**Name:**  Graph Neural Network-State Predictive Information Bottleneck (GNN-SPIB) approach for learning molecular thermodynamics and kinetics  
**Archive:** [ https://github.com/connorzzou/PLUMED-NEST/raw/main/PLUMED_GNN_SPIB.zip](https://github.com/connorzzou/PLUMED-NEST/raw/main/PLUMED_GNN_SPIB.zip)  
**Category:**  bio  
**Keywords:**  LJ7, alanine, well-tempered metadynamics, infrequent metadynamics, machine learning  
**PLUMED version:**  2.8.1  
**Contributor:**  Ziyue Zou, Dedi Wang, Pratyush Tiwary  
**Submitted on:** 22 Sep 2024  
**Publication:** [Ziyue Zou, Dedi Wang, Pratyush Tiwary. Graph Neural Network-State Predictive Information Bottleneck (GNN-SPIB) approach for learning molecular thermodynamics and kinetics](https://arxiv.org/abs/2409.11843)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [ala2/imetad/plumed_phi_10000.dat](./data/ala2/imetad/plumed_phi_10000.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/ala2/imetad/plumed_phi_10000.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/ala2/imetad/plumed_phi_10000.dat.plumed_master.stderr) |  
| [ala2/imetad/plumed_phi_2000.dat](./data/ala2/imetad/plumed_phi_2000.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/ala2/imetad/plumed_phi_2000.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/ala2/imetad/plumed_phi_2000.dat.plumed_master.stderr) |  
| [ala2/imetad/plumed_phi_50000.dat](./data/ala2/imetad/plumed_phi_50000.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/ala2/imetad/plumed_phi_50000.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/ala2/imetad/plumed_phi_50000.dat.plumed_master.stderr) |  
| [ala2/imetad/plumed_psi_10000.dat](./data/ala2/imetad/plumed_psi_10000.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/ala2/imetad/plumed_psi_10000.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/ala2/imetad/plumed_psi_10000.dat.plumed_master.stderr) |  
| [ala2/imetad/plumed_psi_2000.dat](./data/ala2/imetad/plumed_psi_2000.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/ala2/imetad/plumed_psi_2000.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/ala2/imetad/plumed_psi_2000.dat.plumed_master.stderr) |  
| [ala2/imetad/plumed_psi_50000.dat](./data/ala2/imetad/plumed_psi_50000.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/ala2/imetad/plumed_psi_50000.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/ala2/imetad/plumed_psi_50000.dat.plumed_master.stderr) |  
| [ala2/imetad/plumed_z1z2_10000.dat](./data/ala2/imetad/plumed_z1z2_10000.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-failed-red.svg)](data/ala2/imetad/plumed_z1z2_10000.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/ala2/imetad/plumed_z1z2_10000.dat.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
| [ala2/imetad/plumed_z1z2_2000.dat](./data/ala2/imetad/plumed_z1z2_2000.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-failed-red.svg)](data/ala2/imetad/plumed_z1z2_2000.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/ala2/imetad/plumed_z1z2_2000.dat.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
| [ala2/imetad/plumed_z1z2_50000.dat](./data/ala2/imetad/plumed_z1z2_50000.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-failed-red.svg)](data/ala2/imetad/plumed_z1z2_50000.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/ala2/imetad/plumed_z1z2_50000.dat.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
| [ala2/wtmetad/plumed_ang.dat](./data/ala2/wtmetad/plumed_ang.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/ala2/wtmetad/plumed_ang.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/ala2/wtmetad/plumed_ang.dat.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
| [ala2/wtmetad/plumed_gnn.dat](./data/ala2/wtmetad/plumed_gnn.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-failed-red.svg)](data/ala2/wtmetad/plumed_gnn.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/ala2/wtmetad/plumed_gnn.dat.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
| [ala3/imetad/plumed_phi_1000.dat](./data/ala3/imetad/plumed_phi_1000.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/ala3/imetad/plumed_phi_1000.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/ala3/imetad/plumed_phi_1000.dat.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
| [ala3/imetad/plumed_phi_200.dat](./data/ala3/imetad/plumed_phi_200.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/ala3/imetad/plumed_phi_200.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/ala3/imetad/plumed_phi_200.dat.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
| [ala3/imetad/plumed_phi_5000.dat](./data/ala3/imetad/plumed_phi_5000.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/ala3/imetad/plumed_phi_5000.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/ala3/imetad/plumed_phi_5000.dat.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
| [ala3/imetad/plumed_psi_1000.dat](./data/ala3/imetad/plumed_psi_1000.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/ala3/imetad/plumed_psi_1000.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/ala3/imetad/plumed_psi_1000.dat.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
| [ala3/imetad/plumed_psi_200.dat](./data/ala3/imetad/plumed_psi_200.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/ala3/imetad/plumed_psi_200.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/ala3/imetad/plumed_psi_200.dat.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
| [ala3/imetad/plumed_psi_5000.dat](./data/ala3/imetad/plumed_psi_5000.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/ala3/imetad/plumed_psi_5000.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/ala3/imetad/plumed_psi_5000.dat.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
| [ala3/imetad/plumed_z1z2_1000.dat](./data/ala3/imetad/plumed_z1z2_1000.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-failed-red.svg)](data/ala3/imetad/plumed_z1z2_1000.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/ala3/imetad/plumed_z1z2_1000.dat.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
| [ala3/imetad/plumed_z1z2_200.dat](./data/ala3/imetad/plumed_z1z2_200.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-failed-red.svg)](data/ala3/imetad/plumed_z1z2_200.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/ala3/imetad/plumed_z1z2_200.dat.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
| [ala3/imetad/plumed_z1z2_5000.dat](./data/ala3/imetad/plumed_z1z2_5000.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-failed-red.svg)](data/ala3/imetad/plumed_z1z2_5000.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/ala3/imetad/plumed_z1z2_5000.dat.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
  
**Last tested:**  19 Feb 2025, 14:22:35
  
**Project description and instructions**  
Software used was PLUMED-2.8.1 with PYTORCH module, GROMACS 2021.6 (alanine tetrapeptide), and GROMACS 2019.6 (alanine dipeptide)

  
**Submission history**  
**[v1]** 22 Sep 2024: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:24.020" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:24.020](https://www.plumed-nest.org/eggs/24/020/badge.svg)](https://www.plumed-nest.org/eggs/24/020/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/24/020/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/24/020/badge.svg" alt="plumID:24.020"&gt;&lt;/a&gt;</pre>
  </div>
</div>
