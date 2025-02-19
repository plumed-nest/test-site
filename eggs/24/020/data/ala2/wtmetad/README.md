gmx_mpi grompp -f aladip.mdp -p aladip.top -c aladip.gro -o md
gmx_mpi mdrun -deffnm md -ntomp 1 -plumed plumed.dat