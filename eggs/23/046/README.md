**Project ID:** [plumID:23.046]({{ '/' | absolute_url }}eggs/23/046/)  
**Name:**  Lasso Peptides - HLDA CV  
**Archive:** [ https://github.com/gabedahora/HLDA-WTMetaD-lasso/raw/main/lasso_HLDA.zip](https://github.com/gabedahora/HLDA-WTMetaD-lasso/raw/main/lasso_HLDA.zip)  
**Category:**  bio  
**Keywords:**  metadynamics, protein folding, HLDA, harmonic  
**PLUMED version:**  2.7.1  
**Contributor:**  Gabriel da Hora  
**Submitted on:** 21 Dec 2023  
**Publication:** [G. C. A. da Hora, M. Oh, J. D. M. Nguyen, J. M. J. Swanson, One Descriptor to Fold Them All: Harnessing Intuition and Machine Learning to Identify Transferable Lasso Peptide Reaction Coordinates. The Journal of Physical Chemistry B. 128, 4063–4075 (2024)](http://dx.doi.org/10.1021/acs.jpcb.3c08492)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [github/MccJ25/plumed.dat](./data/github/MccJ25/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/github/MccJ25/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/github/MccJ25/plumed.dat.plumed_master.stderr) |  
| [github/Sun/plumed.dat](./data/github/Sun/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/github/Sun/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/github/Sun/plumed.dat.plumed_master.stderr) |  
| [github/Uln/plumed.dat](./data/github/Uln/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/github/Uln/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/github/Uln/plumed.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:29:49
  
**Project description and instructions**  
These are AMBER and PLUMED files to run Well-Tempered Metadynamics for each lasso peptide (MccJ25, ulleungdin and sungsanpin) with two CVs. One of the CVs biases the isopeptide bond between residues 1 and 8 and the second is defined by HLDA as a combination of weighted distances from the ring 1-8 to the piercing residue.
  
**Submission history**  
**[v1]** 21 Dec 2023: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:23.046" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:23.046](https://www.plumed-nest.org/eggs/23/046/badge.svg)](https://www.plumed-nest.org/eggs/23/046/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/23/046/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/23/046/badge.svg" alt="plumID:23.046"&gt;&lt;/a&gt;</pre>
  </div>
</div>
