**Project ID:** [plumID:22.037]({{ '/' | absolute_url }}eggs/22/037/)  
**Name:**  Splitting of Energetic and Dynamics Base Pairing Cooperativity in DNA Duplexes by an Abasic Site  
**Archive:** [ https://github.com/mrjoness/abasic-thermo/archive/refs/heads/main.zip](https://github.com/mrjoness/abasic-thermo/archive/refs/heads/main.zip)  
**Category:**  chemistry  
**Keywords:**  metadynamics, DNA, abasic  
**PLUMED version:**  2.7  
**Contributor:**  Mike Jones  
**Submitted on:** 16 Oct 2022  
**Publication:** [B. Ashwood, M. S. Jones, A. L. Ferguson, A. Tokmakoff, Disruption of energetic and dynamic base pairing cooperativity in DNA duplexes by an abasic site. Proceedings of the National Academy of Sciences. 120 (2023)](http://dx.doi.org/10.1073/pnas.2219124120)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [metad_setup/11bp_abasic-2_plumed.dat](./data/metad_setup/11bp_abasic-2_plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/metad_setup/11bp_abasic-2_plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/metad_setup/11bp_abasic-2_plumed.dat.plumed_master.stderr) |  
| [metad_setup/11bp_abasic-4_plumed.dat](./data/metad_setup/11bp_abasic-4_plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/metad_setup/11bp_abasic-4_plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/metad_setup/11bp_abasic-4_plumed.dat.plumed_master.stderr) |  
| [metad_setup/11bp_abasic-6_plumed.dat](./data/metad_setup/11bp_abasic-6_plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/metad_setup/11bp_abasic-6_plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/metad_setup/11bp_abasic-6_plumed.dat.plumed_master.stderr) |  
| [metad_setup/11bp_plumed.dat](./data/metad_setup/11bp_plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/metad_setup/11bp_plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/metad_setup/11bp_plumed.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:31:28
  
**Project description and instructions**  
Input files are compatible with the 3 Sites Per Nucleotide (3SPN.2) plugin for LAMMPS and applied to three 11-mer DNA oligomer sequences. 11bp_plumed.dat biases the mean distance between native base pairs for an intact (WT) oligomer. 11bp_abasic-6_plumed.dat biases the mean distance between all available native base pairs for an abasic sequence with the central nucleobase removed. PLUMED files for additional abasic configurations can be generated using abasic_site_to_plumed.py.

  
**Submission history**  
**[v1]** 16 Oct 2022: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:22.037" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:22.037](https://www.plumed-nest.org/eggs/22/037/badge.svg)](https://www.plumed-nest.org/eggs/22/037/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/22/037/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/22/037/badge.svg" alt="plumID:22.037"&gt;&lt;/a&gt;</pre>
  </div>
</div>
