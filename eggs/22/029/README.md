**Project ID:** [plumID:22.029]({{ '/' | absolute_url }}eggs/22/029/)  
**Name:**  Angiotensin-1-7_Metadynamics  
**Archive:** [ https://github.com/AmericaChi/Angiotensin-1-7_Metadynamics/archive/refs/heads/main.zip](https://github.com/AmericaChi/Angiotensin-1-7_Metadynamics/archive/refs/heads/main.zip)  
**Category:**  bio  
**Keywords:**  Metadynamics, Angiotensin-(1-7), peptide  
**PLUMED version:**  2.5  
**Contributor:**  L.-América Chi  
**Submitted on:** 21 Jun 2022  
**Publication:** [L. A. Chi, S. Asgharpour, J. Correa-Basurto, C. R. Bandala, M. Martínez-Archundia, Unveiling the G4-PAMAM capacity to bind and protect Ang-(1-7) bioactive peptide by molecular dynamics simulations. Journal of Computer-Aided Molecular Design. 36, 653–675 (2022)](http://dx.doi.org/10.1007/s10822-022-00470-5)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [metad.dat](./data/metad.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/metad.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/metad.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:32:51
  
**Project description and instructions**  
These scripts can be used to run  Metadynamics simulation of Angiotensin-(1-7) vasoactive peptide in order to explore its conformational landscape in solution at neutral pH. Collective variables are a kind of HBs and gyration radius. If useful for your project, please cite this [preprint](https://doi.org/10.1101/2022.05.23.493150). Call via `bash run.sh`. This script needs md.tpr, index_metad2.ndx and metad.dat files in the root directory. md.tpr should be created in its corresponding GROMACS version by using .itr, .top, .mdp and .pdb files. Force field used can be found here as a .zip file. FF reference [Horta, B. A., et al (2016). A GROMOS-compatible force field for small organic molecules in the condensed phase The 2016H66 parameter set. J. Chem. Theory Comput. 2016, 12, 8, 3825–3850](https://doi.org/10.1021/acs.jctc.6b00187). Scripts require a proper GROMACS patched with PLUMED installed. This simulations were run on a GROMACS 2016.5 and PLUMED Version 2.5.0.

  
**Submission history**  
**[v1]** 21 Jun 2022: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:22.029" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:22.029](https://www.plumed-nest.org/eggs/22/029/badge.svg)](https://www.plumed-nest.org/eggs/22/029/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/22/029/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/22/029/badge.svg" alt="plumID:22.029"&gt;&lt;/a&gt;</pre>
  </div>
</div>
