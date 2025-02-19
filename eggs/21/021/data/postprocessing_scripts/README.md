# Postprocessing scripts used to generate FES, KL divergence and DeltaF

This folder contains the scripts used to postprocess ATLAS or META calculations and generate the observables.
I reported a use-case for each scripts so to clarify how to use them:

This construct the mono-dimensional FES as a function of the second CV in the TRAJ which contains the colvar. It requires bins so that it can be overlayed to the PT one
```bash
python3 construct_1D_fes.py --colvar TRAJ --col 2 --ct c_t.dat --potential rr.gbias --bins ../bins.dat --fes fes_2.dat --histo histo_2.dat
```

This construct the bi-dimensional FES as a function of the second and third CVs in the TRAJ which contains the colvar. It requires bins so that it can be overlayed to the PT one
```bash
python3 construct_2D_fes.py --cv TRAJ --col 2 3  --ct c_t.dat --potential rr.gbias --bins ../bins.dat --fes fes_2_3.dat --histo histo_2_3.dat
```

This scripts evaluate the FES difference as a function of time between the first cluster in the GMM and all the others. The THETA file contains the PMIs during the trajectory
```bash
python3 get_fes_difference.py --bias rr.gbias --ct c_t.dat --kT 1.0 --theta THETA
```

These two scripts calculate the KL divergence as a function of time during the trajectory. The first evaluate the KL for mono-dimensional distribution and the second for bi-dimensional distribution.
The total\_fes\_X.dat file contains the PT FES evaluate along dimension X and is used as reference. TRAJ contains the colvar. 
```bash
python3 get_KL_1D.py --bins ../bins.dat --data TRAJ --bias rr.gbias --ct c_t.dat --reference ../total_fes_2.dat --out kl_2.dat --column 2
python3 get_KL_2D.py --bins ../bins.dat --data TRAJ --col 2 3  --bias rr.gbias --ct c_t.dat --reference ../total_fes_2_3.dat --out kl_2_3.dat
```

These files are generated for one trajectory. If we need to average them, in case we have multiple trajectory, we can ues the following scripts. The use is self explanatory.

```bash
python3 average_quantity.py -d list_dir -f fes_diff_min_1_2.dat -o fes_diff_min_1_2.dat
python3 average_quantity.py -d list_dir -f kl_2.dat -o kl_2.dat
python3 average_quantity.py -d list_dir -f kl_2_3.dat -o kl_2_3.dat
python3 average_fes.py -d list_dir -f fes_2.dat -o average_fes_2.dat
python3 average_fes_2D.py -d list_dir -f fes_2_3.dat -o average_fes_2_3.dat
```
