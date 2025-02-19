**Project ID:** [plumID:20.033]({{ '/' | absolute_url }}eggs/20/033/)  
**Name:**  COVID-19 Spike protein opening transition mechanism  
**Archive:** [ https://github.com/vendruscolo-lab/Spike-OpeningTransitionEnsemble/raw/main/SpikeInput.zip](https://github.com/vendruscolo-lab/Spike-OpeningTransitionEnsemble/raw/main/SpikeInput.zip)  
**Category:**  bio  
**Keywords:**  EMMI, CryoEM, COVID-19, Spike, Metainference  
**PLUMED version:**  2.6  
**Contributor:**  Faidon Brotzakis  
**Submitted on:** 25 Nov 2020  
**Last revised:** 04 Aug 2021  
**Publication:** [Z. F. Brotzakis, T. Löhr, M. Vendruscolo, Determination of intermediate state structures in the opening pathway of SARS-CoV-2 spike using cryo-electron microscopy. Chemical Science. 12, 9168–9175 (2021)](http://dx.doi.org/10.1039/D1SC00244A)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [ANALYSIS/plumed_histogram.dat](./data/ANALYSIS/plumed_histogram.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/ANALYSIS/plumed_histogram.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/ANALYSIS/plumed_histogram.dat.plumed_master.stderr) |  
| [PRODUCTION/plumed.dat](./data/PRODUCTION/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-failed-red.svg)](data/PRODUCTION/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/PRODUCTION/plumed.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:38:29
  
**Project description and instructions**  
The deposited input files contain the following directories. 1) The "TOPO_MDP" directory containing the GROMACS topology and parameter files. 2) The "PRODUCTION" directory containing the plumed input file for EMMI and the associated companion files such as an index file, data GMM file (SARS_COV2.dat) and pdb files for the definition of the CVs. 3) The "ANALYSIS" directory containing the plumed histogram file to project the 2D FES using the equilibrated trajectory data COLVAR_final of the EMMI simulations. More information can be found [here](https://github.com/vendruscolo-lab/Spike-OpeningTransitionEnsemble). GROMACS 2018.6 double precision patched with PLUMED 2.6.0-dev was used.

  
**Submission history**  
**[v1]** 25 Nov 2020: original submission  
**[v2]** 04 Aug 2021: updated doi  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:20.033" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:20.033](https://www.plumed-nest.org/eggs/20/033/badge.svg)](https://www.plumed-nest.org/eggs/20/033/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/20/033/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/20/033/badge.svg" alt="plumID:20.033"&gt;&lt;/a&gt;</pre>
  </div>
</div>
