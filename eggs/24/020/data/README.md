The pipeline can be (roughly) splited into the following steps:

(0). Compute distance matrix (i.e., edge feature) with plumed driver. 'plumed driver --ixyz dir_to_traj --plumed plumed.dat'

1. Convert distance (or other feature) matrix into graph objects using data.py. 

2. Train the model with train.py.

3. Convert the model into torchscipt with jit.py. 

4. Perform metaD simulations with starting files in corresponding directory.  


Details please refer to https://arxiv.org/abs/2409.11843. 