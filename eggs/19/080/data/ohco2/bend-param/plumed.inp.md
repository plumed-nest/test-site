**Project ID:** [plumID:19.080]({{ '/' | absolute_url }}eggs/19/080/)  
**Source:** ohco2/bend-param/plumed.inp  
**Originally used with PLUMED version:** 2.4.1  
**Stable:** [raw zipped stdout](plumed.inp.plumed.stdout.txt.zip) - [stderr](plumed.inp.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.inp.plumed_master.stdout.txt.zip) - [stderr](plumed.inp.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> LENGTH=A TIME=fs ENERGY=kcal/mol

<a href="https://plumed.github.io/doc-master/user-doc/html/_a_n_g_l_e.html">ANGLE</a> ATOMS=2,1,3 LABEL=d1

bf1: <a href="https://plumed.github.io/doc-master/user-doc/html/_b_f__c_h_e_b_y_s_h_e_v.html">BF_CHEBYSHEV</a> MINIMUM=pi/2 MAXIMUM=pi ORDER=48

td: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_d__g_r_i_d.html">TD_GRID</a> FILE=histo

<span style="color:blue"># Expansion</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_v_e_s__l_i_n_e_a_r__e_x_p_a_n_s_i_o_n.html">VES_LINEAR_EXPANSION</a> ...
 ARG=d1
 BASIS_FUNCTIONS=bf1
 TEMP=300
 GRID_BINS=500
 TARGET_DISTRIBUTION=td
 LABEL=b1
... <a href="https://plumed.github.io/doc-master/user-doc/html/_v_e_s__l_i_n_e_a_r__e_x_p_a_n_s_i_o_n.html">VES_LINEAR_EXPANSION</a>

<span style="color:blue"># Optimization algorithm</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_t__a_v_e_r_a_g_e_d__s_g_d.html">OPT_AVERAGED_SGD</a> ...
  BIAS=b1
  STRIDE=2000
  LABEL=o1
  STEPSIZE=0.25
  FES_OUTPUT=1000
  BIAS_OUTPUT=10
  FES_PROJ_OUTPUT=20
  COEFFS_OUTPUT=1
... <a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_t__a_v_e_r_a_g_e_d__s_g_d.html">OPT_AVERAGED_SGD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=200
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=d1,b1.bias STRIDE=200 FILE=colvar

</pre>{% endraw %}
