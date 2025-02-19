**Project ID:** [plumID:22.024]({{ '/' | absolute_url }}eggs/22/024/)  
**Name:**  Conformational Entropy as a Potential Liability of Computationally Designed Antibodies  
**Archive:** [ https://github.com/vendruscolo-lab/sdab-entropy/raw/main/plumed-nest.zip](https://github.com/vendruscolo-lab/sdab-entropy/raw/main/plumed-nest.zip)  
**Category:**  bio  
**Keywords:**  metadynamics, conformational entropy, antibody, nanobody  
**PLUMED version:**  2.6  
**Contributor:**  Thomas Löhr  
**Submitted on:** 23 May 2022  
**Publication:** [T. Löhr, P. Sormanni, M. Vendruscolo, Conformational Entropy as a Potential Liability of Computationally Designed Antibodies. Biomolecules. 12, 718 (2022)](http://dx.doi.org/10.3390/biom12050718)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [des/plumed.dat](./data/des/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/des/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/des/plumed.dat.plumed_master.stderr) |  
| [dka/plumed.dat](./data/dka/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/dka/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/dka/plumed.dat.plumed_master.stderr) |  
| [vhh/plumed.dat](./data/vhh/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/vhh/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/vhh/plumed.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:26:18
  
**Project description and instructions**  
GROMACS 2019.3, Simulations run using mpirun -n 32 gmx_mpi mdrun -s topol -cpi state -multidir r{0..31} -plumed ../plumed.dat -v

  
**Submission history**  
**[v1]** 23 May 2022: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:22.024" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:22.024](https://www.plumed-nest.org/eggs/22/024/badge.svg)](https://www.plumed-nest.org/eggs/22/024/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/22/024/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/22/024/badge.svg" alt="plumID:22.024"&gt;&lt;/a&gt;</pre>
  </div>
</div>
