# LJ calculation

In this we collected the inputs to run a LJ-38 atoms calculation biasing it with ATLAS.

The inputs for the calculation to be executed in LAMMSP patched with PLUMED are

lj.data
biased.input
plumed\_biased.dat
cluster\_plumed.dat

Teh calculation can be done by running 

```bash
mpirun -np 1 lmp_mpi -i biased.input
```

after that the calculations is finished, the c(t) constant can be evaluated using the python script

```bash
workwon ITRE
python3 itre_reweight.py
```

again we suggested the use of a virtualenvironment in python to use the python reweighting script.

Then the free energy surface can be evaluated using the other python script

```bash
python3 recover_fes.py
```


