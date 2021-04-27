**Project ID:** [plumID:21.002]({{ '/' | absolute_url }}eggs/21/002/)  
**Source:** Crystallization/IceIh/288molecules/350K/plumed.start.dat  
**Originally used with PLUMED version:** 2.8  
**Stable:** [raw zipped stdout](plumed.start.dat.plumed.stdout.txt.zip) - [stderr](plumed.start.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.start.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.start.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>

vol: <a href="https://plumed.github.io/doc-master/user-doc/html/_v_o_l_u_m_e.html">VOLUME</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_v_i_r_o_n_m_e_n_t_s_i_m_i_l_a_r_i_t_y.html">ENVIRONMENTSIMILARITY</a> ...
 SPECIES=1-864:3
 SIGMA=0.05
 CRYSTAL_STRUCTURE=CUSTOM
 LABEL=refcv
 REFERENCE_1=env1h.pdb
 REFERENCE_2=env2h.pdb
 REFERENCE_3=env3h.pdb
 REFERENCE_4=env4h.pdb
 MORE_THAN={RATIONAL R_0=0.5 NN=6 MM=12}
 MEAN
... <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_v_i_r_o_n_m_e_n_t_s_i_m_i_l_a_r_i_t_y.html">ENVIRONMENTSIMILARITY</a>

<span style="color:blue"># Construct a bias potential</span>

energy: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a>

<span style="color:blue"># Construct a bias potential using VES</span>
<span style="color:blue">#</span>
<span style="color:blue"># Basis functions</span>

bf1: <a href="https://plumed.github.io/doc-master/user-doc/html/_b_f__l_e_g_e_n_d_r_e.html">BF_LEGENDRE</a> ORDER=40 MINIMUM=0.0 MAXIMUM=288.0

<span style="color:blue"># Target distribution</span>

td_uni: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_d__u_n_i_f_o_r_m.html">TD_UNIFORM</a>

<span style="color:blue"># Expansion</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_v_e_s__l_i_n_e_a_r__e_x_p_a_n_s_i_o_n.html">VES_LINEAR_EXPANSION</a> ...
 ARG=refcv.morethan
 BASIS_FUNCTIONS=bf1
 TEMP=350.0
 GRID_BINS=300
 TARGET_DISTRIBUTION=td_uni
 LABEL=b1
... <a href="https://plumed.github.io/doc-master/user-doc/html/_v_e_s__l_i_n_e_a_r__e_x_p_a_n_s_i_o_n.html">VES_LINEAR_EXPANSION</a>

<span style="color:blue"># Optimization algorithm</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_t__a_v_e_r_a_g_e_d__s_g_d.html">OPT_AVERAGED_SGD</a> ...
  BIAS=b1
  STRIDE=500
  LABEL=o1
  STEPSIZE=1
  FES_OUTPUT=500
  BIAS_OUTPUT=500
  COEFFS_OUTPUT=100
  <span style="color:blue">#MULTIPLE_WALKERS</span>
... <a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_t__a_v_e_r_a_g_e_d__s_g_d.html">OPT_AVERAGED_SGD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_v_i_r_o_n_m_e_n_t_s_i_m_i_l_a_r_i_t_y.html">ENVIRONMENTSIMILARITY</a> ...
 SPECIES=1-864:3
 SIGMA=0.05
 CRYSTAL_STRUCTURE=CUSTOM
 LABEL=refcv2
 REFERENCE_1=env1c.pdb
 REFERENCE_2=env2c.pdb
 MORE_THAN={RATIONAL R_0=0.5 NN=6 MM=12}
 MEAN
... <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_v_i_r_o_n_m_e_n_t_s_i_m_i_l_a_r_i_t_y.html">ENVIRONMENTSIMILARITY</a>

diff: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=refcv2.mean,refcv.mean FUNC=((x-0.2075)/(0.5821-0.2075)-(y-0.2319)/(0.8137-0.2319)) PERIODIC=NO
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=diff AT=0.05 KAPPA=100000 EXP=2 LABEL=uwall

<span style="color:blue"># Avoid other structures</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_q6.html">Q6</a> SPECIES=1-864:3 SWITCH={CUBIC D_0=0.3 D_MAX=0.35} VMEAN LABEL=q6
diff2: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=q6.vmean,refcv.mean FUNC=((x-0.0402)/(0.4404-0.0402)-(y-0.2319)/(0.8137-0.2319)) PERIODIC=NO
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=diff2 AT=0.05 KAPPA=100000 EXP=2 LABEL=uwall2

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=500  ARG=* FILE=COLVAR
</pre>{% endraw %}
