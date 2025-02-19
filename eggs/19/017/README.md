**Project ID:** [plumID:19.017]({{ '/' | absolute_url }}eggs/19/017/)  
**Name:**  Ligand binding pathways exploration  
**Archive:** [ https://github.com/riccardocapelli/papers_data/raw/master/pathway_search2019/input_data.zip](https://github.com/riccardocapelli/papers_data/raw/master/pathway_search2019/input_data.zip)  
**Category:**  bio  
**Keywords:**  metadynamics, ligand binding  
**PLUMED version:**  2.5  
**Contributor:**  Riccardo Capelli  
**Submitted on:** 23 Apr 2019  
**Last revised:** 17 Jun 2019  
**Publication:** [R. Capelli, P. Carloni, M. Parrinello, Exhaustive Search of Ligand Binding Pathways via Volume-Based Metadynamics. The Journal of Physical Chemistry Letters. 10, 3495–3499 (2019)](http://dx.doi.org/10.1021/acs.jpclett.9b01183)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [plumed_metad/metad_20ang.dat](./data/plumed_metad/metad_20ang.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed_metad/metad_20ang.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed_metad/metad_20ang.dat.plumed_master.stderr) |  
| [plumed_metad/metad_22ang.dat](./data/plumed_metad/metad_22ang.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed_metad/metad_22ang.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed_metad/metad_22ang.dat.plumed_master.stderr) |  
| [plumed_metad/metad_24ang.dat](./data/plumed_metad/metad_24ang.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed_metad/metad_24ang.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed_metad/metad_24ang.dat.plumed_master.stderr) |  
| [plumed_metad/metad_26ang.dat](./data/plumed_metad/metad_26ang.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed_metad/metad_26ang.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed_metad/metad_26ang.dat.plumed_master.stderr) |  
| [plumed_metad/metad_28ang.dat](./data/plumed_metad/metad_28ang.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed_metad/metad_28ang.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed_metad/metad_28ang.dat.plumed_master.stderr) |  
| [plumed_reweight/reweight_rho_c.dat](./data/plumed_reweight/reweight_rho_c.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed_reweight/reweight_rho_c.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/plumed_reweight/reweight_rho_c.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:35:36
  
**Project description and instructions**  
The data are in three different folders: * input, which contains the GROMACS (2016.5) input files (gro, top, itp, and mdp) to run the MD simulation. * plumed_metad, which contains the PLUMED input file to perform volume-based metadynamics with different restraining potential size * plumed_reweight, which contains the PLUMED reweighing input file.

  
**Submission history**  
**[v1]** 23 Apr 2019: original submission  
**[v2]** 24 Apr 2019: corrected paths for input files (ndx, pdb, dat), example data files added for the reweighting procedure  
**[v3]** 17 Jun 2019: doi added  
  
**Acknowledgement**  
For the Nature Methods paper by the PLUMED consortium ([Nat. Methods 16, 670–673, 2019](https://doi.org/10.1038/s41592-019-0506-8)), Paolo Carloni acknowledges funding by the Deutsche Forschungsgemeinschaft- FOR 2518 DynIon project P6, and, along with Riccardo Capelli, the Human Brain Project.
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:19.017" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:19.017](https://www.plumed-nest.org/eggs/19/017/badge.svg)](https://www.plumed-nest.org/eggs/19/017/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/19/017/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/19/017/badge.svg" alt="plumID:19.017"&gt;&lt;/a&gt;</pre>
  </div>
</div>
