**Project ID:** [plumID:19.080]({{ '/' | absolute_url }}eggs/19/080/)  
**Source:** h3/fes/plumed.inp  
**Originally used with PLUMED version:** 2.4.1  
**Stable:** [raw zipped stdout](plumed.inp.plumed.stdout.txt.zip) - [stderr](plumed.inp.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.inp.plumed_master.stdout.txt.zip) - [stderr](plumed.inp.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> LENGTH=A TIME=fs ENERGY=kcal/mol

<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1,2 LABEL=d1
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=2,3 LABEL=d2
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1,3 LABEL=d3

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2 COEFFICIENTS=1.0,-1.0 PERIODIC=NO LABEL=cv
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d3 COEFFICIENTS=-1.0,1.0 PERIODIC=NO LABEL=block1
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d2,d3 COEFFICIENTS=-1.0,1.0 PERIODIC=NO LABEL=block2

<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=d1,d2 AT=2.5,2.5 KAPPA=100.0,100.0 LABEL=constrain
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=block1,block2 AT=0.0,0.0 KAPPA=1000.0,1000.0 LABEL=cone
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_x_t_e_r_n_a_l.html">EXTERNAL</a> ARG=d1 FILE=extbias1 LABEL=external1
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_x_t_e_r_n_a_l.html">EXTERNAL</a> ARG=d2 FILE=extbias2 LABEL=external2

bf1: <a href="https://plumed.github.io/doc-master/user-doc/html/_b_f__c_h_e_b_y_s_h_e_v.html">BF_CHEBYSHEV</a> MINIMUM=-2.5 MAXIMUM=2.5 ORDER=48

td: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_d__w_e_l_l_t_e_m_p_e_r_e_d.html">TD_WELLTEMPERED</a> BIASFACTOR=30

<span style="color:blue"># Expansion</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_v_e_s__l_i_n_e_a_r__e_x_p_a_n_s_i_o_n.html">VES_LINEAR_EXPANSION</a> ...
 ARG=cv
 BASIS_FUNCTIONS=bf1
 TEMP=300
 GRID_BINS=1000
 TARGET_DISTRIBUTION=td
 LABEL=b1
... <a href="https://plumed.github.io/doc-master/user-doc/html/_v_e_s__l_i_n_e_a_r__e_x_p_a_n_s_i_o_n.html">VES_LINEAR_EXPANSION</a>

<span style="color:blue"># Optimization algorithm</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_t__a_v_e_r_a_g_e_d__s_g_d.html">OPT_AVERAGED_SGD</a> ...
  BIAS=b1
  STRIDE=50000
  LABEL=o1
  STEPSIZE=0.25
  FES_OUTPUT=10
  BIAS_OUTPUT=1000
  COEFFS_OUTPUT=1
  TARGETDIST_STRIDE=5
... <a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_t__a_v_e_r_a_g_e_d__s_g_d.html">OPT_AVERAGED_SGD</a>


<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=d1,d2,cv,b1.bias STRIDE=10000 FILE=colvar

</pre>{% endraw %}
