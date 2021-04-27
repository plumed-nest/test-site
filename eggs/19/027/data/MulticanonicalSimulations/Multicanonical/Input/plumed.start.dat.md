**Project ID:** [plumID:19.027]({{ '/' | absolute_url }}eggs/19/027/)  
**Source:** MulticanonicalSimulations/Multicanonical/Input/plumed.start.dat  
**Originally used with PLUMED version:** 2.4-dev  
**Stable:** [raw zipped stdout](plumed.start.dat.plumed.stdout.txt.zip) - [stderr](plumed.start.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.start.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.start.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> LENGTH=A

energy: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a>

<span style="color:blue"># Construct a bias potential using VES</span>
<span style="color:blue">#</span>
<span style="color:blue"># Basis functions</span>

bf1: <a href="https://plumed.github.io/doc-master/user-doc/html/_b_f__l_e_g_e_n_d_r_e.html">BF_LEGENDRE</a> ORDER=20 MINIMUM=-25000 MAXIMUM=-23500

<span style="color:blue"># Target distributions</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_t_d__m_u_l_t_i_c_a_n_o_n_i_c_a_l.html">TD_MULTICANONICAL</a> ...
 LABEL=td_multi
 SIGMA=50.0
 MIN_TEMP=400
 MAX_TEMP=600
 THRESHOLD=1
... <a href="https://plumed.github.io/doc-master/user-doc/html/_t_d__m_u_l_t_i_c_a_n_o_n_i_c_a_l.html">TD_MULTICANONICAL</a>


<span style="color:blue"># Expansion</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_v_e_s__l_i_n_e_a_r__e_x_p_a_n_s_i_o_n.html">VES_LINEAR_EXPANSION</a> ...
 ARG=energy
 BASIS_FUNCTIONS=bf1
 TEMP=500.0
 GRID_BINS=1000
 TARGET_DISTRIBUTION=td_multi
 LABEL=b1
... <a href="https://plumed.github.io/doc-master/user-doc/html/_v_e_s__l_i_n_e_a_r__e_x_p_a_n_s_i_o_n.html">VES_LINEAR_EXPANSION</a>

<span style="color:blue"># Optimization algorithm</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_t__a_v_e_r_a_g_e_d__s_g_d.html">OPT_AVERAGED_SGD</a> ...
  BIAS=b1
  STRIDE=500
  LABEL=o1
  STEPSIZE=1.
  FES_OUTPUT=500
  BIAS_OUTPUT=500
  TARGETDIST_OUTPUT=500
  COEFFS_OUTPUT=100
  TARGETDIST_STRIDE=500
... <a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_t__a_v_e_r_a_g_e_d__s_g_d.html">OPT_AVERAGED_SGD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=* FILE=COLVAR STRIDE=500

</pre>{% endraw %}
