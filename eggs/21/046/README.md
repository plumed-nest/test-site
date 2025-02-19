**Project ID:** [plumID:21.046]({{ '/' | absolute_url }}eggs/21/046/)  
**Name:**  Ubiquitin Interacting Motifs, Duality Between Structured and Disordered Motifs  
**Archive:** [ https://github.com/ELELAB/disoUIM/raw/main/plumednest/plumednest.zip](https://github.com/ELELAB/disoUIM/raw/main/plumednest/plumednest.zip)  
**Category:**  bio  
**Keywords:**  wt metadynamics, ubiquitin, ataxin-3, short linear motifs, ubiquitin binding motif, moonlight functions, intrinsic disorder  
**PLUMED version:**  2.3  
**Contributor:**  Elena Papaleo  
**Submitted on:** 11 Nov 2021  
**Publication:** [M. Lambrughi, E. Maiani, B. Aykac Fas, G. S. Shaw, B. B. Kragelund, K. Lindorff-Larsen, K. Teilum, G. Invernizzi, E. Papaleo, Ubiquitin Interacting Motifs: Duality Between Structured and Disordered Motifs. Frontiers in Molecular Biosciences. 8 (2021)](http://dx.doi.org/10.3389/fmolb.2021.676235)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [WT-metaD.a032005/plumed2.dat](./data/WT-metaD.a032005/plumed2.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/WT-metaD.a032005/plumed2.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/WT-metaD.a032005/plumed2.dat.plumed_master.stderr) |  
| [WT-metaD.a03ws/plumed2.dat](./data/WT-metaD.a03ws/plumed2.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/WT-metaD.a03ws/plumed2.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/WT-metaD.a03ws/plumed2.dat.plumed_master.stderr) |  
| [WT-metaD.c22star/plumed2.dat](./data/WT-metaD.c22star/plumed2.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/WT-metaD.c22star/plumed2.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/WT-metaD.c22star/plumed2.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:33:24
  
**Project description and instructions**  
Here we include the files to reproduce the WT-metaD simulations associated with the publication [Lambrughi M, Maiani E, Aykac Fas B, Shaw GS, Kragelund BB, Lindorff-Larsen K, Teilum K, Invernizzi G and Papaleo E (2021) Ubiquitin Interacting Motifs. Duality Between Structured and Disordered Motifs. Front. Mol. Biosci. 8 676235](https://www.frontiersin.org/articles/10.3389/fmolb.2021.676235/full). We include the files to reproduce the WT-metaD simulation with i) [Amber ff03w](https://pubs.acs.org/doi/10.1021/jp108618d) force field with the [TIP4P/2005](https://aip.scitation.org/doi/10.1063/1.2121687) (folder WT-metaD.a032005), ii) [Amber ff03ws](https://pubs.acs.org/doi/10.1021/ct500569b) with TIP4P/2005 water model with modified protein–water pair interactions, iii) [CHARMM22star](https://www.cell.com/biophysj/fulltext/S0006-3495(11)00409-7) force field with [TIPS3P](https://pubs.acs.org/doi/10.1021/jp973084f) water model. For each of the three metadynamics included in the publication, we provide the input files (plumed2.dat plumed.dat sim.tpr). The simulations were performed using GROMACS 4.6.2 and PLUMED 1.3. We converted plumed.dat in the formalism of PLUMED 2 in the plumed2.dat and tested it using GROMACS 5.1.2 and PLUMED 2.3.

  
**Submission history**  
**[v1]** 11 Nov 2021: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:21.046" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:21.046](https://www.plumed-nest.org/eggs/21/046/badge.svg)](https://www.plumed-nest.org/eggs/21/046/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/21/046/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/21/046/badge.svg" alt="plumID:21.046"&gt;&lt;/a&gt;</pre>
  </div>
</div>
