input and analysis files for simulations of GGGAGGGAGGGAGGG G4 and GGGAGGG/GGGTTAGGG hairpins

trajectory data will be uploaded to Zenodo soon

Manuscript will be uploaded to biorXiv soon

![](https://github.com/ppokor/G4_folding_parallel/blob/main/folding6_240ns.gif)

**What is here**

MTD.mdp - Gromacs input file with simulation settings

dG_calculation - example script to calculate dG_fold for full G4 and for individual hairpins from the G4 trajectory

lambdas - lambda values for different simulations (12 and 16 replicas)

plumed_inputs - plumed input files for ST-metaD simulations and gHBfix setting files

reference_structures - .pdb files of reference hairpins, crosses, tilted structures, and full G4. For triplex, the first three G-tracts of full G4 were used as a reference

topologies_coord_inpunts - Gromacs .tpr files from which the ST-metaD simulations were initiated. Gromacs topology and Amber topology+coordinate files are also included

example command line input for 1-microsecond Gromacs2021 ST-metaD run with 12 replicas is:

	module load PLUMED/2.7.3-fosscuda-2020b 
	module load GROMACS/2021.4-fosscuda-2020b-PLUMED-2.7.3
	mpirun -np 12 -x CUDA_VISIBLE_DEVICES=0,1,2,3,4,5 --map-by node  gmx_mpi mdrun -pin on -ntomp 8 -nb gpu -v -s MTD -plumed plumed.dat -multidir rep0 rep1 rep2 rep3 rep4 rep5 rep6 rep7 rep8 rep9 rep10 rep11  -replex 2500 -hrex -nsteps 250000000 -cpi state.cpt -noappend

see the manuscript for further details
