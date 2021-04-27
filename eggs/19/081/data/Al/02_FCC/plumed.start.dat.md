**Project ID:** [plumID:19.081]({{ '/' | absolute_url }}eggs/19/081/)  
**Source:** Al/02_FCC/plumed.start.dat  
**Originally used with PLUMED version:** 2.6-dev  
**Stable:** [raw zipped stdout](plumed.start.dat.plumed.stdout.txt.zip) - [stderr](plumed.start.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.start.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.start.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_a_d.html">LOAD</a> FILE=../../RefCV.cpp

energy: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a>

vol: <a href="https://plumed.github.io/doc-master/user-doc/html/_v_o_l_u_m_e.html">VOLUME</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_f_c_v.html">REFCV</a> ...
 SPECIES=1-256
 SIGMA=0.04
 LATTICE_CONSTANTS=0.38
 CRYSTAL_STRUCTURE=FCC
 LABEL=refcv
 MORE_THAN={RATIONAL R_0=0.5 NN=12 MM=24}
 MEAN
... <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_f_c_v.html">REFCV</a>

<span style="color:blue"># Construct a bias potential using VES</span>
<span style="color:blue">#</span>
<span style="color:blue"># Basis functions</span>

bf1: <a href="https://plumed.github.io/doc-master/user-doc/html/_b_f__l_e_g_e_n_d_r_e.html">BF_LEGENDRE</a> ORDER=8 MINIMUM=-80000 MAXIMUM=-51000
bf2: <a href="https://plumed.github.io/doc-master/user-doc/html/_b_f__l_e_g_e_n_d_r_e.html">BF_LEGENDRE</a> ORDER=8 MINIMUM=2.9 MAXIMUM=4.3
bf3: <a href="https://plumed.github.io/doc-master/user-doc/html/_b_f__l_e_g_e_n_d_r_e.html">BF_LEGENDRE</a> ORDER=8 MINIMUM=0.0 MAXIMUM=256.0

<span style="color:blue"># Target distribution</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_t_d__m_u_l_t_i_t_h_e_r_m_a_l__m_u_l_t_i_b_a_r_i_c.html">TD_MULTITHERMAL_MULTIBARIC</a> ... 
 LABEL=td_multitp
 MIN_PRESSURE=12044.281714
 MAX_PRESSURE=24088.563428
 MIN_TEMP=1800.0
 MAX_TEMP=2400.0
 PRESSURE=18066.422571
 SIGMA=500.0,0.05,10.0
 THRESHOLD=20
 STEPS_TEMP=20
 STEPS_PRESSURE=20
... <a href="https://plumed.github.io/doc-master/user-doc/html/_t_d__m_u_l_t_i_t_h_e_r_m_a_l__m_u_l_t_i_b_a_r_i_c.html">TD_MULTITHERMAL_MULTIBARIC</a>

<span style="color:blue"># Expansion</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_v_e_s__l_i_n_e_a_r__e_x_p_a_n_s_i_o_n.html">VES_LINEAR_EXPANSION</a> ...
 ARG=energy,vol,refcv.morethan
 BASIS_FUNCTIONS=bf1,bf2,bf3
 TEMP=2000.0
 GRID_BINS=40,40,40
 TARGET_DISTRIBUTION=td_multitp
 LABEL=b1
... <a href="https://plumed.github.io/doc-master/user-doc/html/_v_e_s__l_i_n_e_a_r__e_x_p_a_n_s_i_o_n.html">VES_LINEAR_EXPANSION</a>

<span style="color:blue"># Optimization algorithm</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_t__a_v_e_r_a_g_e_d__s_g_d.html">OPT_AVERAGED_SGD</a> ...
  BIAS=b1
  STRIDE=500
  LABEL=o1
  STEPSIZE=50.
  FES_OUTPUT=500
  BIAS_OUTPUT=500
  TARGETDIST_OUTPUT=500
  COEFFS_OUTPUT=100
  TARGETDIST_STRIDE=500
  <span style="color:blue">#MULTIPLE_WALKERS # Commented out to pass plumed nest's test, uncomment for calculation</span>
... <a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_t__a_v_e_r_a_g_e_d__s_g_d.html">OPT_AVERAGED_SGD</a>


<a href="https://plumed.github.io/doc-master/user-doc/html/_q6.html">Q6</a> SPECIES=1-256 SWITCH={CUBIC D_0=0.25 D_MAX=0.35} VMEAN LABEL=q6
diff: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=q6.vmean,refcv.mean FUNC=(x-0.064)/(0.461-0.064)-(y-0.251)/(0.752-0.251) PERIODIC=NO
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=diff AT=0.05 KAPPA=500000 EXP=2 LABEL=uwall

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=* FILE=COLVAR STRIDE=500
</pre>{% endraw %}
