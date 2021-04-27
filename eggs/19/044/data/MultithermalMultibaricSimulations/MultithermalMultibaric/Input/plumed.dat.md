**Project ID:** [plumID:19.044]({{ '/' | absolute_url }}eggs/19/044/)  
**Source:** MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.dat  
**Originally used with PLUMED version:** 2.4-dev  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>

energy: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a>

vol: <a href="https://plumed.github.io/doc-master/user-doc/html/_v_o_l_u_m_e.html">VOLUME</a>

<span style="color:blue"># Construct a bias potential using VES</span>
<span style="color:blue">#</span>
<span style="color:blue"># Basis functions</span>

bf1: <a href="https://plumed.github.io/doc-master/user-doc/html/_b_f__l_e_g_e_n_d_r_e.html">BF_LEGENDRE</a> ORDER=10 MINIMUM=-14750 MAXIMUM=-12250
bf2: <a href="https://plumed.github.io/doc-master/user-doc/html/_b_f__l_e_g_e_n_d_r_e.html">BF_LEGENDRE</a> ORDER=10 MINIMUM=6.5 MAXIMUM=8.25

<span style="color:blue"># Target distributions</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_t_d__m_u_l_t_i_t_h_e_r_m_a_l__m_u_l_t_i_b_a_r_i_c.html">TD_MULTITHERMAL_MULTIBARIC</a> ...
 MIN_TEMP=260
 MAX_TEMP=350
 MAX_PRESSURE=180.66422571 <span style="color:blue"># 300 MPa</span>
 MIN_PRESSURE=0.06022140857
 PRESSURE=0.06022140857
 STEPS_PRESSURE=20
 STEPS_TEMP=20
 SIGMA=50.,0.05
 THRESHOLD=1
 LABEL=td_multi
... <a href="https://plumed.github.io/doc-master/user-doc/html/_t_d__m_u_l_t_i_t_h_e_r_m_a_l__m_u_l_t_i_b_a_r_i_c.html">TD_MULTITHERMAL_MULTIBARIC</a>

<span style="color:blue"># Expansion</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_v_e_s__l_i_n_e_a_r__e_x_p_a_n_s_i_o_n.html">VES_LINEAR_EXPANSION</a> ...
 ARG=energy,vol
 BASIS_FUNCTIONS=bf1,bf2
 TEMP=300.0
 GRID_BINS=200,200
 TARGET_DISTRIBUTION=td_multi
 LABEL=b1
... <a href="https://plumed.github.io/doc-master/user-doc/html/_v_e_s__l_i_n_e_a_r__e_x_p_a_n_s_i_o_n.html">VES_LINEAR_EXPANSION</a>

<span style="color:blue"># Optimization algorithm</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_t__d_u_m_m_y.html">OPT_DUMMY</a> ...
  BIAS=b1
  STRIDE=500
  LABEL=o1
  COEFFS_OUTPUT=10
... <a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_t__d_u_m_m_y.html">OPT_DUMMY</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=* FILE=COLVAR STRIDE=500

</pre>{% endraw %}
