gmx_mpi grompp -f md.mdp -p ala3.top -c ala3.gro -o md -maxwarn 10 

gmx_mpi mdrun -deffnm md -ntomp 1 -plumed plumed.dat