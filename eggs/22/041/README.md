**Project ID:** [plumID:22.041]({{ '/' | absolute_url }}eggs/22/041/)  
**Name:**  Skipping the Replica Exchange Ladder with Normalizing Flows  
**Archive:** [ https://github.com/invemichele/learned-replica-exchange/archive/main.zip](https://github.com/invemichele/learned-replica-exchange/archive/main.zip) [(browse)](https://github.com/invemichele/learned-replica-exchange/tree/main)  
**Category:**  methods  
**Keywords:**  OPES, alanine, normalizing flows, replica exchange  
**PLUMED version:**  2.8  
**Contributor:**  Michele Invernizzi  
**Submitted on:** 14 Nov 2022  
**Publication:** [M. Invernizzi, A. Krämer, C. Clementi, F. Noé, Skipping the Replica Exchange Ladder with Normalizing Flows. The Journal of Physical Chemistry Letters. 13, 11643–11649 (2022)](http://dx.doi.org/10.1021/acs.jpclett.2c03327)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [ala2/plumed.dat](./data/ala2/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/ala2/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/ala2/plumed.dat.plumed_master.stderr) |  
| [ala4/plumed.dat](./data/ala4/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/ala4/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/ala4/plumed.dat.plumed_master.stderr) |  
| [dw/plumed.dat](./data/dw/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/dw/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/dw/plumed.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:27:44
  
**Project description and instructions**  
PLUMED was used to obtain reference free energies with the OPES method. The main method described in the paper is not implemented in PLUMED. The Jupyter notebook contains an implementation in OpenMM of OPES for multithermal simulations (currently not supported by the `openmm-plumed` plugin).

  
**Submission history**  
**[v1]** 14 Nov 2022: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:22.041" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:22.041](https://www.plumed-nest.org/eggs/22/041/badge.svg)](https://www.plumed-nest.org/eggs/22/041/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/22/041/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/22/041/badge.svg" alt="plumID:22.041"&gt;&lt;/a&gt;</pre>
  </div>
</div>
