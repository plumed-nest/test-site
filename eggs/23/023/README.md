**Project ID:** [plumID:23.023]({{ '/' | absolute_url }}eggs/23/023/)  
**Name:**  Rational design of novel biomimetic sequence-defined polymers for mineralization applications  
**Archive:** [ https://github.com/katorke/R5_Mineralization/raw/main/plumed_nest.zip](https://github.com/katorke/R5_Mineralization/raw/main/plumed_nest.zip)  
**Category:**  methods  
**Keywords:**  metadynamics, surface binding, biomimetic mineralization  
**PLUMED version:**  2.8  
**Contributor:**  Kaylyn Torkelson  
**Submitted on:** 15 Jun 2023  
**Publication:** [K. Torkelson, N. Y. Naser, X. Qi, Z. Li, W. Yang, K. Pushpavanam, C.-L. Chen, F. Baneyx, J. Pfaendtner, Rational Design of Novel Biomimetic Sequence-Defined Polymers for Mineralization Applications. Chemistry of Materials. 36, 786–794 (2024)](http://dx.doi.org/10.1021/acs.chemmater.3c02216)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [dimer_files/plumed.dat](./data/dimer_files/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/dimer_files/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/dimer_files/plumed.dat.plumed_master.stderr) |  
| [silicate_files/plumed.dat](./data/silicate_files/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/silicate_files/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/silicate_files/plumed.dat.plumed_master.stderr) |  
| [surface_files/plumed.dat](./data/surface_files/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/surface_files/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/surface_files/plumed.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:23:16
  
**Project description and instructions**  
Each directory (dimer_files, silicate_files, surface_files) contains an example gro file (system.gro), the topology files needed to run that system (*.itp and topol.top), an example mdp file, and the plumed.dat file corresponding to each simulation type. Each metadynamics calculation was run in GROMACS 2020.5 with PLUMED 2.8. The main directory contains a directory named PDB that has example structures for all five systems studied (R5 peptide, R5 peptoid mimic, R5 peptoid analog, R5 peptide reverse, and R5 peptoid analog reverse) as well as another forcefield directory that contains all the modifications necessary to run our peptoid systems.
  
**Submission history**  
**[v1]** 15 Jun 2023: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:23.023" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:23.023](https://www.plumed-nest.org/eggs/23/023/badge.svg)](https://www.plumed-nest.org/eggs/23/023/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/23/023/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/23/023/badge.svg" alt="plumID:23.023"&gt;&lt;/a&gt;</pre>
  </div>
</div>
