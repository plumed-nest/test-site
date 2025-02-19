**Project ID:** [plumID:22.035]({{ '/' | absolute_url }}eggs/22/035/)  
**Name:**  Deciphering the alphabet of disorder — Glu and Asp act differently on local but not global properties  
**Archive:** [ https://github.com/KULL-Centre/_2022_Roesgaard-Lundsgaard_DSS1/raw/main/plumed-input.zip](https://github.com/KULL-Centre/_2022_Roesgaard-Lundsgaard_DSS1/raw/main/plumed-input.zip)  
**Category:**  bio  
**Keywords:**  intrinsically disordered proteins, parallel bias metadynamics, protein  
**PLUMED version:**  2.6.1  
**Contributor:**  Kresten Lindorff-Larsen  
**Submitted on:** 24 Sep 2022  
**Publication:** [M. A. Roesgaard, J. E. Lundsgaard, E. A. Newcombe, N. L. Jacobsen, F. Pesce, E. E. Tranchant, S. Lindemose, A. Prestel, R. Hartmann-Petersen, K. Lindorff-Larsen, B. B. Kragelund, Deciphering the Alphabet of Disorder—Glu and Asp Act Differently on Local but Not Global Properties. Biomolecules. 12, 1426 (2022)](http://dx.doi.org/10.3390/biom12101426)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [allD.dat](./data/allD.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/allD.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/allD.dat.plumed_master.stderr) |  
| [allD_helix.dat](./data/allD_helix.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/allD_helix.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/allD_helix.dat.plumed_master.stderr) |  
| [allE.dat](./data/allE.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/allE.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/allE.dat.plumed_master.stderr) |  
| [allE_helix.dat](./data/allE_helix.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/allE_helix.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/allE_helix.dat.plumed_master.stderr) |  
| [swap.dat](./data/swap.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/swap.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/swap.dat.plumed_master.stderr) |  
| [swap_helix.dat](./data/swap_helix.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/swap_helix.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/swap_helix.dat.plumed_master.stderr) |  
| [wt.dat](./data/wt.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/wt.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/wt.dat.plumed_master.stderr) |  
| [wt_helix.dat](./data/wt_helix.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/wt_helix.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/wt_helix.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:36:40
  
**Project description and instructions**  
Software used. GROMACS v. 2019.6, cuda toolkit 10.2.89, openmpi 1.10.2. Example command line.  mpirun -np 160 ${gmx} mdrun -deffnm wt_helix_prod -plumed wt_helix.dat -pin on -npme 0 -notunepme -v -maxh 0.5 -cpi -cpt 360. 

  
**Submission history**  
**[v1]** 24 Sep 2022: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:22.035" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:22.035](https://www.plumed-nest.org/eggs/22/035/badge.svg)](https://www.plumed-nest.org/eggs/22/035/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/22/035/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/22/035/badge.svg" alt="plumID:22.035"&gt;&lt;/a&gt;</pre>
  </div>
</div>
