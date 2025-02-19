**Project ID:** [plumID:24.036]({{ '/' | absolute_url }}eggs/24/036/)  
**Name:**  Leveraging cryptic ligand envelopes through enhanced molecular simulations  
**Archive:** [ https://github.com/fcolizzi/cryptic_envelope/archive/refs/heads/main.zip](https://github.com/fcolizzi/cryptic_envelope/archive/refs/heads/main.zip)  
**Category:**  bio  
**Keywords:**  HREX, conformational heterogeneity, drug discovery, ligand binding, plitidepsin, aplidin, ligand-target complexes, cryptic ligand envelope  
**PLUMED version:**  2.4  
**Contributor:**  Francesco Colizzi  
**Submitted on:** 14 Dec 2024  
**Publication:** unpublished  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [2r3i/plumed.dat](./data/2r3i/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/2r3i/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/2r3i/plumed.dat.plumed_master.stderr) |  
| [2vwx/plumed.dat](./data/2vwx/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/2vwx/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/2vwx/plumed.dat.plumed_master.stderr) |  
| [5dro/plumed.dat](./data/5dro/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/5dro/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/5dro/plumed.dat.plumed_master.stderr) |  
| [DIDE/plumed.dat](./data/DIDE/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/DIDE/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/DIDE/plumed.dat.plumed_master.stderr) |  
| [DIDE/plumed_water.dat](./data/DIDE/plumed_water.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/DIDE/plumed_water.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/DIDE/plumed_water.dat.plumed_master.stderr) |  
| [DIDE-water/plumed.dat](./data/DIDE-water/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/DIDE-water/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/DIDE-water/plumed.dat.plumed_master.stderr) |  
| [PLIT/plumed.dat](./data/PLIT/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/PLIT/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/PLIT/plumed.dat.plumed_master.stderr) |  
| [PLIT/plumed_h1h2.dat](./data/PLIT/plumed_h1h2.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/PLIT/plumed_h1h2.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/PLIT/plumed_h1h2.dat.plumed_master.stderr) |  
| [PLIT/plumed_water.dat](./data/PLIT/plumed_water.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/PLIT/plumed_water.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/PLIT/plumed_water.dat.plumed_master.stderr) |  
| [PLIT-CH3Cl/plumed.dat](./data/PLIT-CH3Cl/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/PLIT-CH3Cl/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/PLIT-CH3Cl/plumed.dat.plumed_master.stderr) |  
| [PLIT-water/plumed.dat](./data/PLIT-water/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/PLIT-water/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/PLIT-water/plumed.dat.plumed_master.stderr) |  
| [PLIT_A399V/plumed.dat](./data/PLIT_A399V/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/PLIT_A399V/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/PLIT_A399V/plumed.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:20:20
  
**Project description and instructions**  
Simulations have been performed with GROMACS 2018.3 and PLUMED 2.4.3. The input files for HREX simulations of several ligand-protein complexes are provided, along with PLUMED input files for the analysis of free-in-solution and target-bound conformational heterogeneity of ligands (aka the cryptic ligand envelope).

  
**Submission history**  
**[v1]** 14 Dec 2024: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:24.036" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:24.036](https://www.plumed-nest.org/eggs/24/036/badge.svg)](https://www.plumed-nest.org/eggs/24/036/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/24/036/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/24/036/badge.svg" alt="plumID:24.036"&gt;&lt;/a&gt;</pre>
  </div>
</div>
