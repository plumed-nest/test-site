**Project ID:** [plumID:19.047]({{ '/' | absolute_url }}eggs/19/047/)  
**Name:**  Close Structure  
**Archive:** [ https://archive.materialscloud.org/record/file?file_id=adf64bd0-0d5c-450e-b9e2-87436c901881&record_id=133&filename=close_structure.zip](https://archive.materialscloud.org/record/file?file_id=adf64bd0-0d5c-450e-b9e2-87436c901881&record_id=133&filename=close_structure.zip)  
**Category:**  methods  
**Keywords:**  metadynamics, RMSD, path collective variables, property map  
**PLUMED version:**  2.5  
**Contributor:**  Vojtech Spiwok  
**Submitted on:** 22 May 2019  
**Last revised:** 18 Jun 2019  
**Publication:** [J. Pazúriková, A. Křenek, V. Spiwok, M. Šimková, Reducing the number of mean-square deviation calculations with floating close structure in metadynamics. The Journal of Chemical Physics. 146 (2017)](http://dx.doi.org/10.1063/1.4978296)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [cyclo/close/plumed_v2.dat](./data/cyclo/close/plumed_v2.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/cyclo/close/plumed_v2.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/cyclo/close/plumed_v2.dat.plumed_master.stderr) |  
| [cyclo/normal/plumed_v2.dat](./data/cyclo/normal/plumed_v2.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/cyclo/normal/plumed_v2.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/cyclo/normal/plumed_v2.dat.plumed_master.stderr) |  
| [trpcage/close/plumed.dat](./data/trpcage/close/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/trpcage/close/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/trpcage/close/plumed.dat.plumed_master.stderr) |  
| [trpcage/normal/plumed.dat](./data/trpcage/normal/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/trpcage/normal/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/trpcage/normal/plumed.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:52:13
  
**Project description and instructions**  
Input files (input structures, topology, PLUMED input) for simulations used to demonstrate functionality of Close Structure algorithm ([J. Chem. Phys. 2017, 146, 115101](https://doi.org/10.1063/1.4978296)). The method replaces frequent calculations of root mean square deviations in Path collective variables or Property Map collective variables. This accelerates simulations. Input files for metadynamics simulation of cyclooctane derivative in vacuum and Trp-cage in implicit solvent with two or three, respectively, Isomap CVs (with and without Close Structure). Tested with OpenMPI4.0.0, Gromacs 2018.5 and PLUMED v2.5.0. Scripts provided

  
**Submission history**  
**[v1]** 22 May 2019: original submission  
**[v2]** 17 Jun 2019: update archive  
**[v3]** 18 Jun 2019: switched to Materials Cloud  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:19.047" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:19.047](https://www.plumed-nest.org/eggs/19/047/badge.svg)](https://www.plumed-nest.org/eggs/19/047/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/19/047/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/19/047/badge.svg" alt="plumID:19.047"&gt;&lt;/a&gt;</pre>
  </div>
</div>
