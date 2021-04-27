**Project ID:** [plumID:19.060]({{ '/' | absolute_url }}eggs/19/060/)  
**Source:** 3_ala4/simulation/plumed.dat  
**Originally used with PLUMED version:** 2.5-mod  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue">#RESTART</span>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>
phi1: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=5,7,9,15
phi2: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=15,17,19,25
phi3: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=25,27,29,35
psi1: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=7,9,15,17
psi2: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=17,19,25,27
psi3: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=27,29,35,37


<span style="color:blue"># Construct a bias potential using VES</span>
<span style="color:blue">#</span>
<span style="color:blue"># Basis functions</span>


<a href="https://plumed.github.io/doc-master/user-doc/html/_n_n__v_e_s.html">NN_VES</a> ...
<span style="color:blue">#  RESTART_FROM=50000</span>
  TEMP=300.0
  LABEL=bias
  ARG=phi1,phi2,phi3,psi1,psi2,psi3
  NODES=96,48,24
  OPTIM=ADAM
  ACTIVATION=RELU
  GRID_MIN=-pi,-pi,-pi,-pi,-pi,-pi
  GRID_MAX=pi,pi,pi,pi,pi,pi
  GRID_BIN=300,300,300,300,300,300
  AVE_STRIDE=500
  PRINT_STRIDE=100
  TARGET_STRIDE=1
  LRATE=0.001
  GAMMA=10
  TAU_KL=100000
  MODE_DECAY=4
  DECAY_STEP_START=10000
  DECAY=2000
  ADAPTIVE_DECAY=20
  MC_POINTS=20000
  MC_SIGMA=0.5,0.5,0.5,0.5,0.5,0.5
  CALC_MC_ERR=0
  MC_CONVERGENCE_TEST=0
  L2_weight=0.2
  SERIAL
  CALC_RCT
... <a href="https://plumed.github.io/doc-master/user-doc/html/_n_n__v_e_s.html">NN_VES</a>


<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=* STRIDE=100 FILE=COLVAR

</pre>{% endraw %}
