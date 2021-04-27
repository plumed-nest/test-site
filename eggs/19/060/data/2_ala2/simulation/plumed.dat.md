**Project ID:** [plumID:19.060]({{ '/' | absolute_url }}eggs/19/060/)  
**Source:** 2_ala2/simulation/plumed.dat  
**Originally used with PLUMED version:** 2.5-mod  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># set up two variables for Phi and Psi dihedral angles </span>
phi: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=5,7,9,15
psi: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=7,9,15,17
<span style="color:blue"># nn bias</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_n_n__v_e_s.html">NN_VES</a> ...
LABEL=nn
ARG=phi 
NODES=48,24,12 
OPTIM=ADAM
ACTIVATION=RELU
GRID_MIN=-pi 
GRID_MAX=pi 
GRID_BIN=50 
TEMP=300.
AVE_STRIDE=500
PRINT_STRIDE=1000 
TARGET_STRIDE=1 
GAMMA=10
LRATE=0.001 
TAU_KL=10000
DECAY=1000
ADAPTIVE_DECAY=0.5
... <a href="https://plumed.github.io/doc-master/user-doc/html/_n_n__v_e_s.html">NN_VES</a>
<span style="color:blue"># monitor the two variables and the metadynamics bias potential</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=500 ARG=* FILE=COLVAR FMT=%10.8f

</pre>{% endraw %}
