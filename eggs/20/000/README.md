**Project ID:** [plumID:20.000]({{ '/' | absolute_url }}eggs/20/000/)  
**Name:**  Muscarinic M2 receptor-ligand funnel metadynamics  
**Archive:** [ https://github.com/riccardocapelli/papers_data/raw/master/muscarinic_m2_2019/input_data.zip](https://github.com/riccardocapelli/papers_data/raw/master/muscarinic_m2_2019/input_data.zip)  
**Category:**  bio  
**Keywords:**  multiple walker metadynamics, well-tempered metadynamics, funnel metadynamics, MC-HLDA, GPCR, receptor, Adiabatic Bias MD  
**PLUMED version:**  2.5  
**Contributor:**  Riccardo Capelli  
**Submitted on:** 03 Feb 2020  
**Publication:** [R. Capelli, A. Bochicchio, G. Piccini, R. Casasnovas, P. Carloni, M. Parrinello, Chasing the Full Free Energy Landscape of Neuroreceptor/Ligand Unbinding by Metadynamics Simulations. Journal of Chemical Theory and Computation. 15, 3354–3361 (2019)](http://dx.doi.org/10.1021/acs.jctc.9b00118)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [ratchet/rMD_plumed.dat](./data/ratchet/rMD_plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/ratchet/rMD_plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/ratchet/rMD_plumed.dat.plumed_master.stderr) |  
| [funnel_metad/funnel_metad_plumed.dat](./data/funnel_metad/funnel_metad_plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/funnel_metad/funnel_metad_plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/funnel_metad/funnel_metad_plumed.dat.plumed_master.stderr) |  
| [reweighting/reweighting.dat](./data/reweighting/reweighting.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/reweighting/reweighting.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/reweighting/reweighting.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:43:03
  
**Project description and instructions**  
This egg contains (I) the structure and input files for the M2 muscarinic receptor with iperoxo (input folder), (II) the plumed file for Ratcheted MD (ratcheted folder), (III) the plumed file for funnel metadynamics (funnel_metad folder), and (IV) the input file for the reweighting procedure.

  
**Submission history**  
**[v1]** 03 Feb 2020: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:20.000" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:20.000](https://www.plumed-nest.org/eggs/20/000/badge.svg)](https://www.plumed-nest.org/eggs/20/000/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/20/000/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/20/000/badge.svg" alt="plumID:20.000"&gt;&lt;/a&gt;</pre>
  </div>
</div>
