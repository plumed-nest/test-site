**Project ID:** [plumID:22.003]({{ '/' | absolute_url }}eggs/22/003/)  
**Name:**  Exploration vs Convergence Speed in Adaptive-bias Enhanced Sampling  
**Archive:** [ https://github.com/invemichele/OPES-explore/archive/main.zip](https://github.com/invemichele/OPES-explore/archive/main.zip) [(browse)](https://github.com/invemichele/OPES-explore/tree/main)  
**Category:**  methods  
**Keywords:**  opes, metadynamics, reweighting, alanine, muller  
**PLUMED version:**  2.8  
**Contributor:**  Michele Invernizzi  
**Submitted on:** 26 Jan 2022  
**Last revised:** 28 May 2022  
**Publication:** [M. Invernizzi, M. Parrinello, Exploration vs Convergence Speed in Adaptive-Bias Enhanced Sampling. Journal of Chemical Theory and Computation. 18, 3988–3996 (2022)](http://dx.doi.org/10.1021/acs.jctc.2c00152)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [ala2/explore/plumed.dat](./data/ala2/explore/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/ala2/explore/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/ala2/explore/plumed.dat.plumed_master.stderr) |  
| [ala2/opes/plumed.dat](./data/ala2/opes/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/ala2/opes/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/ala2/opes/plumed.dat.plumed_master.stderr) |  
| [ala4/combined_multiT-psi/plumed.dat](./data/ala4/combined_multiT-psi/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/ala4/combined_multiT-psi/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/ala4/combined_multiT-psi/plumed.dat.plumed_master.stderr) |  
| [ala4/explore/plumed.dat](./data/ala4/explore/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/ala4/explore/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/ala4/explore/plumed.dat.plumed_master.stderr) |  
| [ala4/metad/plumed.dat](./data/ala4/metad/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/ala4/metad/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/ala4/metad/plumed.dat.plumed_master.stderr) |  
| [ala4/opes/plumed.dat](./data/ala4/opes/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/ala4/opes/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/ala4/opes/plumed.dat.plumed_master.stderr) |  
| [ala4/pbmetad/plumed.dat](./data/ala4/pbmetad/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/ala4/pbmetad/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/ala4/pbmetad/plumed.dat.plumed_master.stderr) |  
| [mueller/explore/plumed.dat](./data/mueller/explore/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/mueller/explore/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/mueller/explore/plumed.dat.plumed_master.stderr) |  
| [mueller/metad/plumed.dat](./data/mueller/metad/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/mueller/metad/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/mueller/metad/plumed.dat.plumed_master.stderr) |  
| [mueller/opes/plumed.dat](./data/mueller/opes/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/mueller/opes/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/mueller/opes/plumed.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:25:06
  
**Project description and instructions**  
Introducing the exploratory variant of the OPES method, [OPES_METAD_EXPLORE](https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s__m_e_t_a_d__e_x_p_l_o_r_e.html). It is tested on model systems and compared with standard OPES and metadynamics. The MD engine used is GROMACS 2019.

  
**Submission history**  
**[v1]** 26 Jan 2022: original submission  
**[v2]** 28 May 2022: updated doi  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:22.003" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:22.003](https://www.plumed-nest.org/eggs/22/003/badge.svg)](https://www.plumed-nest.org/eggs/22/003/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/22/003/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/22/003/badge.svg" alt="plumID:22.003"&gt;&lt;/a&gt;</pre>
  </div>
</div>
