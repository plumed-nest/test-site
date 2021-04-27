# Info for running FAMetaD using conformational exchange in Nme-Ala3-Ace as example
For further instructions see also:
https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html

We provide a typical example of the method as described in https://doi.org/10.1063/1.5024679
Users should be able to adopt this to other situations.

The used sofwares are:
 - PLUMED v2.5 
 - GROMACS 2015.4

The example uses an implicit solvent model that may not be well supported in later versions of GROMACS, but if the user wants to run explicit solvent calculations (as per other examples in our paper) this should be feasible with later versions of GROMCAS.

# To run FaMetaD in GROMACS:

top=ala3.amber99sb-tip3p.top

gro=ala3_basinA.gro

export PLUMED_KERNEL=/home/people/wanyong/usr/local/PLUMED251/lib/libplumedKernel.so

export LD_LIBRARY_PATH=/home/people/wanyong/usr/local/PLUMED251/lib:$LD_LIBRARY_PATH

export PLUMED_USE_LEPTON=yes

gmx grompp -f md-implicit.mdp -c $gro -p $top -o md.tpr -maxwarn 2

mpirun -n 8 gmx mdrun -deffnm md -plumed plumed_FaMetaD.dat

