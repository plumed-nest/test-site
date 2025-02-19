**Project ID:** [plumID:21.018]({{ '/' | absolute_url }}eggs/21/018/)  
**Name:**  Localized Volume-based Metadynamics  
**Archive:** [ https://github.com/riccardocapelli/papers_data/raw/master/LV-MetaD_2021/input_data.zip](https://github.com/riccardocapelli/papers_data/raw/master/LV-MetaD_2021/input_data.zip)  
**Category:**  bio  
**Keywords:**  LV-MetaD, Volume-based MetaD, Metadynamics, Ligand binding, Induced-fit effects, Binding pose identification  
**PLUMED version:**  2.6  
**Contributor:**  Riccardo Capelli  
**Submitted on:** 04 May 2021  
**Last revised:** 09 Dec 2021  
**Publication:** [Q. Zhao, R. Capelli, P. Carloni, B. Lüscher, J. Li, G. Rossetti, Enhanced Sampling Approach to the Induced-Fit Docking Problem in Protein–Ligand Binding: The Case of Mono-ADP-Ribosylation Hydrolase Inhibitors. Journal of Chemical Theory and Computation. 17, 7899–7911 (2021)](http://dx.doi.org/10.1021/acs.jctc.1c00649)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [input/MacroD2_I189R_input/metad_35ang.dat](./data/input/MacroD2_I189R_input/metad_35ang.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/input/MacroD2_I189R_input/metad_35ang.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/input/MacroD2_I189R_input/metad_35ang.dat.plumed_master.stderr) |  
| [input/MacroD1_para_input/metad_35ang.dat](./data/input/MacroD1_para_input/metad_35ang.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/input/MacroD1_para_input/metad_35ang.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/input/MacroD1_para_input/metad_35ang.dat.plumed_master.stderr) |  
| [input/MacroD2_Y190N_input/metad_35ang.dat](./data/input/MacroD2_Y190N_input/metad_35ang.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/input/MacroD2_Y190N_input/metad_35ang.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/input/MacroD2_Y190N_input/metad_35ang.dat.plumed_master.stderr) |  
| [input/MacroD2_para_input/metad_35ang.dat](./data/input/MacroD2_para_input/metad_35ang.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/input/MacroD2_para_input/metad_35ang.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/input/MacroD2_para_input/metad_35ang.dat.plumed_master.stderr) |  
| [input/MacroD2_sphere_input/metad_35ang.dat](./data/input/MacroD2_sphere_input/metad_35ang.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/input/MacroD2_sphere_input/metad_35ang.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/input/MacroD2_sphere_input/metad_35ang.dat.plumed_master.stderr) |  
| [plumed_metad/metad_35ang_sphere.dat](./data/plumed_metad/metad_35ang_sphere.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed_metad/metad_35ang_sphere.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed_metad/metad_35ang_sphere.dat.plumed_master.stderr) |  
| [plumed_metad/metad_35ang_para.dat](./data/plumed_metad/metad_35ang_para.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed_metad/metad_35ang_para.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed_metad/metad_35ang_para.dat.plumed_master.stderr) |  
| [plumed_reweight/reweight_rho_hb.dat](./data/plumed_reweight/reweight_rho_hb.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed_reweight/reweight_rho_hb.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/plumed_reweight/reweight_rho_hb.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:47:03
  
**Project description and instructions**  
All the input files to simulate MacroD1, MacroD2, and the studied mutants of MacroD2 (Y190N and I189R) in complex with ADPr using Gromacs 2019.2 are in the *input* folder.   In the *plumed_metad* folder 2 reference input files for parabolic and 1/3 sphere volume restraint are available.  In the *plumed_reweight* folder the reweight input file is available. 

  
**Submission history**  
**[v1]** 04 May 2021: original submission  
**[v2]** 04 Aug 2021: updated doi  
**[v3]** 09 Dec 2021: updated doi  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:21.018" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:21.018](https://www.plumed-nest.org/eggs/21/018/badge.svg)](https://www.plumed-nest.org/eggs/21/018/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/21/018/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/21/018/badge.svg" alt="plumID:21.018"&gt;&lt;/a&gt;</pre>
  </div>
</div>
