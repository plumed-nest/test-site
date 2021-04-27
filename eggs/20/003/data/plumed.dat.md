**Project ID:** [plumID:20.003]({{ '/' | absolute_url }}eggs/20/003/)  
**Source:** plumed.dat  
**Originally used with PLUMED version:** 2.6-dev  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_a_d.html">LOAD</a> FILE=TD_TS-target-plumed2.6.cpp
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> NATURAL
p: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_o_s_i_t_i_o_n.html">POSITION</a> ATOM=1
ene: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a>
bf1: <a href="https://plumed.github.io/doc-master/user-doc/html/_b_f__l_e_g_e_n_d_r_e.html">BF_LEGENDRE</a> MINIMUM=-3 MAXIMUM=+3 ORDER=14 SCALED 

<a href="https://plumed.github.io/doc-master/user-doc/html/_t_d__t_s__t_a_r_g_e_t.html">TD_TS_TARGET</a> ...
  SCALEFACTOR=30
  LAMBDA=0.05    
  LIMIT=0.1
  PRINT_STRIDE=500
  LABEL=td
... <a href="https://plumed.github.io/doc-master/user-doc/html/_t_d__t_s__t_a_r_g_e_t.html">TD_TS_TARGET</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_v_e_s__l_i_n_e_a_r__e_x_p_a_n_s_i_o_n.html">VES_LINEAR_EXPANSION</a> ...
  ARG=p.x
  BASIS_FUNCTIONS=bf1
  LABEL=b1
  TEMP=1.0
  GRID_BINS=300
  TARGET_DISTRIBUTION=td
... <a href="https://plumed.github.io/doc-master/user-doc/html/_v_e_s__l_i_n_e_a_r__e_x_p_a_n_s_i_o_n.html">VES_LINEAR_EXPANSION</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_t__a_v_e_r_a_g_e_d__s_g_d.html">OPT_AVERAGED_SGD</a> ...
  BIAS=b1
  STRIDE=500
  LABEL=o1
  STEPSIZE=1
  FES_OUTPUT=100
  COEFFS_OUTPUT=100
  TARGETDIST_OUTPUT=500
  TARGETDIST_STRIDE=500
  MONITOR_AVERAGE_GRADIENT
... <a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_t__a_v_e_r_a_g_e_d__s_g_d.html">OPT_AVERAGED_SGD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=* STRIDE=100 FILE=colvar.data FMT=%8.4f
</pre>{% endraw %}
