**Project ID:** [plumID:19.080]({{ '/' | absolute_url }}eggs/19/080/)  
**Source:** clch3cl/ch-param/plumed.inp  
**Originally used with PLUMED version:** 2.4.1  
**Stable:** [raw zipped stdout](plumed.inp.plumed.stdout.txt.zip) - [stderr](plumed.inp.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.inp.plumed_master.stdout.txt.zip) - [stderr](plumed.inp.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> LENGTH=A TIME=fs ENERGY=kcal/mol

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=2 GROUPB=3 R_0=1.10 NN=12 LABEL=dis1
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=2 GROUPB=4 R_0=1.10 NN=12 LABEL=dis2
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=2 GROUPB=5 R_0=1.10 NN=12 LABEL=dis3

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=dis1,dis2,dis3 COEFFICIENTS=0.333,0.333,0.333 PERIODIC=NO LABEL=nm

bf1: <a href="https://plumed.github.io/doc-master/user-doc/html/_b_f__c_h_e_b_y_s_h_e_v.html">BF_CHEBYSHEV</a> MINIMUM=0 MAXIMUM=1 ORDER=48

td: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_d__g_r_i_d.html">TD_GRID</a> FILE=histo

<span style="color:blue"># Expansion</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_v_e_s__l_i_n_e_a_r__e_x_p_a_n_s_i_o_n.html">VES_LINEAR_EXPANSION</a> ...
 ARG=nm
 BASIS_FUNCTIONS=bf1
 TEMP=300
 GRID_BINS=500
 TARGET_DISTRIBUTION=td
 LABEL=external
... <a href="https://plumed.github.io/doc-master/user-doc/html/_v_e_s__l_i_n_e_a_r__e_x_p_a_n_s_i_o_n.html">VES_LINEAR_EXPANSION</a>

<span style="color:blue"># Optimization algorithm</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_t__a_v_e_r_a_g_e_d__s_g_d.html">OPT_AVERAGED_SGD</a> ...
  BIAS=external
  STRIDE=2000
  LABEL=o1
  STEPSIZE=0.10
  FES_OUTPUT=1000
  BIAS_OUTPUT=10
  FES_PROJ_OUTPUT=20
  COEFFS_OUTPUT=1
... <a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_t__a_v_e_r_a_g_e_d__s_g_d.html">OPT_AVERAGED_SGD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=400
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=nm,external.bias STRIDE=400 FILE=colvar

</pre>{% endraw %}
