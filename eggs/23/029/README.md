**Project ID:** [plumID:23.029]({{ '/' | absolute_url }}eggs/23/029/)  
**Name:**  An accurate and efficient SAXS/SANS implementation including solvation layer effects suitable for restrained Molecular Dynamics simulations  
**Archive:** [ https://zenodo.org/record/8192455/files/PLUMED_NEST_REPO.zip](https://zenodo.org/record/8192455/files/PLUMED_NEST_REPO.zip)  
**Category:**  bio  
**Keywords:**  SAXS, SANS, SAS, metainference, proteins, nucleic-acid  
**PLUMED version:**  2.9  
**Contributor:**  Federico Ballabio  
**Submitted on:** 04 Aug 2023  
**Publication:** [F. Ballabio, C. Paissoni, M. Bollati, M. de Rosa, R. Capelli, C. Camilloni, Accurate and Efficient SAXS/SANS Implementation Including Solvation Layer Effects Suitable for Molecular Simulations. Journal of Chemical Theory and Computation. 19, 8401–8413 (2023)](http://dx.doi.org/10.1021/acs.jctc.3c00864)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [GELSOLIN/SLC_OFF/plumed.dat](./data/GELSOLIN/SLC_OFF/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/GELSOLIN/SLC_OFF/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/GELSOLIN/SLC_OFF/plumed.dat.plumed_master.stderr) |  
| [GELSOLIN/SLC_ON/plumed.dat](./data/GELSOLIN/SLC_ON/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/GELSOLIN/SLC_ON/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/GELSOLIN/SLC_ON/plumed.dat.plumed_master.stderr) |  
| [UP1_RNA/SLC_OFF/plumed.dat](./data/UP1_RNA/SLC_OFF/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/UP1_RNA/SLC_OFF/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/UP1_RNA/SLC_OFF/plumed.dat.plumed_master.stderr) |  
| [UP1_RNA/SLC_ON/plumed.dat](./data/UP1_RNA/SLC_ON/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/UP1_RNA/SLC_ON/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/UP1_RNA/SLC_ON/plumed.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:23:14
  
**Project description and instructions**  
Included are the input files to perform a metainference calculation using SAXS data as restraints and our latest hybrid SAXS forward model. This model allows for the inclusion of a solvent layer correction term. The simulations are meant to be performed using GROMACS and multiple replicas in the case of GELSOLIN, while using a single replica in the case of UP1.
  
**Submission history**  
**[v1]** 04 Aug 2023: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:23.029" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:23.029](https://www.plumed-nest.org/eggs/23/029/badge.svg)](https://www.plumed-nest.org/eggs/23/029/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/23/029/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/23/029/badge.svg" alt="plumID:23.029"&gt;&lt;/a&gt;</pre>
  </div>
</div>
