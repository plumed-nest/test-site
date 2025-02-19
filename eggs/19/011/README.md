**Project ID:** [plumID:19.011]({{ '/' | absolute_url }}eggs/19/011/)  
**Name:**  Automatic Gradient Computation for Collective Variables  
**Archive:** [ https://github.com/tonigi/plumed2-automatic-gradients/releases/download/standalone-dist-v2.5.1-r2/plumed2-automatic-gradients-dist.zip](https://github.com/tonigi/plumed2-automatic-gradients/releases/download/standalone-dist-v2.5.1-r2/plumed2-automatic-gradients-dist.zip)  
**Category:**  other  
**Keywords:**  gradient, differentiation, curvature  
**PLUMED version:**  2.5.1-giorgino-j.cpc.2018.02.017  
**Contributor:**  Toni Giorgino  
**Submitted on:** 16 Apr 2019  
**Publication:** [T. Giorgino, How to differentiate collective variables in free energy codes: Computer-algebra code generation and automatic differentiation. Computer Physics Communications. 228, 258–263 (2018)](http://dx.doi.org/10.1016/j.cpc.2018.02.017)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [plumed-nest-readme.dat](./data/plumed-nest-readme.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed-nest-readme.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed-nest-readme.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:52:23
  
**Project description and instructions**  
This repository contains code illustrating two approaches to automate gradient computation for collective variables in PLUMED.  The two approaches are used to implement the example colvars `CURVATURE_CODEGEN` and `CURVATURE_AUTODIFF`, which compute the radius of curvature given three atoms, and `CURVATURE_MULTICOLVAR_CODEGEN`, given a polymer. The code is found in submodules named `src/curvature_codegen` (code generation approach from symbolic expressions by SymPy) and `src/curvature_autodiff` (code differentiation approach with the Stan Math library). Example files with regression tests are provided in the directories `regtest/curvature_codegen` and `regtest/curvature_autodiff` respectively.

  
**Submission history**  
**[v1]** 16 Apr 2019: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:19.011" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:19.011](https://www.plumed-nest.org/eggs/19/011/badge.svg)](https://www.plumed-nest.org/eggs/19/011/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/19/011/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/19/011/badge.svg" alt="plumID:19.011"&gt;&lt;/a&gt;</pre>
  </div>
</div>
