**Project ID:** [plumID:21.052]({{ '/' | absolute_url }}eggs/21/052/)  
**Name:**  On the Role of Solvent in the Formation of Vacancies on Ibuprofen Crystal Facets  
**Archive:** [ https://github.com/mme-ucl/plumed-nest-data/raw/master/002_input_and_plumed.zip](https://github.com/mme-ucl/plumed-nest-data/raw/master/002_input_and_plumed.zip)  
**Category:**  materials  
**Keywords:**  Ibuprofen, unbinding, WTmetaD  
**PLUMED version:**  2.5  
**Contributor:**  Matteo Salvalaglio  
**Submitted on:** 18 Dec 2021  
**Publication:** [V. Marinova, G. P. F. Wood, I. Marziano, M. Salvalaglio, Investigating the Role of Solvent in the Formation of Vacancies on Ibuprofen Crystal Facets. Crystal Growth &amp; Design. 22, 3034–3041 (2022)](http://dx.doi.org/10.1021/acs.cgd.1c01479)  
  
**PLUMED input files**  
  
| File     | Compatible with |  
|:--------:|:--------:|  
| [002_acetonitrile_plumed.dat](./data/002_acetonitrile_plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/002_acetonitrile_plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/002_acetonitrile_plumed.dat.plumed_master.stderr) |  
| [002_butanol_plumed.dat](./data/002_butanol_plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/002_butanol_plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/002_butanol_plumed.dat.plumed_master.stderr) |  
| [002_cyclohexane_plumed.dat](./data/002_cyclohexane_plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/002_cyclohexane_plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/002_cyclohexane_plumed.dat.plumed_master.stderr) |  
| [002_cyclohexanone_plumed.dat](./data/002_cyclohexanone_plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/002_cyclohexanone_plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/002_cyclohexanone_plumed.dat.plumed_master.stderr) |  
| [002_ethanol_plumed.dat](./data/002_ethanol_plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/002_ethanol_plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/002_ethanol_plumed.dat.plumed_master.stderr) |  
| [002_ethyl-acetate_plumed.dat](./data/002_ethyl-acetate_plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/002_ethyl-acetate_plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/002_ethyl-acetate_plumed.dat.plumed_master.stderr) |  
| [002_hexane_plumed.dat](./data/002_hexane_plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/002_hexane_plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/002_hexane_plumed.dat.plumed_master.stderr) |  
| [002_methanol_plumed.dat](./data/002_methanol_plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/002_methanol_plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/002_methanol_plumed.dat.plumed_master.stderr) |  
| [002_toluene_plumed.dat](./data/002_toluene_plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/002_toluene_plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/002_toluene_plumed.dat.plumed_master.stderr) |  
| [002_trichloromethane_plumed.dat](./data/002_trichloromethane_plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/002_trichloromethane_plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/002_trichloromethane_plumed.dat.plumed_master.stderr) |  
| [002_water_plumed.dat](./data/002_water_plumed.dat.md) |  [![tested on v2.10](https://img.shields.io/badge/v2.10-passing-green.svg)](data/002_water_plumed.dat.plumed.stderr) [![tested on master](https://img.shields.io/badge/master-passing-green.svg)](data/002_water_plumed.dat.plumed_master.stderr) |  
  
**Last tested:**  19 Feb 2025, 14:33:04
  
**Project description and instructions**  
Input structure and plumed files for sampling the formation of a surface vacancy in Ibuprofen crystals, 002 face. Input files for the 011 and 100 faces are available [here](https://github.com/mme-ucl/plumed-nest-data/raw/master/011_input_and_plumed.zip) and [here](https://github.com/mme-ucl/plumed-nest-data/raw/master/100_input_and_plumed.zip), respectively. The MD engine used was GROMACS. See also [plumID:19.069](https://www.plumed-nest.org/eggs/19/069/) and [plumID:19.015](https://www.plumed-nest.org/eggs/19/015/). For MFI, please see [here](https://github.com/mme-ucl/MFI).

  
**Submission history**  
**[v1]** 18 Dec 2021: original submission  
  
**Badge**  
Click on the image below and get the code to add the badge to your website!  
<img src="./badge.svg" alt="plumeDnest:21.052" id="myBtn" class="badge">
<div id="myModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    Markdown<pre>[![plumID:21.052](https://www.plumed-nest.org/eggs/21/052/badge.svg)](https://www.plumed-nest.org/eggs/21/052/)</pre>
    HTML<pre>&lt;a href="https://www.plumed-nest.org/eggs/21/052/"&gt;&lt;img src="https://www.plumed-nest.org/eggs/21/052/badge.svg" alt="plumID:21.052"&gt;&lt;/a&gt;</pre>
  </div>
</div>
