**Project ID:** [plumID:21.020]({{ '/' | absolute_url }}eggs/21/020/)  
**Name:**  Reweighted Jarzynski sampling  
**Archive:** [ https://github.com/kbal/reweightedjarzynski/archive/main.zip](https://github.com/kbal/reweightedjarzynski/archive/main.zip) [(browse)](https://github.com/kbal/reweightedjarzynski/tree/main)  
**Category:**  methods  
**Keywords:**  free energies, steered MD, neural network, nonequilibrium work, nucleation, chemical reactions  
**PLUMED version:**  2.8  
**Contributor:**  Kristof Bal  
**Submitted on:** 07 May 2021  
**Last revised:** 02 Nov 2021  
**Publication:** [K. M. Bal, Reweighted Jarzynski Sampling: Acceleration of Rare Events and Free Energy Calculation with a Bias Potential Learned from Nonequilibrium Work. Journal of Chemical Theory and Computation. 17, 6766–6774 (2021)](http://dx.doi.org/10.1021/acs.jctc.1c00574)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [droplet/smd/plumed1.inp](./data/droplet/smd/plumed1.inp.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/droplet/smd/plumed1.inp.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/droplet/smd/plumed1.inp.plumed_master.stderr) |  
| [droplet/smd/plumed2.inp](./data/droplet/smd/plumed2.inp.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/droplet/smd/plumed2.inp.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/droplet/smd/plumed2.inp.plumed_master.stderr) |  
| [droplet/fes/plumed.inp](./data/droplet/fes/plumed.inp.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/droplet/fes/plumed.inp.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/droplet/fes/plumed.inp.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
| [dimer/smd/plumed1.inp](./data/dimer/smd/plumed1.inp.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/dimer/smd/plumed1.inp.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/dimer/smd/plumed1.inp.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
| [dimer/smd/plumed2.inp](./data/dimer/smd/plumed2.inp.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/dimer/smd/plumed2.inp.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/dimer/smd/plumed2.inp.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
| [dimer/fes/plumed.inp](./data/dimer/fes/plumed.inp.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/dimer/fes/plumed.inp.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/dimer/fes/plumed.inp.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
| [sn2/smd/plumed.inp](./data/sn2/smd/plumed.inp.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/sn2/smd/plumed.inp.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/sn2/smd/plumed.inp.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
| [sn2/fes/plumed.inp](./data/sn2/fes/plumed.inp.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/sn2/fes/plumed.inp.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/sn2/fes/plumed.inp.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
| [hbr/smd/plumed.inp](./data/hbr/smd/plumed.inp.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/hbr/smd/plumed.inp.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/hbr/smd/plumed.inp.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
| [hbr/fes/plumed.inp](./data/hbr/fes/plumed.inp.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/hbr/fes/plumed.inp.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/hbr/fes/plumed.inp.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
| [hbr/hlda/1/plumed.inp](./data/hbr/hlda/1/plumed.inp.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/hbr/hlda/1/plumed.inp.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/hbr/hlda/1/plumed.inp.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
| [hbr/hlda/2/plumed.inp](./data/hbr/hlda/2/plumed.inp.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/hbr/hlda/2/plumed.inp.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/hbr/hlda/2/plumed.inp.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
| [hbr/metad/plumed.inp](./data/hbr/metad/plumed.inp.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/hbr/metad/plumed.inp.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/hbr/metad/plumed.inp.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
| [hbr/ves/plumed.inp](./data/hbr/ves/plumed.inp.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/hbr/ves/plumed.inp.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/hbr/ves/plumed.inp.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
| [hbr/opes/plumed.inp](./data/hbr/opes/plumed.inp.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/hbr/opes/plumed.inp.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/hbr/opes/plumed.inp.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
  
**Last tested:**  19 Feb 2025, 14:29:41
  
**Project description and instructions**  
A simple enhanced sampling approach using a bias potential learned from a nonequilibrium work distribution  and the Jarzynski equality. LAMMPS, CP2K, and PLUMED inputs are provided. For each system, the workflow is as follows. 1) Perform a number of steered MD (SMD) runs along the reaction coordinate of choice.  2) Fit a  neural network (NN) to the approximate free energy surface with the nn.py script.  3) Calculate the true free energy surface from a biased run, using the NN as bias potential, as a  reweighted histogram. Processing of the SMD runs has to be done with the nn.py scripts provided for each system, which depend  on scikit-learn and numpy. For the HBr system we also have inputs for the HLDA analysis, for which you'll  need G. Piccini's [scripts](https://github.com/piccig/HLDA).

  
**Submission history**  
**[v1]** 07 May 2021: original submission  
**[v2]** 01 Sep 2021: updated examples  
**[v3]** 02 Nov 2021: updated doi  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:21.020" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:21.020](https://www.plumed-nest.org/eggs/21/020/badge.svg)](https://www.plumed-nest.org/eggs/21/020/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/21/020/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/21/020/badge.svg" alt="plumID:21.020"&gt;&lt;/a&gt;</pre>
  </div>
</div>
