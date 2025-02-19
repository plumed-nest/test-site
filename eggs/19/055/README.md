**Project ID:** [plumID:19.055]({{ '/' | absolute_url }}eggs/19/055/)  
**Name:**  Flying Gaussian method  
**Archive:** [ https://archive.materialscloud.org/record/file?file_id=bd5f8b2e-50a2-4f5e-897a-b4eeec1cf8d5&record_id=158&filename=flyinggaussian.zip](https://archive.materialscloud.org/record/file?file_id=bd5f8b2e-50a2-4f5e-897a-b4eeec1cf8d5&record_id=158&filename=flyinggaussian.zip)  
**Category:**  methods  
**Keywords:**  flying Gaussians, alanine dipeptide, peptide bond, Met-enkephalin  
**PLUMED version:**  2.5.0  
**Contributor:**  Vojtech Spiwok  
**Submitted on:** 17 Jun 2019  
**Last revised:** 18 Jun 2019  
**Publication:** [Z. Šućur, V. Spiwok, Sampling Enhancement and Free Energy Prediction by the Flying Gaussian Method. Journal of Chemical Theory and Computation. 12, 4644–4650 (2016)](http://dx.doi.org/10.1021/acs.jctc.6b00551)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [AceProNH2/plumed.dat](./data/AceProNH2/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/AceProNH2/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/AceProNH2/plumed.dat.plumed_master.stderr) |  
| [AceProProNH2/plumed.dat](./data/AceProProNH2/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/AceProProNH2/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/AceProProNH2/plumed.dat.plumed_master.stderr) |  
| [AceProProProNH2/plumed.dat](./data/AceProProProNH2/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/AceProProProNH2/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/AceProProProNH2/plumed.dat.plumed_master.stderr) |  
| [acealanmevacuum/plumed.dat](./data/acealanmevacuum/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/acealanmevacuum/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/acealanmevacuum/plumed.dat.plumed_master.stderr) |  
| [acealanmewater16/plumed.dat](./data/acealanmewater16/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/acealanmewater16/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/acealanmewater16/plumed.dat.plumed_master.stderr) |  
| [acealanmewater32/plumed.dat](./data/acealanmewater32/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/acealanmewater32/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/acealanmewater32/plumed.dat.plumed_master.stderr) |  
| [acealanmewater64/plumed.dat](./data/acealanmewater64/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/acealanmewater64/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/acealanmewater64/plumed.dat.plumed_master.stderr) |  
| [acealanmewater8/plumed.dat](./data/acealanmewater8/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/acealanmewater8/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/acealanmewater8/plumed.dat.plumed_master.stderr) |  
| [metenkephalin/plumed.dat](./data/metenkephalin/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/metenkephalin/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/metenkephalin/plumed.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:52:58
  
**Project description and instructions**  
Input files (input structures, topology, Plumed input files) for simulations used to demonstrate functionality of Flying Gaussian algorithm ([J. Chem. Theory Comput. 2016, 12, 4644-4650](https://pubs.acs.org/doi/10.1021/acs.jctc.6b00551)). The method simulates a molecular system in multiple replicas and enhances sampling by disfavoring states that are close to each other in different replicas. Input files for Flying Gaussian simulation of alanine dipeptide in vacuum and water, cis/trans isomerization of Ace-(Pro)n-NH2 and Met-enkephalin are provided.

  
**Submission history**  
**[v1]** 17 Jun 2019: original submission  
**[v2]** 18 Jun 2019: Switched to Materials Cloud  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:19.055" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:19.055](https://www.plumed-nest.org/eggs/19/055/badge.svg)](https://www.plumed-nest.org/eggs/19/055/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/19/055/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/19/055/badge.svg" alt="plumID:19.055"&gt;&lt;/a&gt;</pre>
  </div>
</div>
