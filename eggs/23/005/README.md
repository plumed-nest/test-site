**Project ID:** [plumID:23.005]({{ '/' | absolute_url }}eggs/23/005/)  
**Name:**  A general metadynamics protocol to simulate activation/deactivation of Class A GPCRs  
**Archive:** [ https://github.com/dorotheagobbo/5HT1_NEST/raw/main/apo-5HT1A.zip](https://github.com/dorotheagobbo/5HT1_NEST/raw/main/apo-5HT1A.zip)  
**Category:**  bio  
**Keywords:**  metadynamics, activation/deactivation, activation index, GPCRs, 5HT1A  
**PLUMED version:**  2.5.3  
**Contributor:**  Timothy Clark  
**Submitted on:** 13 Feb 2023  
**Publication:** [J. C. Calderón, P. Ibrahim, D. Gobbo, F. L. Gervasio, T. Clark, General Metadynamics Protocol To Simulate Activation/Deactivation of Class A GPCRs: Proof of Principle for the Serotonin Receptor. Journal of Chemical Information and Modeling. 63, 3105–3117 (2023)](http://dx.doi.org/10.1021/acs.jcim.3c00208)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [apo-5HT1A/plumed.dat](./data/apo-5HT1A/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/apo-5HT1A/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/apo-5HT1A/plumed.dat.plumed_master.stderr) |  
| [apo-5HT1A/plumed_reweight_2D_microsw_5ht1a_rec.dat](./data/apo-5HT1A/plumed_reweight_2D_microsw_5ht1a_rec.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/apo-5HT1A/plumed_reweight_2D_microsw_5ht1a_rec.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/apo-5HT1A/plumed_reweight_2D_microsw_5ht1a_rec.dat.plumed_master.stderr) |  
| [apo-5HT1A/plumed_reweight_microsw_5ht1a_rec.dat](./data/apo-5HT1A/plumed_reweight_microsw_5ht1a_rec.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/apo-5HT1A/plumed_reweight_microsw_5ht1a_rec.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/apo-5HT1A/plumed_reweight_microsw_5ht1a_rec.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:38:51
  
**Project description and instructions**  
Multiple-walkers Metadynamics simulations were performed using GROMACS 2019.4 with the PLUMED 2.5.3 plug-in. Topologies for the receptors were generated using the AMBER99SB-ILDN force field. Ligands were parameterized using the generalized AMBER force field (GAFF) together with AM1-BCC partial charges.
  
**Submission history**  
**[v1]** 13 Feb 2023: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:23.005" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:23.005](https://www.plumed-nest.org/eggs/23/005/badge.svg)](https://www.plumed-nest.org/eggs/23/005/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/23/005/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/23/005/badge.svg" alt="plumID:23.005"&gt;&lt;/a&gt;</pre>
  </div>
</div>
