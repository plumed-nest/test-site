**Project ID:** [plumID:22.017]({{ '/' | absolute_url }}eggs/22/017/)  
**Name:**  Water regulates the residence time of Benzamidine in Trypsin  
**Archive:** [ https://github.com/narjesansari/LigandBinding_Trypsin_FES_RATE/archive/refs/heads/main.zip](https://github.com/narjesansari/LigandBinding_Trypsin_FES_RATE/archive/refs/heads/main.zip)  
**Category:**  bio  
**Keywords:**  ligand binding, water, opes, benzamidine trypsin, unbinding rates, machine learning, Deep-LDA, Deep-TICA  
**PLUMED version:**  2.8  
**Contributor:**  Narjes Ansari  
**Submitted on:** 11 Apr 2022  
**Publication:** [N. Ansari, V. Rizzi, M. Parrinello, Water regulates the residence time of Benzamidine in Trypsin. Nature Communications. 13 (2022)](http://dx.doi.org/10.1038/s41467-022-33104-3)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [FES/plumed.dat](./data/FES/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-failed-red.svg)](data/FES/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/FES/plumed.dat.plumed_master.stderr) |  
| [RATE/plumed.dat](./data/RATE/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-failed-red.svg)](data/RATE/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/RATE/plumed.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:41:48
  
**Project description and instructions**  
This egg contains the input files for replicating Trypsin-Benzamidine ligand binding simulations with Deep-LDA and Deep-TICA CVs. These CVs accelerate water throughout the binding/unbinding events. For more information about Deep-LDA, we refer to [plumID:20.004](https://www.plumed-nest.org/eggs/22/004/) and about Deep-TICA to [plumID:21.039](https://www.plumed-nest.org/eggs/21/039/). The CVs were trained with Pytorch version 1.4 and the simulations were run with Gromacs 2020.4. 

  
**Submission history**  
**[v1]** 11 Apr 2022: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:22.017" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:22.017](https://www.plumed-nest.org/eggs/22/017/badge.svg)](https://www.plumed-nest.org/eggs/22/017/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/22/017/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/22/017/badge.svg" alt="plumID:22.017"&gt;&lt;/a&gt;</pre>
  </div>
</div>
