**Project ID:** [plumID:19.056]({{ '/' | absolute_url }}eggs/19/056/)  
**Source:** 4w53/plumed.dat  
**Originally used with PLUMED version:** 2.6-dev  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> LENGTH=A TIME=ps ENERGY=kcal/mol

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_z_e__l_o_s_s.html">MAZE_LOSS</a> ...
  LABEL=l

  PARAMS=1,1,1
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_z_e__l_o_s_s.html">MAZE_LOSS</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_z_e__s_i_m_u_l_a_t_e_d__a_n_n_e_a_l_i_n_g.html">MAZE_SIMULATED_ANNEALING</a> ...
  LABEL=opt
  
  LOSS=l
  
  N_ITER=1000
  OPTIMIZER_STRIDE=250000 <span style="color:blue"># 1 ns</span>

  PROBABILITY_DECREASER=300
  COOLING=0.95
  COOLING_SCHEME=geometric  
   
  LIGAND=2635-2649
  PROTEIN=1-2634

  NLIST
  NL_CUTOFF=7
  NL_STRIDE=100
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_z_e__s_i_m_u_l_a_t_e_d__a_n_n_e_a_l_i_n_g.html">MAZE_SIMULATED_ANNEALING</a>

p: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_o_s_i_t_i_o_n.html">POSITION</a> ATOM=2635 NOPBC

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_z_e__o_p_t_i_m_i_z_e_r__b_i_a_s.html">MAZE_OPTIMIZER_BIAS</a> ...
  LABEL=b  

  ARG=p.x,p.y,p.z

  BIASING_RATE=0.02
  ALPHA=3.6
  OPTIMIZER=opt
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_z_e__o_p_t_i_m_i_z_e_r__b_i_a_s.html">MAZE_OPTIMIZER_BIAS</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ...
  ARG=opt.loss,opt.sr,b.bias,b.force2,b.tdist
  STRIDE=500
  FILE=colvar
  FMT=%15.8f 
... <a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a>
</pre>{% endraw %}
