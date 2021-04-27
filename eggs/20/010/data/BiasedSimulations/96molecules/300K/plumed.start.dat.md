**Project ID:** [plumID:20.010]({{ '/' | absolute_url }}eggs/20/010/)  
**Source:** BiasedSimulations/96molecules/300K/plumed.start.dat  
**Originally used with PLUMED version:** 2.6-dev  
**Stable:** [raw zipped stdout](plumed.start.dat.plumed.stdout.txt.zip) - [stderr](plumed.start.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.start.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.start.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>

vol: <a href="https://plumed.github.io/doc-master/user-doc/html/_v_o_l_u_m_e.html">VOLUME</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_v_i_r_o_n_m_e_n_t_s_i_m_i_l_a_r_i_t_y.html">ENVIRONMENTSIMILARITY</a> ...
 SPECIES=1-288:3
 SIGMA=0.055
 CRYSTAL_STRUCTURE=CUSTOM
 LABEL=refcv
 REFERENCE_1=../../../Environments/IceIhExtendedEnvironments/env1.pdb
 REFERENCE_2=../../../Environments/IceIhExtendedEnvironments/env2.pdb
 REFERENCE_3=../../../Environments/IceIhExtendedEnvironments/env3.pdb
 REFERENCE_4=../../../Environments/IceIhExtendedEnvironments/env4.pdb
 MORE_THAN={RATIONAL R_0=0.5 NN=12 MM=24}
 MEAN
... <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_v_i_r_o_n_m_e_n_t_s_i_m_i_l_a_r_i_t_y.html">ENVIRONMENTSIMILARITY</a>

<span style="color:blue"># Construct a bias potential using VES</span>
<span style="color:blue">#</span>
<span style="color:blue"># Basis functions</span>

bf1: <a href="https://plumed.github.io/doc-master/user-doc/html/_b_f__l_e_g_e_n_d_r_e.html">BF_LEGENDRE</a> ORDER=20 MINIMUM=0.0 MAXIMUM=96.0

<span style="color:blue"># Target distribution</span>

td_welltemp: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_d__w_e_l_l_t_e_m_p_e_r_e_d.html">TD_WELLTEMPERED</a> BIASFACTOR=50

<span style="color:blue"># Expansion</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_v_e_s__l_i_n_e_a_r__e_x_p_a_n_s_i_o_n.html">VES_LINEAR_EXPANSION</a> ...
 ARG=refcv.morethan
 BASIS_FUNCTIONS=bf1
 TEMP=300.0
 GRID_BINS=300
 TARGET_DISTRIBUTION=td_welltemp
 LABEL=b1
... <a href="https://plumed.github.io/doc-master/user-doc/html/_v_e_s__l_i_n_e_a_r__e_x_p_a_n_s_i_o_n.html">VES_LINEAR_EXPANSION</a>

<span style="color:blue"># Optimization algorithm</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_t__a_v_e_r_a_g_e_d__s_g_d.html">OPT_AVERAGED_SGD</a> ...
  BIAS=b1
  STRIDE=500
  LABEL=o1
  STEPSIZE=2.
  FES_OUTPUT=500
  BIAS_OUTPUT=500
  TARGETDIST_OUTPUT=500
  COEFFS_OUTPUT=100
  TARGETDIST_STRIDE=500
  <span style="color:blue">#MULTIPLE_WALKERS</span>
... <a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_t__a_v_e_r_a_g_e_d__s_g_d.html">OPT_AVERAGED_SGD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_v_i_r_o_n_m_e_n_t_s_i_m_i_l_a_r_i_t_y.html">ENVIRONMENTSIMILARITY</a> ...
 SPECIES=1-288:3
 SIGMA=0.055
 CRYSTAL_STRUCTURE=CUSTOM
 LABEL=refcv2
 REFERENCE_1=../../../Environments/IceIcExtendedEnvironments/env1.pdb
 REFERENCE_2=../../../Environments/IceIcExtendedEnvironments/env2.pdb
 MORE_THAN={RATIONAL R_0=0.5 NN=12 MM=24}
 MEAN
... <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_v_i_r_o_n_m_e_n_t_s_i_m_i_l_a_r_i_t_y.html">ENVIRONMENTSIMILARITY</a>

diff: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=refcv2.mean,refcv.mean FUNC=((x-0.26)/(0.58-0.26)-(y-0.29)/(0.80-0.29)) PERIODIC=NO
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=diff AT=0.04 KAPPA=100000 EXP=2 LABEL=uwall

<span style="color:blue"># Avoid other structures</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_q6.html">Q6</a> SPECIES=1-288:3 SWITCH={CUBIC D_0=0.3 D_MAX=0.35} VMEAN LABEL=q6
diff2: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=q6.vmean,refcv.mean FUNC=((x-0.0668781995)/(0.39184059-0.0668781995)-(y-0.2899390548628429)/(0.7838534089775562-0.2899390548628429)) PERIODIC=NO


<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=500  ARG=* FILE=COLVAR
</pre>{% endraw %}
