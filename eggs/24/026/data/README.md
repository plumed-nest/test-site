# CpH-MetaD

## General Information

This page provides access to RNA parameters compatible with the stochastic titration Constant-pH Molecular Dynamics method and the metadynamics version (CpH-MetaD) using PLUMED v2.0 (see https://www.plumed.org/). The parametrization and metadynamics integration was developed in the Bussi Lab group by Tomás F.D. Silva (see: https://www.sissa.it/sbp/members.php?ID=472) and Prof. Giovanni Bussi (see: https://www.sissa.it/sbp/members.php?ID=323). 

The files in the folders are modified to allow compatibility of the st-CpHMD method with RNA and metadynamics. They should replace the already existing ones in the equally named folders in the source code of CpHMD-v3.0 (available on Nuno F.B. Oliveira's GitHub page: https://github.com/NunoFBOliveira/CpHMD_v3).

To perform reweight analysis, we recommend using the WHAM module available on the Bussi Lab GitHub: https://bussilab.github.io/doc-py-bussilab/bussilab/wham.html.
Notebooks and scripts will be available as protonation and conformation analysis templates.

### A tutorial is available here: https://github.com/Tomfersil/CpHMetaD_Tutorial  

## Acknowledgments
We thank Dr. Miguel Machuqueiro and Nuno F.B. Oliveira (see page: https://mms.rd.ciencias.ulisboa.pt/index.html) for access to their CpHMD-V3.0 code and help in this current implementation.

Please cite the original and current versions of the st-CpHMD method and the CpHMD-metadynamics approach papers when using the method:
1) [ArXiv version of the CpH-MetaD paper](https://arxiv.org/abs/2410.16064) ;
2) [Recent st-CpHMD v3.0 paper](https://pubs.acs.org/doi/full/10.1021/acs.jpcb.2c04529) ;
3) [Original st-CpHMD paper](https://doi.org/10.1063/1.1497164) ;


## LOGBOOK

###03/10/2024

  Added necessary parameter and script files to run metadynamics on st-CpHMD and RNA simulations
  
