**Project ID:** [plumID:23.032]({{ '/' | absolute_url }}eggs/23/032/)  
**Name:**  Acceleration of Molecular Simulations by Parametric Time-Lagged tSNE Metadynamics  
**Archive:** [ https://zenodo.org/record/8246298/files/ptltsne_nest.zip](https://zenodo.org/record/8246298/files/ptltsne_nest.zip)  
**Category:**  bio  
**Keywords:**  metadynamics, tSNE, neural network, machine learning, trp-cage, folding  
**PLUMED version:**  2.9  
**Contributor:**  Vojtech Spiwok  
**Submitted on:** 14 Aug 2023  
**Publication:** [H. Hradiská, M. Kurečka, J. Beránek, G. Tedeschi, V. Višňovský, A. Křenek, V. Spiwok, Acceleration of Molecular Simulations by Parametric Time-Lagged tSNE Metadynamics. The Journal of Physical Chemistry B. 128, 903–913 (2024)](http://dx.doi.org/10.1021/acs.jpcb.3c05669)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [mtd1/plumed.dat](./data/mtd1/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/mtd1/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/mtd1/plumed.dat.plumed_master.stderr) |  
| [mtd2/plumed.dat](./data/mtd2/plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/mtd2/plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/mtd2/plumed.dat.plumed_master.stderr) |  
| [pt/plumedpt.dat](./data/pt/plumedpt.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-failed-red.svg)](data/pt/plumedpt.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/pt/plumedpt.dat.plumed_master.stderr) |  
| [ptmtd/plumedpt.dat](./data/ptmtd/plumedpt.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-failed-red.svg)](data/ptmtd/plumedpt.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-failed-red.svg)](data/ptmtd/plumedpt.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:32:45
  
**Project description and instructions**  
Data for metadynamics with two parametric time-lagged tSNE collective variables are in the mtd1 directory. Data for metadynamics with two parametric time-lagged tSNE collective variables and alphaRMSD are in the mtd2 directory. Data for parallel tempering metadynamics with two parametric time-lagged tSNE collective variables are in the ptmtd directory. Data for reference parallel tempering simulations are in the pt directory. The results were obtained using Gromacs (2021.4, 2021), Plumed (2.8.0, 2.9.0) and other codes available [here](https://github.com/spiwokv/ptltsne) and [here](https://github.com/kurecka/plumed2/tree/uvt_extensions).
  
**Submission history**  
**[v1]** 14 Aug 2023: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:23.032" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:23.032](https://www.plumed-nest.org/eggs/23/032/badge.svg)](https://www.plumed-nest.org/eggs/23/032/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/23/032/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/23/032/badge.svg" alt="plumID:23.032"&gt;&lt;/a&gt;</pre>
  </div>
</div>
