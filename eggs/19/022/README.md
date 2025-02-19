**Project ID:** [plumID:19.022]({{ '/' | absolute_url }}eggs/19/022/)  
**Name:**  eABF simulation of NANMA (alanine dipeptide)  
**Archive:** [ https://github.com/HanatoK/eABF_plumed_examples/raw/master/eABF_NANMA_gmx.zip](https://github.com/HanatoK/eABF_plumed_examples/raw/master/eABF_NANMA_gmx.zip)  
**Category:**  methods  
**Keywords:**  eABF, DRR, alanine dipeptide  
**PLUMED version:**  2.4  
**Contributor:**  Haochuan Chen  
**Submitted on:** 30 Apr 2019  
**Publication:** [H. Chen, H. Fu, X. Shao, C. Chipot, W. Cai, ELF: An Extended-Lagrangian Free Energy Calculation Module for Multiple Molecular Dynamics Engines. Journal of Chemical Information and Modeling. 58, 1315–1318 (2018)](http://dx.doi.org/10.1021/acs.jcim.8b00115)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [plumed.dat](./data/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:54:26
  
**Project description and instructions**  
The software used is GROMACS version >2018.6. Assuming GROMACS is installed as /usr/local/gromacs/bin/gmx and compiled with PLUMED support, you can run: `/usr/local/gromacs/bin/gmx mdrun -ntomp 8 -s ./alad_600ns.tpr -plumed ./plumed.dat&` After the simulation, you can extract the gradients from the .drrstate file using `plumed drr_tool --extract ./alad.drrstate -v` and then integrate the alad.czar.grad file by abf_integrate alad.czar.grad The abf_integrate program can be found at [here](https://github.com/Colvars/colvars/tree/master) 

  
**Submission history**  
**[v1]** 30 Apr 2019: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:19.022" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:19.022](https://www.plumed-nest.org/eggs/19/022/badge.svg)](https://www.plumed-nest.org/eggs/19/022/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/19/022/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/19/022/badge.svg" alt="plumID:19.022"&gt;&lt;/a&gt;</pre>
  </div>
</div>
