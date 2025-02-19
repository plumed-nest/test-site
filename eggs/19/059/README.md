**Project ID:** [plumID:19.059]({{ '/' | absolute_url }}eggs/19/059/)  
**Name:**  cis-trans isomerization of the Ac-Ala-Ala-Pro-Ala-Lys-NH2 peptide  
**Archive:** [ https://github.com/fabsugar/plumed-nest-files/raw/master/AAPAK_input.zip](https://github.com/fabsugar/plumed-nest-files/raw/master/AAPAK_input.zip)  
**Category:**  bio  
**Keywords:**  bias-exchange metadynamics, cis-trans isomerization  
**PLUMED version:**  2.2.3  
**Contributor:**  Fabrizio Marinelli  
**Submitted on:** 19 Jul 2019  
**Publication:** unpublished  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [plumed.0.dat](./data/plumed.0.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed.0.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed.0.dat.plumed_master.stderr) |  
| [plumed.1.dat](./data/plumed.1.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed.1.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed.1.dat.plumed_master.stderr) |  
| [plumed_be-common.dat](./data/plumed_be-common.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed_be-common.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed_be-common.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:45:45
  
**Project description and instructions**  
The deposited files contain the necessary input to run bias-exchange metadynamics simulations to investigate the cis-trans isomerization of the Ac-Ala-Ala-Pro-Ala-Lys-NH2 peptide using two replicas, each one using a specific torsion angle as collective variable. The simulations were performed using GROMACS VERSION 5.0.2 and PLUMED VERSION 2.2.3.  The simulations can be run for example using the command  "mpirun -np 4 gmx_mpi mdrun -deffnm metad-be -plumed plumed -multi 2 -replex 2000 > & meta-be.out &". Newer versions of GROMACS are able to read the .tpr files and run the simulations as well as newer versions of PLUMED. 

  
**Submission history**  
**[v1]** 19 Jul 2019: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:19.059" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:19.059](https://www.plumed-nest.org/eggs/19/059/badge.svg)](https://www.plumed-nest.org/eggs/19/059/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/19/059/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/19/059/badge.svg" alt="plumID:19.059"&gt;&lt;/a&gt;</pre>
  </div>
</div>
