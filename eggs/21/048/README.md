**Project ID:** [plumID:21.048]({{ '/' | absolute_url }}eggs/21/048/)  
**Name:**  Enhancing ligand exploration within a channel pore and fenestrations using metadynamics  
**Archive:** [ https://github.com/etaoster/etaoster.github.io/raw/main/fenestration_project/plumed_wtmetad.zip](https://github.com/etaoster/etaoster.github.io/raw/main/fenestration_project/plumed_wtmetad.zip)  
**Category:**  bio  
**Keywords:**  well-tempered metadynamics, protein-ligand enhanced sampling, sodium channel, Nav, small molecule drug  
**PLUMED version:**  2.5  
**Contributor:**  Elaine Tao  
**Submitted on:** 30 Nov 2021  
**Last revised:** 25 Jan 2022  
**Publication:** [E. Tao, B. Corry, Characterizing fenestration size in sodium channel subtypes and their accessibility to inhibitors. Biophysical Journal. 121, 193–206 (2022)](http://dx.doi.org/10.1016/j.bpj.2021.12.025)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [plumed0.dat](./data/plumed0.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed0.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed0.dat.plumed_master.stderr) |  
| [plumed1.dat](./data/plumed1.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed1.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed1.dat.plumed_master.stderr) |  
| [plumed2.dat](./data/plumed2.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed2.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed2.dat.plumed_master.stderr) |  
| [plumed3.dat](./data/plumed3.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed3.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed3.dat.plumed_master.stderr) |  
| [plumed4.dat](./data/plumed4.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed4.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed4.dat.plumed_master.stderr) |  
| [plumed5.dat](./data/plumed5.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed5.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed5.dat.plumed_master.stderr) |  
| [plumed6.dat](./data/plumed6.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed6.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed6.dat.plumed_master.stderr) |  
| [plumed7.dat](./data/plumed7.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed7.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed7.dat.plumed_master.stderr) |  
| [plumed8.dat](./data/plumed8.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed8.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed8.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:40:36
  
**Project description and instructions**  
Files are for running nine different walkers using AMBER/20 patched with PLUMED/2.5.0 on separate GPUs. Metadynamics potential is applied to the ligand (center of mass) position relative to the protein defined by three collective variables (z, r and theta).

  
**Submission history**  
**[v1]** 30 Nov 2021: original submission  
**[v2]** 25 Jan 2022: updated doi  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:21.048" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:21.048](https://www.plumed-nest.org/eggs/21/048/badge.svg)](https://www.plumed-nest.org/eggs/21/048/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/21/048/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/21/048/badge.svg" alt="plumID:21.048"&gt;&lt;/a&gt;</pre>
  </div>
</div>
