# Info for running coarse-grained, metadynamics simulations of CBM binding to a chitin surface. Using CBM5 as an example.

The used sofware versions are:
 - PLUMED v2.5 
 - GROMACS 5.1.4


# To rescale protein-chitin interactions use 

../../scripts/chitin-protein-rescale.py {input-topology} {rescaling} {output-topology}

../../scripts/chitin-protein-rescale.py martini_v3.0.4_chitin.itp 1.10 martini_v3.0.4_chitin_1.10.itp

And change the topology name in the top-file (complex-CBM5_SOL_IONS.top)


# To run the simulation in GROMACS:

gmx=/groups/sbinlab/wyong/usr/local/GMX514/bin/gmx_mpi_plumed
export GMX_ALLOW_CPT_MISMATCH=1
export PLUMED_USE_LEPTON=yes
export PLUMED_KERNEL="/groups/sbinlab/wyong/usr/local/PLUMED250dev_PathCV/lib/libplumedKernel.so"
export LD_LIBRARY_PATH="/groups/sbinlab/wyong/usr/local/PLUMED250dev_PathCV/lib":$LD_LIBRARY_PATH

top=complex-CBM5_SOL_IONS.top
gro=complex-CBM5_SOL_IONS.gro


$gmx grompp -f minimization.mdp -p $top -c $gro -o min.tpr -pp all.top -maxwarn 2
$gmx mdrun -deffnm min -v -ntomp 1


$gmx grompp -f relax.mdp -p all.top -c min.gro -o md1.tpr -n index.ndx -maxwarn 2
$gmx mdrun -deffnm md1 -v -ntomp 8


$gmx grompp -f md.mdp -p all.top -c md1.gro -o md2.tpr -n index.ndx -maxwarn 2
$gmx mdrun -deffnm md2 -v -plumed plumed.dat -ntomp 8

# For post-processing, in the CBM/post_processing folder:

gmx=/groups/sbinlab/wyong/usr/local/GMX2018.2/bin/gmx_mpi_plumed
export GMX_ALLOW_CPT_MISMATCH=1
export PLUMED_USE_LEPTON=yes
export PLUMED_KERNEL="/groups/sbinlab/wyong/usr/local/PLUMED250dev_PathCV/lib/libplumedKernel.so"
export LD_LIBRARY_PATH="/groups/sbinlab/wyong/usr/local/PLUMED250dev_PathCV/lib":$LD_LIBRARY_PATH
plumed=/groups/sbinlab/wyong/usr/local/PLUMED250dev_PathCV/bin/plumed

$gmx trjcat -f ../md2*xtc  -o md_cat.xtc
echo 16 | $gmx trjconv -f md_cat.xtc -s ../md2.tpr -o md_comp.xtc -n ../index.ndx
echo 16 | $gmx trjconv -f ../md1.gro -s ../md2.tpr -o md_comp.gro -n ../index.ndx
rm md_cat.xtc

cp ../HILLS .
cp ../COLVAR .

$plumed driver --mf_xtc md_comp.xtc --plumed calc-weights.dat --timestep 0.02 --trajectory-stride 50000


$plumed driver --mf_xtc md_comp.xtc --plumed coordination-groups.dat --timestep 0.02 --trajectory-stride 50000


python3 ../../../scripts/calc_block_errors.py


rm -r FES_stride
mkdir FES_stride
$plumed sum_hills --hills HILLS --outfile FES_stride/fes- --kt 2.5 --mintozero --stride 1000
n=$(ls FES_stride/* | wc -l)
python2 ../../../scripts/reweight_2_GC.py -bsf 50.0 -kt 2.5 -fpref FES_stride/fes- -nf ${n} -fcol 3 -colvar COLVAR -biascol 4 -rewcol 2 3

# To make the figures derived from MetaD data in the paper:
Extract HILLS.zip and copy output to the make_figures folder
Use the Jupyter notebook make_plots_6.ipynb in the make_figures folder


