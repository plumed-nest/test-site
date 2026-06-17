**Project ID:** [plumID:25.013]({{ '/' | absolute_url }}eggs/25/013/)  
**Name:**  Data-Driven Engineering of Highly Thermostable Collagen-Mimetic Peptoid Triple Helices  
**Archive:** [ https://github.com/alexberlaga/cmp_plumed_nest/archive/refs/heads/main.zip](https://github.com/alexberlaga/cmp_plumed_nest/archive/refs/heads/main.zip)  
**Category:**  bio  
**Keywords:**  umbrella sampling, temperature ramping  
**PLUMED version:**  2.9  
**Contributor:**  Alexander Berlaga  
**Submitted on:** 19 May 2025  
**Publication:** unpublished  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [annealing/plumed0.dat](./data/annealing/plumed0.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/annealing/plumed0.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/annealing/plumed0.dat.plumed_master.stderr) |  
| [umbrella/plumed.dat](./data/umbrella/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/umbrella/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/umbrella/plumed.dat.plumed_master.stderr) |  
  
**Last tested:**  17 Jun 2026, 09:09:13
  
**Project description and instructions**  
This repository has the necessary code to run annealing and umbrella simulations of collagen-mimetic peptoids. Files are organized as follows. The `Annealing` Folder contains initial structure (npt.gro) and topology files (topol.top); Code generating PLUMED files to track CVs (gen_plumed.py); molecular dynamics parameters for annealing (npt_run.mdp); Example PLUMED file (plumed0.dat); code to run the MD (anneal.sbatch and run_sim.py). The `Umbrella` Folder contains initial structure (npt.gro) and topology files (topol.top); Code generating TICA object and PLUMED files to bias CVs (make_tica_plumed.py); molecular dynamics parameters for equilibration and umbrella runs (umbrella_equil.mdp and umbrella_run.mdp, respectively); Example PLUMED file (plumed.dat); code to run the MD (run_umbrella.sbatch).

  
{% raw %}
<b><a href="https://www.plumed.org/doc-master/user-doc/html/actionlist/?actions=DISTANCE,PYTORCH_MODEL,GYRATION,PRINT,RESTRAINT" target="_blank">Click here</a> to open manual pages for actions used in this project.</b>
{% endraw %}
**Submission history**  
**[v1]** 19 May 2025: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:25.013" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:25.013](https://www.plumed-nest.org/eggs/25/013/badge.svg)](https://www.plumed-nest.org/eggs/25/013/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/25/013/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/25/013/badge.svg" alt="plumID:25.013"&gt;&lt;/a&gt;</pre>
  </div>
</div>
