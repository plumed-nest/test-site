**Project ID:** [plumID:20.015]({{ '/' | absolute_url }}eggs/20/015/)  
**Name:**  Rational design of ASCT2 inhibitors using an integrated experimental-computational approach  
**Archive:** [ https://github.com/COSBlab/EMMI-ASCT2/archive/main.zip](https://github.com/COSBlab/EMMI-ASCT2/archive/main.zip) [(browse)](https://github.com/COSBlab/EMMI-ASCT2/tree/main)  
**Category:**  bio  
**Keywords:**  ASCT2 transporter, small-molecules, cryo-EM, metainference  
**PLUMED version:**  2.6-dev  
**Contributor:**  Max Bonomi  
**Submitted on:** 20 May 2020  
**Last revised:** 09 Dec 2021  
**Publication:** [R.-A. A. Garibsingh, E. Ndaru, A. A. Garaeva, Y. Shi, L. Zielewicz, P. Zakrepine, M. Bonomi, D. J. Slotboom, C. Paulino, C. Grewer, A. Schlessinger, Rational design of ASCT2 inhibitors using an integrated experimental-computational approach. Proceedings of the National Academy of Sciences. 118 (2021)](http://dx.doi.org/10.1073/pnas.2104093118)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [2-EMMI/plumed.dat](./data/2-EMMI/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-failed-red.svg)](data/2-EMMI/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/2-EMMI/plumed.dat.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
| [3-ANALYSIS/3.1-ASSEMBLE-XTC/plumed_driver.dat](./data/3-ANALYSIS/3.1-ASSEMBLE-XTC/plumed_driver.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/3-ANALYSIS/3.1-ASSEMBLE-XTC/plumed_driver.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/3-ANALYSIS/3.1-ASSEMBLE-XTC/plumed_driver.dat.plumed_master.stderr) [![with LOAD](https://img.shields.io/badge/with-LOAD-yellow.svg)]({{ "/" | absolute_url }}badges) |  
  
**Last tested:**  19 Feb 2025, 14:49:32
  
**Project description and instructions**  
This egg contains the GROMACS topology files (0-TOPO), input files for equilibration (1-EQUIL), and production scripts (2-EMMI) to model conformational ensembles of ASCT2 from cryo-EM data. All the analysis programs and scripts are contained in the directory 3-ANALYSIS. The final models are contained in 4-PDBs. Detailed instructions of the procedure to follow can be found in each directory. PLUMED [GitHub ISDB branch](https://github.com/plumed/plumed2/tree/isdb) and GROMACS 2019.6 were used. 

  
**Submission history**  
**[v1]** 20 May 2020: original submission  
**[v2]** 20 May 2021: updated path and title  
**[v3]** 09 Dec 2021: updated doi  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:20.015" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:20.015](https://www.plumed-nest.org/eggs/20/015/badge.svg)](https://www.plumed-nest.org/eggs/20/015/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/20/015/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/20/015/badge.svg" alt="plumID:20.015"&gt;&lt;/a&gt;</pre>
  </div>
</div>
