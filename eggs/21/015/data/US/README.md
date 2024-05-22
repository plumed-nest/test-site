# Info for running coarse-grained, umbrella-sampling simulations of CBM binding to a chitin surface. Using CBM5 as an example.

The used sofware versions are:
 - PLUMED v2.5 
 - GROMACS 5.1.4


# To rescale protein-chitin interactions use 

../../scripts/chitin-protein-rescale.py {input-topology} {rescaling} {output-topology}

../../scripts/chitin-protein-rescale.py martini_v3.0.4_chitin.itp 1.10 martini_v3.0.4_chitin_1.10.itp

And change the topology name in the top-file (complex-CBM5_SOL_IONS.top)

After preprocessing (see MetaD folder), the all.top file (cbm5-all.top) contains the right rescaling. 

top=complex-CBM5_SOL_IONS.top
gro=complex-CBM5_SOL_IONS.gro

$gmx grompp -f minimization.mdp -p $top -c $gro -o min.tpr -pp all.top -maxwarn 2



# To run the simulation in GROMACS:

Use the Flow_prepare_all.sh script to generate plumed.dat files and submission scripts for each independent simulation in the US.
The submit\*.sh files can be submitted individually or in batch.


# For post-processing, in the CBM/post_processing folder:

Use the run_wham.sh script.


# To calculate Kd's and make the figures derived from US data in the paper:

Use the Jupyter notebook US-analysis_2.ipynb in the make_figures folder



