**Project ID:** [plumID:19.060]({{ '/' | absolute_url }}eggs/19/060/)  
**Source:** 1_wolfe_quapp_potential/single_replica/inputs/plumed.dat  
**Originally used with PLUMED version:** 2.5-mod  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> NATURAL

p: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_o_s_i_t_i_o_n.html">POSITION</a> ATOM=1

ene: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a>
<span style="color:blue"># nn bias</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_n_n__v_e_s.html">NN_VES</a> ...
LABEL=nn
ARG=p.x
NODES=48,24,12 
OPTIM=ADAM
ACTIVATION=RELU
GRID_MIN=-3. 
GRID_MAX=3.
GRID_BIN=50 
TEMP=1.
AVE_STRIDE=500 
PRINT_STRIDE=1000 
TARGET_STRIDE=1
GAMMA=10
LRATE=0.001
TAU_KL=50000
DECAY=5000
ADAPTIVE_DECAY=0.5
... <a href="https://plumed.github.io/doc-master/user-doc/html/_n_n__v_e_s.html">NN_VES</a>

<span style="color:blue"># monitor the two variables and the metadynamics bias potential</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=500 ARG=* FILE=COLVAR FMT=%10.8f
</pre>{% endraw %}
