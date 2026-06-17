**Project ID:** [plumID:25.009]({{ '/' | absolute_url }}eggs/25/009/)  
**Name:**  Ab Initio Multiple Walkers Metadynamics Simulations of Nitrate Photolysis in Water  
**Archive:** [ https://github.com/kamtung-tonybill/Nitrate_Photolysis_Aqueous_Solution/archive/refs/heads/main.zip](https://github.com/kamtung-tonybill/Nitrate_Photolysis_Aqueous_Solution/archive/refs/heads/main.zip)  
**Category:**  chemistry  
**Keywords:**  metadynamics, nitrate photolysis  
**PLUMED version:**  2.8  
**Contributor:**  Kam-Tung Chan  
**Submitted on:** 04 Apr 2025  
**Last revised:** 16 Jul 2025  
**Publication:** [K.-T. Chan, M. L. Berrens, Z. Chen, C. W. McCurdy, C. Anastasio, D. Donadio, Revealing the photochemical pathways of nitrate in water through first-principles simulations. The Journal of Chemical Physics 162 (2025)](http://dx.doi.org/10.1063/5.0262438)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [..._MetaD/hills/plumed-reweight-time-dependent-w0.dat](./data/T1_MetaD/hills/plumed-reweight-time-dependent-w0.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/T1_MetaD/hills/plumed-reweight-time-dependent-w0.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/T1_MetaD/hills/plumed-reweight-time-dependent-w0.dat.plumed_master.stderr) |  
| [..._MetaD/hills/plumed-reweight-time-dependent-w1.dat](./data/T1_MetaD/hills/plumed-reweight-time-dependent-w1.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/T1_MetaD/hills/plumed-reweight-time-dependent-w1.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/T1_MetaD/hills/plumed-reweight-time-dependent-w1.dat.plumed_master.stderr) |  
| [T1_MetaD/plumed.dat](./data/T1_MetaD/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/T1_MetaD/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/T1_MetaD/plumed.dat.plumed_master.stderr) |  
| [T1_MetaD/walker-0/plumed.dat](./data/T1_MetaD/walker-0/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/T1_MetaD/walker-0/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/T1_MetaD/walker-0/plumed.dat.plumed_master.stderr) |  
| [T1_MetaD/walker-1/plumed.dat](./data/T1_MetaD/walker-1/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/T1_MetaD/walker-1/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/T1_MetaD/walker-1/plumed.dat.plumed_master.stderr) |  
  
**Last tested:**  17 Jun 2026, 09:10:39
  
**Project description and instructions**  
Ab initio metadynamics simulations with multiple walkers were performed with CP2K 8.2 package. Further instructions can be found [here](https://github.com/kamtung-tonybill/Nitrate_Photolysis_Aqueous_Solution). 

  
{% raw %}
<b><a href="https://www.plumed.org/doc-master/user-doc/html/actionlist/?actions=UPPER_WALLS,REWEIGHT_METAD,CUSTOM,GROUP,READ,DUMPGRID,FLUSH,RESTART,METAD,HISTOGRAM,PRINT,COORDINATION,DISTANCE" target="_blank">Click here</a> to open manual pages for actions used in this project.</b>
{% endraw %}
**Submission history**  
**[v1]** 04 Apr 2025: original submission  
**[v2]** 16 Jul 2025: updated reference  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:25.009" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:25.009](https://www.plumed-nest.org/eggs/25/009/badge.svg)](https://www.plumed-nest.org/eggs/25/009/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/25/009/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/25/009/badge.svg" alt="plumID:25.009"&gt;&lt;/a&gt;</pre>
  </div>
</div>
