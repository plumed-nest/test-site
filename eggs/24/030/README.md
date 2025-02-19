**Project ID:** [plumID:24.030]({{ '/' | absolute_url }}eggs/24/030/)  
**Name:**  NMR guided simulation of dsRBD  
**Archive:** [ https://github.com/debadutta-patra/dsRBD_simulation/archive/refs/heads/main.zip](https://github.com/debadutta-patra/dsRBD_simulation/archive/refs/heads/main.zip)  
**Category:**  bio  
**Keywords:**  Metainference, NMR, protein dynamics  
**PLUMED version:**  2.9  
**Contributor:**  Debadutta Patra  
**Submitted on:** 11 Nov 2024  
**Publication:** unpublished  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [drb2d1/drb2d1_plumed.dat](./data/drb2d1/drb2d1_plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/drb2d1/drb2d1_plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/drb2d1/drb2d1_plumed.dat.plumed_master.stderr) |  
| [drb2d1/plumed_distances_pp.dat](./data/drb2d1/plumed_distances_pp.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/drb2d1/plumed_distances_pp.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/drb2d1/plumed_distances_pp.dat.plumed_master.stderr) |  
| [drb3d1/drb3d1_plumed.dat](./data/drb3d1/drb3d1_plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/drb3d1/drb3d1_plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/drb3d1/drb3d1_plumed.dat.plumed_master.stderr) |  
| [drb3d1/plumed_distances_pp.dat](./data/drb3d1/plumed_distances_pp.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/drb3d1/plumed_distances_pp.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/drb3d1/plumed_distances_pp.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:20:05
  
**Project description and instructions**  
The code used is gromacs-2022.5 with PLUMED v2.9. The command line to run the simulation is `mpirun -np # gmx_mpi mdrun -deffnm metainf.tpr -multidir rep_* -plumed drb*d1_plumed.dat`

  
**Submission history**  
**[v1]** 11 Nov 2024: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:24.030" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:24.030](https://www.plumed-nest.org/eggs/24/030/badge.svg)](https://www.plumed-nest.org/eggs/24/030/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/24/030/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/24/030/badge.svg" alt="plumID:24.030"&gt;&lt;/a&gt;</pre>
  </div>
</div>
