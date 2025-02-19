**Project ID:** [plumID:19.001]({{ '/' | absolute_url }}eggs/19/001/)  
**Name:**  RNA SHAPE  
**Archive:** [ https://github.com/srnas/shape-md/archive/4506611412ba0c88903483e814baec43b944453a.zip](https://github.com/srnas/shape-md/archive/4506611412ba0c88903483e814baec43b944453a.zip) [(browse)](https://github.com/srnas/shape-md/tree/4506611412ba0c88903483e814baec43b944453a)  
**Checksum (md5):** d9bffa6c195093a4d30e88286d292e4f  
**Category:**  bio  
**Keywords:**  metadynamics, RNA, ligand binding  
**PLUMED version:**  2.4  
**Contributor:**  Giovanni Bussi  
**Submitted on:** 10 Apr 2019  
**Last revised:** 03 Apr 2022  
**Publication:** [V. Mlýnský, G. Bussi, Molecular Dynamics Simulations Reveal an Interplay between SHAPE Reagent Binding and RNA Flexibility. The Journal of Physical Chemistry Letters. 9, 313–318 (2018)](http://dx.doi.org/10.1021/acs.jpclett.7b02921)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [plumed-g3.dat](./data/plumed-g3.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed-g3.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed-g3.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:54:14
  
**Project description and instructions**  
The zip file contains GROMACS topologies and input files together with a plumed example file. Notice that the simulations in the paper were performed using bias exchange metadynamics, and the example input correspond to a single replica (the one where ligand binding to residue 3 was enhanced). Input files for all replicas should be similarly created in order to run a real simulation.

  
**Submission history**  
**[v1]** 10 Apr 2019: original submission  
**[v2]** 03 Apr 2022: fixed input for plumed nest (removed RESTART)  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:19.001" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:19.001](https://www.plumed-nest.org/eggs/19/001/badge.svg)](https://www.plumed-nest.org/eggs/19/001/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/19/001/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/19/001/badge.svg" alt="plumID:19.001"&gt;&lt;/a&gt;</pre>
  </div>
</div>
