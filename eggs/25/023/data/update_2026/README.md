README – Supporting data and analysis files
===========================================

This archive contains the input files and analysis scripts used in the manuscript:

“In silico assessment of Tau R3–R4 oligomers for elucidating the nucleation seed”
(M. Lauricella et al.)

The content is organized as follows.

----------------------------------------------------------------
analysis/
----------------------------------------------------------------
This directory contains all scripts and notebooks used to analyze
molecular dynamics and metadynamics trajectories and to generate
the figures reported in the manuscript and Supporting Information.

1) QT_cluster_analysis/
   Quality Threshold (QT) clustering analysis of unbiased MD trajectories,
   following Heyer et al. and González-Alemán et al.

   For each oligomeric state (monomer to pentamer), the directory contains:
   - QT.py
     Python script implementing QT clustering using Cα RMSD as a distance metric.
   - select_CA.pdb (or select_ca.pdb)
     Reference structure containing the averaged Cα atoms, used to define
     the RMSD metric and cluster assignment.

   This analysis is used to characterize the conformational heterogeneity
   and population of the most representative clusters (Table 1 and Fig. 1
   of the manuscript).

2) free_energy_reconstruction_convergence/
   Jupyter notebooks used to assess the convergence and statistical
   reliability of free-energy reconstruction.

   For each oligomeric state (monomer to pentamer):
   - analisi.<system>.b2.ipynb

   The trajectory is divided into blocks and the free-energy surface is
   reconstructed independently for each block. The convergence toward a
   single, stable free-energy landscape is analyzed by comparing block-wise
   reconstructions, as discussed in the manuscript and Supporting Information.

3) rewighting_2d_map_rmsd_cshape/
   Files used for reweighting well-tempered metadynamics simulations and
   reconstructing the two-dimensional free-energy maps shown in Figure 2
   of the manuscript.

   For each oligomeric state:
   - plumed.sh
     Shell script to perform PLUMED reweighting.
   - plumed_rew.dat
     PLUMED input file defining the reweighting procedure.
   - prot_ref_*.pdb
     Reference structures used to compute RMSD and C-shape order parameters.

----------------------------------------------------------------
gromacs_top_files/
----------------------------------------------------------------
GROMACS topology files used for the simulations.

For each oligomeric state (monomer to pentamer):
- topol.top

The simulations employ the CHARMM36 all-atom force field and the TIP3P
water model as distributed with GROMACS. No custom force-field parameters
were introduced.

----------------------------------------------------------------
initial_conf_for_relaxing_md/
----------------------------------------------------------------
Initial configurations used as starting points for the unbiased molecular
dynamics (MD) relaxation runs.

For each oligomeric state:
- conf.gro

These structures are used to perform standard MD equilibration and
production runs prior to enhanced-sampling simulations.

----------------------------------------------------------------
initial_relaxed_conf_for_metad/
----------------------------------------------------------------
Initial configurations and PLUMED input files used for well-tempered
metadynamics simulations.

For each oligomeric state:
- conf.gro
  Relaxed structure obtained after unbiased MD.
- plumed.dat
  PLUMED input file defining the collective variables and bias potential
  used in metadynamics.

The PLUMED input files are consistent with those deposited in PLUMED-NEST
(plumID:25.023) and referenced in the manuscript.

----------------------------------------------------------------
Notes
----------------------------------------------------------------
• All analyses were performed using GROMACS and PLUMED versions reported
  in the manuscript.
• Trajectory files (.xtc/.trr) and GROMACS parameter files (.mdp) are not
  included, as they are not required to reproduce the analyses and figures.
• The structure and analysis workflow are fully documented to ensure
  transparency and reproducibility in accordance with ACS and JCIM
  guidelines.

