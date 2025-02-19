**Project ID:** [plumID:23.016]({{ '/' | absolute_url }}eggs/23/016/)  
**Name:**  Activation/deactivation free-energy profiles for the β2-adrenergic receptor: Ligand modes of action  
**Archive:** [ https://github.com/jacquecr23/Activation-free-energy-profiles-for-ADRB2/raw/main/Activation%20free%20energy%20profiles%20for%20ADRB2.zip](https://github.com/jacquecr23/Activation-free-energy-profiles-for-ADRB2/raw/main/Activation%20free%20energy%20profiles%20for%20ADRB2.zip)  
**Category:**  bio  
**Keywords:**  G protein coupled receptor, beta-adrenergic, receptor activation, partial agonism, metadynamics  
**PLUMED version:**  2.5.3  
**Contributor:**  Timothy Clark  
**Submitted on:** 27 Apr 2023  
**Publication:** [J. C. Calderón, P. Ibrahim, D. Gobbo, F. L. Gervasio, T. Clark, Activation/Deactivation Free-Energy Profiles for the β2-Adrenergic Receptor: Ligand Modes of Action. Journal of Chemical Information and Modeling. 63, 6332–6343 (2023)](http://dx.doi.org/10.1021/acs.jcim.3c00805)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [plumed.dat](./data/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed.dat.plumed_master.stderr) |  
| [plumed_reweight_2D_microsw_adr_bin.dat](./data/plumed_reweight_2D_microsw_adr_bin.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed_reweight_2D_microsw_adr_bin.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/plumed_reweight_2D_microsw_adr_bin.dat.plumed_master.stderr) |  
| [plumed_reweight_microsw_adr_bin.dat](./data/plumed_reweight_microsw_adr_bin.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed_reweight_microsw_adr_bin.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/plumed_reweight_microsw_adr_bin.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:36:22
  
**Project description and instructions**  
Multiple-walkers Metadynamics simulations were performed using GROMACS 2019.4 with the PLUMED 2.5.3 plug-in. Topologies for the receptors were generated using the AMBER99SB-ILDN force field. Ligands were parameterized using the generalized AMBER force field (GAFF) together with AM1-BCC partial charges.
  
**Submission history**  
**[v1]** 27 Apr 2023: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:23.016" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:23.016](https://www.plumed-nest.org/eggs/23/016/badge.svg)](https://www.plumed-nest.org/eggs/23/016/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/23/016/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/23/016/badge.svg" alt="plumID:23.016"&gt;&lt;/a&gt;</pre>
  </div>
</div>
