**Project ID:** [plumID:20.026]({{ '/' | absolute_url }}eggs/20/026/)  
**Name:**  Free energy calculations of the functional selectivity of 5-HT_2B-TS G protein-coupled receptor  
**Archive:** [ https://zenodo.org/record/4085006/files/plumed-nest.zip](https://zenodo.org/record/4085006/files/plumed-nest.zip)  
**Category:**  bio  
**Keywords:**  Metadynamics, Umbrella sampling  
**PLUMED version:**  2.5  
**Contributor:**  Brandon Peters  
**Submitted on:** 05 Oct 2020  
**Last revised:** 15 Jan 2021  
**Publication:** [B. L. Peters, J. Deng, A. L. Ferguson, Free energy calculations of the functional selectivity of 5-HT2B G protein-coupled receptor. PLOS ONE. 15, e0243313 (2020)](http://dx.doi.org/10.1371/journal.pone.0243313)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [plumed.dat](./data/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed.dat.plumed_master.stderr) |  
| [plumed_WTMD.dat](./data/plumed_WTMD.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed_WTMD.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/plumed_WTMD.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:39:51
  
**Project description and instructions**  
There are the input files for well tempered metadynamics (WTMD) and umbrella sampling for 5-HT2B GPCR simulations with ligand, LSD. I run the PLUMED script as given for WTMD, "gmx grompp -f md.mdp -c lsd_final.gro -p topol.top -n index.ndx -o md_0_1_plumed.tpr" and "mpiexec mdrun_mpi -ntomp 2 -deffnm md_0_1_plumed -plumed plumed_WTMD.dat" and finally "plumed sum_hills --hills hills --outfile fes-lsd-final.dat". Then I run "python 2Dplot_contour_plumed" which gives the Free Energy Surface and the history of hills. I ran the script for restraint. "gmx grompp -f md.mdp -c lsd-final.gro -p topol.top -n index.ndx -o md_final_plumed_startnew2.tpr" and "gmx mdrun -ntmpi 1 -ntomp 16 -v -deffnm md_final_plumed_startnew2 -plumed plumed_restrain.dat". I follow [this tutorial](https://www.plumed.org/doc-v2.5/user-doc/html/belfast-4.html) closely using "create-restraint.sh". 

  
**Submission history**  
**[v1]** 05 Oct 2020: original submission  
**[v2]** 15 Jan 2021: updated doi  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:20.026" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:20.026](https://www.plumed-nest.org/eggs/20/026/badge.svg)](https://www.plumed-nest.org/eggs/20/026/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/20/026/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/20/026/badge.svg" alt="plumID:20.026"&gt;&lt;/a&gt;</pre>
  </div>
</div>
