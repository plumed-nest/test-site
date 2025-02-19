**Project ID:** [plumID:20.017]({{ '/' | absolute_url }}eggs/20/017/)  
**Name:**  FISST  
**Archive:** [ https://github.com/hocky-research-group/plumed-nest-eggs/raw/master/fisst-plumed-nest.zip](https://github.com/hocky-research-group/plumed-nest-eggs/raw/master/fisst-plumed-nest.zip)  
**Category:**  methods  
**Keywords:**  FISST, force, peptide, sampling, tempering  
**PLUMED version:**  2.7  
**Contributor:**  Glen Hocky  
**Submitted on:** 04 Jun 2020  
**Last revised:** 30 Jun 2020  
**Publication:** [M. J. Hartmann, Y. Singh, E. Vanden-Eijnden, G. M. Hocky, Infinite switch simulated tempering in force (FISST). The Journal of Chemical Physics. 152 (2020)](http://dx.doi.org/10.1063/5.0009280)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [ala10/ala10.plumed.dat](./data/ala10/ala10.plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/ala10/ala10.plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/ala10/ala10.plumed.dat.plumed_master.stderr) |  
| [..._fisst_fmin-2.0_fmax8.0_eps7.5_10000000.plumed.dat](./data/beaded-helix/helix_fisst_fmin-2.0_fmax8.0_eps7.5_10000000.plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/beaded-helix/helix_fisst_fmin-2.0_fmax8.0_eps7.5_10000000.plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/beaded-helix/helix_fisst_fmin-2.0_fmax8.0_eps7.5_10000000.plumed.dat.plumed_master.stderr) |  
| [...ed-helix/helix_sf_f-4.5_eps7.5_10000000.plumed.dat](./data/beaded-helix/helix_sf_f-4.5_eps7.5_10000000.plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/beaded-helix/helix_sf_f-4.5_eps7.5_10000000.plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/beaded-helix/helix_sf_f-4.5_eps7.5_10000000.plumed.dat.plumed_master.stderr) |  
| [v-shape-potential/v-shape.plumed.dat](./data/v-shape-potential/v-shape.plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/v-shape-potential/v-shape.plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/v-shape-potential/v-shape.plumed.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:46:59
  
**Project description and instructions**  
This file contains three examples. 1) An analytical 'v-shaped' potential, which is run with FISST using the PLUMED driver. It also contains a python script to analyze the results. 2) A toy helix model to run in LAMMPS (any version with PLUMED). This has an example of FISST and pulling with a single applied force on the ends. 3) FISST applied to ends of Alanine-10, to run in GROMACS (tested in 2018.6)  Each has a run_example.sh script that shows how to perform one representative simulation from the paper. More info [here](https://arxiv.org/abs/1910.14064).

  
**Submission history**  
**[v1]** 04 Jun 2020: original submission  
**[v2]** 30 Jun 2020: updated doi  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:20.017" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:20.017](https://www.plumed-nest.org/eggs/20/017/badge.svg)](https://www.plumed-nest.org/eggs/20/017/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/20/017/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/20/017/badge.svg" alt="plumID:20.017"&gt;&lt;/a&gt;</pre>
  </div>
</div>
