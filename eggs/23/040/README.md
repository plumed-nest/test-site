**Project ID:** [plumID:23.040]({{ '/' | absolute_url }}eggs/23/040/)  
**Name:**  Supramolecular capsules assembly dynamics  
**Archive:** [ https://github.com/riccardocapelli/papers_data/raw/master/capsule_assembly2023/input_data.zip](https://github.com/riccardocapelli/papers_data/raw/master/capsule_assembly2023/input_data.zip)  
**Category:**  chemistry  
**Keywords:**  Self-assembly, H-bond capsules, resorcinarene, pyrogallolarene, metadynamics  
**PLUMED version:**  2.6  
**Contributor:**  Riccardo Capelli  
**Submitted on:** 06 Oct 2023  
**Publication:** [R. Capelli, G. Piccini, Atomistic Insights into Hydrogen-Bonded Supramolecular Capsule Self-Assembly Dynamics. The Journal of Physical Chemistry C. 128, 635–641 (2023)](http://dx.doi.org/10.1021/acs.jpcc.3c07148)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [plumed_analysis/pyrogallolarene/plumed_rewCVs.dat](./data/plumed_analysis/pyrogallolarene/plumed_rewCVs.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed_analysis/pyrogallolarene/plumed_rewCVs.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed_analysis/pyrogallolarene/plumed_rewCVs.dat.plumed_master.stderr) |  
| [plumed_analysis/pyrogallolarene/plumed_solvent.dat](./data/plumed_analysis/pyrogallolarene/plumed_solvent.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed_analysis/pyrogallolarene/plumed_solvent.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed_analysis/pyrogallolarene/plumed_solvent.dat.plumed_master.stderr) |  
| [plumed_analysis/resorcinarene/plumed_rewCVs.dat](./data/plumed_analysis/resorcinarene/plumed_rewCVs.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed_analysis/resorcinarene/plumed_rewCVs.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed_analysis/resorcinarene/plumed_rewCVs.dat.plumed_master.stderr) |  
| [plumed_analysis/resorcinarene/plumed_solvent.dat](./data/plumed_analysis/resorcinarene/plumed_solvent.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed_analysis/resorcinarene/plumed_solvent.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed_analysis/resorcinarene/plumed_solvent.dat.plumed_master.stderr) |  
| [plumed_metad/plumed_pyro.dat](./data/plumed_metad/plumed_pyro.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed_metad/plumed_pyro.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed_metad/plumed_pyro.dat.plumed_master.stderr) |  
| [plumed_metad/plumed_reso.dat](./data/plumed_metad/plumed_reso.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed_metad/plumed_reso.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed_metad/plumed_reso.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:27:15
  
**Project description and instructions**  
We performed for both resorcinarene and pyrogallolarene capsules a Well-Tempered metadynamics simulation, using GROMACS 2019.2 patched with PLUMED 2.6 (all the needed files for the GROMACS run are in the "input" folder, while the ones needed for plumed are in "plumed_metad" folder). The PLUMED input files for i) the calculation of the CVs used for the reweighting, ii) the calculation of the solvent molecules included in the capsules, and iii) the reweighting are in the "plumed_analysis" folder.
  
**Submission history**  
**[v1]** 06 Oct 2023: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:23.040" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:23.040](https://www.plumed-nest.org/eggs/23/040/badge.svg)](https://www.plumed-nest.org/eggs/23/040/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/23/040/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/23/040/badge.svg" alt="plumID:23.040"&gt;&lt;/a&gt;</pre>
  </div>
</div>
