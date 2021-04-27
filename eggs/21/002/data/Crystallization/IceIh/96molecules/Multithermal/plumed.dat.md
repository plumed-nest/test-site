**Project ID:** [plumID:21.002]({{ '/' | absolute_url }}eggs/21/002/)  
**Source:** Crystallization/IceIh/96molecules/Multithermal/plumed.dat  
**Originally used with PLUMED version:** 2.8  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>

<span style="color:blue">#RESTART</span>

vol: <a href="https://plumed.github.io/doc-master/user-doc/html/_v_o_l_u_m_e.html">VOLUME</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_v_i_r_o_n_m_e_n_t_s_i_m_i_l_a_r_i_t_y.html">ENVIRONMENTSIMILARITY</a> ...
 SPECIES=1-288:3
 SIGMA=0.052
 CRYSTAL_STRUCTURE=CUSTOM
 LABEL=refcv
 REFERENCE_1=env1h.pdb
 REFERENCE_2=env2h.pdb
 REFERENCE_3=env3h.pdb
 REFERENCE_4=env4h.pdb
 MORE_THAN={RATIONAL R_0=0.5 NN=8 MM=16}
 MEAN
... <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_v_i_r_o_n_m_e_n_t_s_i_m_i_l_a_r_i_t_y.html">ENVIRONMENTSIMILARITY</a>

<span style="color:blue"># Construct a bias potential</span>

energy: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a>

<span style="color:blue"># Construct bias potential with OPS</span>

ecv: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_c_v__m_u_l_t_i_t_h_e_r_m_a_l__m_u_l_t_i_b_a_r_i_c.html">ECV_MULTITHERMAL_MULTIBARIC</a> ...
   ARG=energy,vol 
   TEMP=330 
   MIN_TEMP=300 
   MAX_TEMP=350 
   PRESSURE=0.06022140857
   MIN_PRESSURE=0.06022140857
   MAX_PRESSURE=0.06022140857
...

ecv2: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_c_v__u_m_b_r_e_l_l_a_s__l_i_n_e.html">ECV_UMBRELLAS_LINE</a> ARG=refcv.morethan MIN_CV=0.0 MAX_CV=96.0 SIGMA=1.0 BARRIER=150 TEMP=330

opes: <a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_e_s__e_x_p_a_n_d_e_d.html">OPES_EXPANDED</a> ARG=ecv.*,ecv2.* FILE=DeltaF.data PACE=100 WALKERS_MPI 

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_v_i_r_o_n_m_e_n_t_s_i_m_i_l_a_r_i_t_y.html">ENVIRONMENTSIMILARITY</a> ...
 SPECIES=1-288:3
 SIGMA=0.052
 CRYSTAL_STRUCTURE=CUSTOM
 LABEL=refcv2
 REFERENCE_1=env1c.pdb
 REFERENCE_2=env2c.pdb
 MORE_THAN={RATIONAL R_0=0.5 NN=10 MM=20}
 MEAN
... <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_v_i_r_o_n_m_e_n_t_s_i_m_i_l_a_r_i_t_y.html">ENVIRONMENTSIMILARITY</a>

diff: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=refcv2.mean,refcv.mean FUNC=((x-0.230)/(0.585-0.230)-(y-0.254)/(0.812-0.254)) PERIODIC=NO
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=diff AT=0.1 KAPPA=100000 EXP=2 LABEL=uwall

<span style="color:blue"># Avoid other structures</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_q6.html">Q6</a> SPECIES=1-288:3 SWITCH={CUBIC D_0=0.3 D_MAX=0.35} VMEAN LABEL=q6
diff2: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=q6.vmean,refcv.mean FUNC=((x-0.0702)/(0.429-0.0702)-(y-0.254)/(0.812-0.254)) PERIODIC=NO
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=diff2 AT=0.1 KAPPA=100000 EXP=2 LABEL=uwall2

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=500  ARG=* FILE=COLVAR
</pre>{% endraw %}
