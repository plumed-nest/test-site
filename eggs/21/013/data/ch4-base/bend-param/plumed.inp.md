**Project ID:** [plumID:21.013]({{ '/' | absolute_url }}eggs/21/013/)  
**Source:** ch4-base/bend-param/plumed.inp  
**Originally used with PLUMED version:** 2.6  
**Stable:** [raw zipped stdout](plumed.inp.plumed.stdout.txt.zip) - [stderr](plumed.inp.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.inp.plumed_master.stdout.txt.zip) - [stderr](plumed.inp.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> LENGTH=A TIME=fs ENERGY=kcal/mol

<a href="https://plumed.github.io/doc-master/user-doc/html/_a_n_g_l_e_s.html">ANGLES</a> GROUPA=1 GROUPB=2-5 BETWEEN={GAUSSIAN LOWER=0.5pi UPPER=0.7pi} SWITCH={RATIONAL D_0=1.50 R_0=0.25} LABEL=ang

bf1: <a href="https://plumed.github.io/doc-master/user-doc/html/_b_f__c_h_e_b_y_s_h_e_v.html">BF_CHEBYSHEV</a> MINIMUM=1.0 MAXIMUM=4.5 ORDER=96

td: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_d__g_r_i_d.html">TD_GRID</a> FILE=histo

<span style="color:blue"># Expansion</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_v_e_s__l_i_n_e_a_r__e_x_p_a_n_s_i_o_n.html">VES_LINEAR_EXPANSION</a> ...
 ARG=ang.between
 BASIS_FUNCTIONS=bf1
 TEMP=500
 GRID_BINS=3500
 TARGET_DISTRIBUTION=td
 LABEL=external
... <a href="https://plumed.github.io/doc-master/user-doc/html/_v_e_s__l_i_n_e_a_r__e_x_p_a_n_s_i_o_n.html">VES_LINEAR_EXPANSION</a>

<span style="color:blue"># Optimization algorithm</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_t__a_v_e_r_a_g_e_d__s_g_d.html">OPT_AVERAGED_SGD</a> ...
  BIAS=external
  STRIDE=5000
  LABEL=o1
  STEPSIZE=0.5
  FES_OUTPUT=10000
  BIAS_OUTPUT=100
  FES_PROJ_OUTPUT=20
  COEFFS_OUTPUT=1
... <a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_t__a_v_e_r_a_g_e_d__s_g_d.html">OPT_AVERAGED_SGD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=100000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=ang.between,external.bias STRIDE=10000 FILE=colvar

</pre>{% endraw %}
