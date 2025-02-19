**Project ID:** [plumID:22.032]({{ '/' | absolute_url }}eggs/22/032/)  
**Name:**  Reciprocal barrier restraint. Application to path-meta-eABF  
**Archive:** [ https://zenodo.org/record/7030287/files/CRL-VHL-degrader-SMARCA2-ring-closure-path-meta-eabf.zip](https://zenodo.org/record/7030287/files/CRL-VHL-degrader-SMARCA2-ring-closure-path-meta-eabf.zip)  
**Category:**  methods  
**Keywords:**  restraint, upper wall, lower wall, path colvar, meta-eABF, metadynamics, DRR, protein conformational transition, PROTAC  
**PLUMED version:**  2.7  
**Contributor:**  Istvan Kolossvary  
**Submitted on:** 29 Aug 2022  
**Publication:** [I. Kolossváry, W. Sherman, Comprehensive Approach to Simulating Large Scale Conformational Changes in Biological Systems Utilizing a Path Collective Variable and New Barrier Restraint. The Journal of Physical Chemistry B. 127, 5214–5229 (2023)](http://dx.doi.org/10.1021/acs.jpcb.3c02028)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [plumed.dat](./data/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/plumed.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:25:56
  
**Project description and instructions**  
To run this simulation you need OpenMM 7.6 or newer and the OpenMM-PLUMED plugin installed. To start the job run the following command line `python run_path-meta-eabf.py n_steps do_relax do_plumed`. For example, `python run_path-meta-eabf.py 50000 1 0` will minimize the system and run 50,000 steps of MD relaxation while `python run_path-meta-eabf.py 5000000 0 1` will read the checkpoint file and continue 5 million steps of meta-eABF simulation using the path colvar representing the opening and closing of the full CRL-VHL-degrader-SMARCA2 ring complex. NOTE. The current implementation of the PATHMSD action has a flaw that results in numerical instability due to computing `exp(-lambda*(it.distance))` with very large lambda values, without scaling. I highly recommend to make the following simple edit to `PathMSDBase.cpp` to introduce proper scaling, as follows.     ``` $ diff PathMSDBase.cpp PathMSDBase.cpp-orig    275d274    < double min_distance=1e10;      281,285c280     < if(it.distance < min_distance) min_distance=it.distance;      < }     <      < for(auto & it : imgVec) {     < it.similarity=exp(-lambda*(it.distance - min_distance));      ---      > it.similarity=exp(-lambda*(it.distance));     293c288       < val_z_path->set(-(1./lambda)*std::log(partition) +min_distance);     ---      > val_z_path->set(-(1./lambda)*std::log(partition));      ```

  
**Submission history**  
**[v1]** 29 Aug 2022: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:22.032" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:22.032](https://www.plumed-nest.org/eggs/22/032/badge.svg)](https://www.plumed-nest.org/eggs/22/032/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/22/032/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/22/032/badge.svg" alt="plumID:22.032"&gt;&lt;/a&gt;</pre>
  </div>
</div>
