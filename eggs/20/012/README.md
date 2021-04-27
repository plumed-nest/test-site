**Project ID:** [plumID:20.012]({{ '/' | absolute_url }}eggs/20/012/)  
**Name:**  Combining Machine Learning and Enhanced Sampling Techniques for Efficient and Accurate Calculation of Absolute Binding Free Energies  
**Archive:** [ https://github.com/Gervasiolab/Gervasio-Protein-Dynamics/raw/master/Fun-metaD_Fun-SWISH/PLUMED-NEST.zip](https://github.com/Gervasiolab/Gervasio-Protein-Dynamics/raw/master/Fun-metaD_Fun-SWISH/PLUMED-NEST.zip)  
**Category:**  bio  
**Keywords:**  metadynamics, well-tempered ensemble, ligand binding, binding affinity calculations, novel COLVAR, funnel restraints, Hamiltonian replica-exchange, PathCV, COMetPath, SWISH  
**PLUMED version:**  2.4.2  
**Contributor:**  Francesco Gervasio  
**Submitted on:** 29 Apr 2020  
**Last revised:** 23 May 2020  
**Publication:** [R. Evans et al., Combining Machine Learning and Enhanced Sampling Techniques for Efficient and Accurate Calculation of Absolute Binding Free Energies, Journal of Chemical Theory and Computation 16, 4641–4654 (2020)](http://dx.doi.org/10.1021/acs.jctc.0c00075)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [COMet_Path/plumed.dat](./data/COMet_Path/plumed.dat.md) |  [![tested on v2.7](https://img.shields.io/badge/v2.7-failed-red.svg)](data/COMet_Path/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/COMet_Path/plumed.dat.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
| [fun_SWISH/plumed.dat](./data/fun_SWISH/plumed.dat.md) |  [![tested on v2.7](https://img.shields.io/badge/v2.7-failed-red.svg)](data/fun_SWISH/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/fun_SWISH/plumed.dat.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
| [fun_metaD/plumed.dat](./data/fun_metaD/plumed.dat.md) |  [![tested on v2.7](https://img.shields.io/badge/v2.7-failed-red.svg)](data/fun_metaD/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/fun_metaD/plumed.dat.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
  
**Last tested:**  27 Apr 2021, 22:36:48
  
**Project description and instructions**  
These are the input files used to fully converge the free energy landscapes of the human soluble epoxide hydrolase (sEH, PDB code 5AKK) using different methodologies, Funnel-shaped restraint metadynamics (fun-metaD), funnel-shaped restraint with SWISH (fun-SWISH) and COMetPath. The input files were used with GROMACS 2018.3 and PLUMED 2.4.2 using the AMBER99SB-disp force field. They include a novel COLVAR(ProjectionOnAxis.cpp) which is included in all directories. 

  
**Submission history**  
**[v1]** 29 Apr 2020: original submission  
**[v2]** 23 May 2020: updated doi  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:20.012" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:20.012](https://www.plumed-nest.org/eggs/20/012/badge.svg)](https://www.plumed-nest.org/eggs/20/012/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/20/012/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/20/012/badge.svg" alt="plumID:20.012"&gt;&lt;/a&gt;</pre>
  </div>
</div>
