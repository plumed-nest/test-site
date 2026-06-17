**Project ID:** [plumID:25.018]({{ '/' | absolute_url }}eggs/25/018/)  
**Name:**  Metainference simulation for dimerization of RNA binding protein  
**Archive:** [ https://github.com/debadutta-patra/dsRBD_dimerization_plumed/archive/refs/heads/main.zip](https://github.com/debadutta-patra/dsRBD_dimerization_plumed/archive/refs/heads/main.zip)  
**Category:**  bio  
**Keywords:**  Metainference, Metadynamics, SAXS, protein dimer  
**PLUMED version:**  2.9  
**Contributor:**  Debadutta Patra  
**Submitted on:** 21 Jun 2025  
**Publication:** unpublished  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [./dsRBD_dimer/plumed.dat](./data/./dsRBD_dimer/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/./dsRBD_dimer/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/./dsRBD_dimer/plumed.dat.plumed_master.stderr) |  
  
**Last tested:**  17 Jun 2026, 09:08:04
  
**Project description and instructions**  
The code used is gromacs-2022.5 with PLUMED v2.9. The command line to run the simulation is `mpirun -np # gmx_mpi mdrun -deffnm topol.tpr -multidir rep_* -plumed plumed.dat`. 

  
{% raw %}
<b><a href="https://www.plumed.org/doc-master/user-doc/html/actionlist/?actions=MOLINFO,TORSION,PRINT,UPPER_WALLS,SAXS,ENSEMBLE,CENTER,METAINFERENCE,FLUSH,PBMETAD,DISTANCE,STATS,GYRATION,WHOLEMOLECULES" target="_blank">Click here</a> to open manual pages for actions used in this project.</b>
{% endraw %}
**Submission history**  
**[v1]** 21 Jun 2025: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:25.018" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:25.018](https://www.plumed-nest.org/eggs/25/018/badge.svg)](https://www.plumed-nest.org/eggs/25/018/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/25/018/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/25/018/badge.svg" alt="plumID:25.018"&gt;&lt;/a&gt;</pre>
  </div>
</div>
