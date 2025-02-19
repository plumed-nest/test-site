**Project ID:** [plumID:22.033]({{ '/' | absolute_url }}eggs/22/033/)  
**Name:**  Reciprocal barrier restraint. Application to PROTAC passive permeability prediction  
**Archive:** [ https://zenodo.org/record/7030401/files/protac2-permeability-meta-eabf.zip](https://zenodo.org/record/7030401/files/protac2-permeability-meta-eabf.zip)  
**Category:**  methods  
**Keywords:**  PROTAC, membrane permeability, PMF, restraint, meta-eABF, metadynamics, DRR  
**PLUMED version:**  2.7  
**Contributor:**  Istvan Kolossvary  
**Submitted on:** 29 Aug 2022  
**Publication:** [I. Kolossváry, W. Sherman, Comprehensive Approach to Simulating Large Scale Conformational Changes in Biological Systems Utilizing a Path Collective Variable and New Barrier Restraint. The Journal of Physical Chemistry B. 127, 5214–5229 (2023)](http://dx.doi.org/10.1021/acs.jpcb.3c02028)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [plumed.dat](./data/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:31:17
  
**Project description and instructions**  
To run this simulation you need OpenMM 7.6 or newer and the OpenMM-PLUMED plugin installed. To start the job run the following command line. `python run_protac-permeab-meta-eabf.py n_steps do_relax do_plumed`. For example, `python run_protac-permeab-meta-eabf.py 50000 1 0` will minimize the system and run 50,000 steps of MD relaxation while `python run_protac-permeab-meta-eabf.py 5000000 0 1` will read the checkpoint file and continue 5 million steps of meta-eABF simulation. The collective variable is the normalized and periodic Z coordinate of the center of mass (COM) of the PROTAC2 molecule within the domain -0.5, 0.5 where the floating origin of the coordinate system corresponds to the COM of the membrane.NOTES. (1) The COM of the membrane should be computed via the PHASES keyword, the traditional calculation gives highly inaccurate results. (2) We found it beneficial to delay the meta-eABF bias significantly by setting FULLSAMPLES=200000 in the DRR action.  

  
**Submission history**  
**[v1]** 29 Aug 2022: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:22.033" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:22.033](https://www.plumed-nest.org/eggs/22/033/badge.svg)](https://www.plumed-nest.org/eggs/22/033/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/22/033/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/22/033/badge.svg" alt="plumID:22.033"&gt;&lt;/a&gt;</pre>
  </div>
</div>
