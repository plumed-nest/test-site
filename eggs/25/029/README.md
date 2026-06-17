**Project ID:** [plumID:25.029]({{ '/' | absolute_url }}eggs/25/029/)  
**Name:**  Energetic Constraints in the Enzymatic Depolymerization of Crystalline PET from enhanced molecular simulations  
**Archive:** [ https://github.com/fcolizzi/PETase_Cryst-vs-Amor/raw/main/PETase-cryst-vs-amor.zip](https://github.com/fcolizzi/PETase_Cryst-vs-Amor/raw/main/PETase-cryst-vs-amor.zip)  
**Category:**  bio  
**Keywords:**  HREX-Metadynamics, PETase, crystalline PET, amorphous PET, conformational ensembles, substrate binding, chain detachment  
**PLUMED version:**  2.8  
**Contributor:**  Ania Di Pede-Mattatelli and Francesco Colizzi  
**Submitted on:** 08 Nov 2025  
**Publication:** unpublished  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [./PET_extr/eq2_amor.dat](./data/./PET_extr/eq2_amor.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/./PET_extr/eq2_amor.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/./PET_extr/eq2_amor.dat.plumed_master.stderr) |  
| [./PET_extr/mtd_amor.dat](./data/./PET_extr/mtd_amor.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/./PET_extr/mtd_amor.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/./PET_extr/mtd_amor.dat.plumed_master.stderr) |  
| [./PET_extr/mtd_crys.dat](./data/./PET_extr/mtd_crys.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/./PET_extr/mtd_crys.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/./PET_extr/mtd_crys.dat.plumed_master.stderr) |  
| [./PET_extr/eq2_crys.dat](./data/./PET_extr/eq2_crys.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/./PET_extr/eq2_crys.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/./PET_extr/eq2_crys.dat.plumed_master.stderr) |  
| [./amor/4-reweight_amor.dat](./data/./amor/4-reweight_amor.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-failed-red.svg)](data/./amor/4-reweight_amor.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/./amor/4-reweight_amor.dat.plumed_master.stderr) |  
| [./amor/2-eq2_amor.dat](./data/./amor/2-eq2_amor.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/./amor/2-eq2_amor.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/./amor/2-eq2_amor.dat.plumed_master.stderr) |  
| [./amor/3-production_mtd_hrex_amor.dat](./data/./amor/3-production_mtd_hrex_amor.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/./amor/3-production_mtd_hrex_amor.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/./amor/3-production_mtd_hrex_amor.dat.plumed_master.stderr) |  
| [./crys/3-production_mtd_hrex_crys.dat](./data/./crys/3-production_mtd_hrex_crys.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/./crys/3-production_mtd_hrex_crys.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/./crys/3-production_mtd_hrex_crys.dat.plumed_master.stderr) |  
| [./crys/2-eq2_crys.dat](./data/./crys/2-eq2_crys.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/./crys/2-eq2_crys.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/./crys/2-eq2_crys.dat.plumed_master.stderr) |  
| [./crys/4-reweight_crys.dat](./data/./crys/4-reweight_crys.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-failed-red.svg)](data/./crys/4-reweight_crys.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/./crys/4-reweight_crys.dat.plumed_master.stderr) |  
  
**Last tested:**  17 Jun 2026, 09:06:06
  
**Project description and instructions**  
Simulations have been performed with GROMACS 2021.4 and PLUMED 2.8. The input files for wt-MTD, and combined HREX-wt-MTD simulations of IsPETase-PET and PET-PET systems are provided, along with PLUMED input files for the analysis and reweighting. To get the .tpr and .gro files, please see [here](https://github.com/fcolizzi/PETase_Cryst-vs-Amor). 

  
{% raw %}
<b><a href="https://www.plumed.org/doc-master/user-doc/html/actionlist/?actions=UPPER_WALLS,DISTANCE,MOLINFO,LOWER_WALLS,CONVERT_TO_FES,REWEIGHT_BIAS,PRINT,DUMPGRID,COM,METAD,WHOLEMOLECULES,FIXEDATOM,HISTOGRAM" target="_blank">Click here</a> to open manual pages for actions used in this project.</b>
{% endraw %}
**Submission history**  
**[v1]** 08 Nov 2025: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:25.029" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:25.029](https://www.plumed-nest.org/eggs/25/029/badge.svg)](https://www.plumed-nest.org/eggs/25/029/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/25/029/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/25/029/badge.svg" alt="plumID:25.029"&gt;&lt;/a&gt;</pre>
  </div>
</div>
