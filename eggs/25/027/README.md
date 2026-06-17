**Project ID:** [plumID:25.027]({{ '/' | absolute_url }}eggs/25/027/)  
**Name:**  Enhanced-sampling MD simulations of a protein-peptide complex integrating SAXS and XL-MS experimental information  
**Archive:** [ https://github.com/mbernett/zip_for_nest/raw/master/saxs-xlms-md_rad.zip](https://github.com/mbernett/zip_for_nest/raw/master/saxs-xlms-md_rad.zip)  
**Category:**  bio  
**Keywords:**  steered MD, metadynamics, SAXS, XL-MS, ensemble reconstruction  
**PLUMED version:**  2.9  
**Contributor:**  Mattia Bernetti  
**Submitted on:** 02 Sep 2025  
**Publication:** [V. Bresciani, F. Rinaldi, P. Franco, S. Girotto, A. Cavalli, J. D. Langer, M. Masetti, M. Bernetti, Integrating computational and experimental biophysics reveals novel insights into the RAD51-BRC4 interaction. doi: 10.1101/2025.03.07.642044 (2025)](http://dx.doi.org/10.1101/2025.03.07.642044)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [metad/input/plumed_input_maxent_onebead.dat](./data/metad/input/plumed_input_maxent_onebead.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/metad/input/plumed_input_maxent_onebead.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/metad/input/plumed_input_maxent_onebead.dat.plumed_master.stderr) |  
| [...reweighting/plumed_input_maxent_onebead_DRIVER.dat](./data/metad/reweighting/plumed_input_maxent_onebead_DRIVER.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/metad/reweighting/plumed_input_maxent_onebead_DRIVER.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/metad/reweighting/plumed_input_maxent_onebead_DRIVER.dat.plumed_master.stderr) |  
| [...weighting/plumed_input_maxent_onebead_reweight.dat](./data/metad/reweighting/plumed_input_maxent_onebead_reweight.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/metad/reweighting/plumed_input_maxent_onebead_reweight.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/metad/reweighting/plumed_input_maxent_onebead_reweight.dat.plumed_master.stderr) |  
| [steered_input/martini/plumed_beads.dat](./data/steered_input/martini/plumed_beads.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/steered_input/martini/plumed_beads.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/steered_input/martini/plumed_beads.dat.plumed_master.stderr) |  
| [steered_input/martini/plumed_input_steered.dat](./data/steered_input/martini/plumed_input_steered.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/steered_input/martini/plumed_input_steered.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/steered_input/martini/plumed_input_steered.dat.plumed_master.stderr) |  
| [...red_input/onebead/plumed_input_steered_onebead.dat](./data/steered_input/onebead/plumed_input_steered_onebead.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/steered_input/onebead/plumed_input_steered_onebead.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/steered_input/onebead/plumed_input_steered_onebead.dat.plumed_master.stderr) |  
  
**Last tested:**  17 Jun 2026, 09:12:23
  
**Project description and instructions**  
Input files to carry out MD simulations of the RAD51-BRC4 complex using enhanced sampling methods, namely steered MD and metadynamics. The simulations integrate experimental information, specifically from SAXS in the steered MD and from XL-MS in the metad. The input folders contain all files required to perform the simulations, while the reweighting subfolder in the metad directory includes input files to compute metad weights a posteriori using the final bias. Simulations were conducted using GROMACS 2023.1 patched with PLUMED 2.9. All the files necessary to reproduce the analyses through a Jupyter Notebook are available on Zenodo under accession code 10.5281/zenodo.17035732.

  
{% raw %}
<b><a href="https://www.plumed.org/doc-master/user-doc/html/actionlist/?actions=GROUP,GYRATION,SAXS,CENTER,MOVINGRESTRAINT,DISTANCE,UPPER_WALLS,WHOLEMOLECULES,PRINT,MOLINFO,METAD,INCLUDE" target="_blank">Click here</a> to open manual pages for actions used in this project.</b>
{% endraw %}
**Submission history**  
**[v1]** 02 Sep 2025: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:25.027" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:25.027](https://www.plumed-nest.org/eggs/25/027/badge.svg)](https://www.plumed-nest.org/eggs/25/027/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/25/027/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/25/027/badge.svg" alt="plumID:25.027"&gt;&lt;/a&gt;</pre>
  </div>
</div>
