**Project ID:** [plumID:20.005]({{ '/' | absolute_url }}eggs/20/005/)  
**Name:**  Muscarinic M2 receptor/ligand Frequency-Adaptive Metadynamics and QM/MM calculations  
**Archive:** [ https://github.com/riccardocapelli/papers_data/raw/master/muscarinic_m2_2020/input_data.zip](https://github.com/riccardocapelli/papers_data/raw/master/muscarinic_m2_2020/input_data.zip)  
**Category:**  bio  
**Keywords:**  Frequency-adaptive metadynamics, multiple-walkers metadynamics, well-tempered metadynamics, GPCR, receptor, Adiabatic Bias MD  
**PLUMED version:**  2.5  
**Contributor:**  Riccardo Capelli  
**Submitted on:** 09 Mar 2020  
**Last revised:** 07 Sep 2020  
**Publication:** [R. Capelli, W. Lyu, V. Bolnykh, S. Meloni, J. M. H. Olsen, U. Rothlisberger, M. Parrinello, P. Carloni, Accuracy of Molecular Simulation-Based Predictions of
                    <i>k</i>
                    <sub>off</sub>
                    Values: A Metadynamics Study. The Journal of Physical Chemistry Letters 11, 6373–6381 (2020)](http://dx.doi.org/10.1021/acs.jpclett.0c00999)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [input_data/classical/FA-metaD/FA-MetaD_plumed.dat](./data/input_data/classical/FA-metaD/FA-MetaD_plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/input_data/classical/FA-metaD/FA-MetaD_plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/input_data/classical/FA-metaD/FA-MetaD_plumed.dat.plumed_master.stderr) |  
| [input_data/classical/WT-metaD/WT-MetaD_plumed.dat](./data/input_data/classical/WT-metaD/WT-MetaD_plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/input_data/classical/WT-metaD/WT-MetaD_plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/input_data/classical/WT-metaD/WT-MetaD_plumed.dat.plumed_master.stderr) |  
| [input_data/classical/ratchet/rMD_plumed.dat](./data/input_data/classical/ratchet/rMD_plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/input_data/classical/ratchet/rMD_plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/input_data/classical/ratchet/rMD_plumed.dat.plumed_master.stderr) |  
| [input_data/classical/reweighting/reweighting.dat](./data/input_data/classical/reweighting/reweighting.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-failed-red.svg)](data/input_data/classical/reweighting/reweighting.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/input_data/classical/reweighting/reweighting.dat.plumed_master.stderr) |  
  
**Last tested:**  17 Jun 2026, 09:29:11
  
**Project description and instructions**  
This egg contains the structure and input files for the M2 muscarinic receptor with iperoxo calculations for both classical force field (with GROMACS 2018.6) and QM/MM (GROMACS+CPMD with MiMiC interface), the PLUMED files for Ratcheted MD (ratchet folder), well-tempered metadynamics (WT-MetaD folder), frequency-adaptive metadynamics (FA-MetaD), and reweighting procedure (reweighting).

  
{% raw %}
<b><a href="https://www.plumed.org/doc-master/user-doc/html/actionlist/?actions=ABMD,ENDPLUMED,DISTANCE,FUNCPATHMSD,WHOLEMOLECULES,COMBINE,DUMPGRID,METAD,COM,FLUSH,MOLINFO,LOWER_WALLS,HISTOGRAM,UPPER_WALLS,CONVERT_TO_FES,CONTACTMAP,REWEIGHT_METAD,READ,PRINT" target="_blank">Click here</a> to open manual pages for actions used in this project.</b>
{% endraw %}
**Submission history**  
**[v1]** 09 Mar 2020: original submission  
**[v2]** 23 May 2020: updated doi  
**[v3]** 07 Sep 2020: updated doi  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:20.005" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:20.005](https://www.plumed-nest.org/eggs/20/005/badge.svg)](https://www.plumed-nest.org/eggs/20/005/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/20/005/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/20/005/badge.svg" alt="plumID:20.005"&gt;&lt;/a&gt;</pre>
  </div>
</div>
