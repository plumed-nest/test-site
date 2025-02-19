**Project ID:** [plumID:19.031]({{ '/' | absolute_url }}eggs/19/031/)  
**Name:**  Ice nucleation using PIV-based path coordinates  
**Archive:** [ https://github.com/physix-repo/plumed_input_nucleation/raw/main/plumed-input-nucleation.zip](https://github.com/physix-repo/plumed_input_nucleation/raw/main/plumed-input-nucleation.zip)  
**Category:**  materials  
**Keywords:**  phase transitions, nucleation, TIP4P, path CV, PIV, metadynamics  
**PLUMED version:**  2.5-dev  
**Contributor:**  Silvio Pipolo  
**Submitted on:** 06 May 2019  
**Publication:** [S. Pipolo, M. Salanne, G. Ferlat, S. Klotz, A. M. Saitta, F. Pietrucci, Navigating at Will on the Water Phase Diagram. Physical Review Letters. 119 (2017)](http://dx.doi.org/10.1103/PhysRevLett.119.245701)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [plumed.dat](./data/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:53:22
  
**Project description and instructions**  
The input files provided were used in [Phys. Rev. Lett. 119, 245701 (2017)](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.119.245701) to simulate the nucleation of ice from liquid water, using the TIP4P/2005 potential and GROMACS as MD engine. Two reference pdb files are needed, providing the endpoints of the transition. PLUMED must be compiled including the PIV module (configure --enable-modules=piv). 

  
**Submission history**  
**[v1]** 06 May 2019: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:19.031" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:19.031](https://www.plumed-nest.org/eggs/19/031/badge.svg)](https://www.plumed-nest.org/eggs/19/031/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/19/031/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/19/031/badge.svg" alt="plumID:19.031"&gt;&lt;/a&gt;</pre>
  </div>
</div>
