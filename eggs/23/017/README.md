**Project ID:** [plumID:23.017]({{ '/' | absolute_url }}eggs/23/017/)  
**Name:**  How and When Does an Enzyme React? Unraveling α-Amylase Catalytic Activity with Enhanced Sampling Techniques  
**Archive:** [ https://github.com/sudipdas789/Reaction_discovery/archive/refs/heads/main.zip](https://github.com/sudipdas789/Reaction_discovery/archive/refs/heads/main.zip)  
**Category:**  bio  
**Keywords:**  enzymatic reaction discovery, reaction mechanism, catalysis, ligand-binding modes, water, alpha-amylase, sugar, QM/MM MD, OPES, OPES explore, graph CV, machine learning, Deep TDA CV, path CV  
**PLUMED version:**  2.9  
**Contributor:**  Sudip Das  
**Submitted on:** 10 May 2023  
**Publication:** [S. Das, U. Raucci, R. P. P. Neves, M. J. Ramos, M. Parrinello, How and When Does an Enzyme React? Unraveling α-Amylase Catalytic Activity with Enhanced Sampling Techniques. ACS Catalysis. 13, 8092–8098 (2023)](http://dx.doi.org/10.1021/acscatal.3c01473)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [QM-MM_MD/34atomsCV/plumed.dat](./data/QM-MM_MD/34atomsCV/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/QM-MM_MD/34atomsCV/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/QM-MM_MD/34atomsCV/plumed.dat.plumed_master.stderr) |  
| [QM-MM_MD/8atomsCV/plumed.dat](./data/QM-MM_MD/8atomsCV/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/QM-MM_MD/8atomsCV/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/QM-MM_MD/8atomsCV/plumed.dat.plumed_master.stderr) |  
| [classical_biased_MD/plumed.dat](./data/classical_biased_MD/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/classical_biased_MD/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/classical_biased_MD/plumed.dat.plumed_master.stderr) |  
| [classical_unbiased_MD/unbiasedCVs/plumed.dat](./data/classical_unbiased_MD/unbiasedCVs/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/classical_unbiased_MD/unbiasedCVs/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/classical_unbiased_MD/unbiasedCVs/plumed.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:30:10
  
**Project description and instructions**  
This egg contains the input files for replicating the reaction discovery and enhanced sampling OPES simulations for alpha-amylase enzyme with a sugar substrate using graph CV, Deep TDA CVs, and path CV. The graph CVs accelerate the exploration of the enzymatic reaction space in QM/MM discovery MD simulations with the explore version of OPES. The path CV used in OPES simulations enhances the sampling (in the Deep TDA CVs' space) of different substrate-binding modes within the enzyme's active site. For more information about Deep TDA, we refer to [plumID:21.028](https://www.plumed-nest.org/eggs/21/028/) and graph-CV to [plumID:22.004](https://www.plumed-nest.org/eggs/22/004/). The CVs were trained with Pytorch version 1.8 and the simulations were run with GROMACS 2021.5, CP2K 9.1, and PLUMED 2.9.
  
**Submission history**  
**[v1]** 10 May 2023: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:23.017" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:23.017](https://www.plumed-nest.org/eggs/23/017/badge.svg)](https://www.plumed-nest.org/eggs/23/017/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/23/017/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/23/017/badge.svg" alt="plumID:23.017"&gt;&lt;/a&gt;</pre>
  </div>
</div>
