# CMP PLUMED-NEST

This repository has the necessary code to run annealing and umbrella simulations of collagen-mimetic peptoids. Files are organized as follows:

Annealing Folder:
1.  npt.gro and topol.top: initial structure and topology files
2.  gen_plumed.py: Code generating PLUMED files to track CVs   
3.  npt_run.mdp: molecular dynamics parameters for annealing   
4.  plumed0.dat: Example PLUMED file    
5.  anneal.sbatch and run_sim.py: code to run the MD

Umbrella Folder:       
1. npt.gro and topol.top: initial structure and topology files
2. torch_tica.pt: PyTorch TICA object
3. make_tica_plumed.py: Code generating TICA object and PLUMED files to bias CVs   
4. umbrella_equil.mdp and umbrella_run.mdp: molecular dynamics parameters for equilibration and umbrella runs, respectively.     
5. plumed.dat: Example PLUMED file
6. run_umbrella.sbatch: code to run the MD
