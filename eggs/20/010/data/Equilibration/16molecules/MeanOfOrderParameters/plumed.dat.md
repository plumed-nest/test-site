**Project ID:** [plumID:20.010]({{ '/' | absolute_url }}eggs/20/010/)  
**Source:** Equilibration/16molecules/MeanOfOrderParameters/plumed.dat  
**Originally used with PLUMED version:** 2.6-dev  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>

vol: <a href="https://plumed.github.io/doc-master/user-doc/html/_v_o_l_u_m_e.html">VOLUME</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_v_i_r_o_n_m_e_n_t_s_i_m_i_l_a_r_i_t_y.html">ENVIRONMENTSIMILARITY</a> ...
 SPECIES=1-48:3
 SIGMA=0.076
 CRYSTAL_STRUCTURE=CUSTOM
 LABEL=refcv
 REFERENCE_1=../../../Environments/IceIhExtendedEnvironments/env1.pdb
 REFERENCE_2=../../../Environments/IceIhExtendedEnvironments/env2.pdb
 REFERENCE_3=../../../Environments/IceIhExtendedEnvironments/env3.pdb
 REFERENCE_4=../../../Environments/IceIhExtendedEnvironments/env4.pdb
 MORE_THAN={RATIONAL R_0=0.5 NN=12 MM=24}
 MEAN
... <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_v_i_r_o_n_m_e_n_t_s_i_m_i_l_a_r_i_t_y.html">ENVIRONMENTSIMILARITY</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_v_i_r_o_n_m_e_n_t_s_i_m_i_l_a_r_i_t_y.html">ENVIRONMENTSIMILARITY</a> ...
 SPECIES=1-48:3
 SIGMA=0.076
 CRYSTAL_STRUCTURE=CUSTOM
 LABEL=refcv2
 REFERENCE_1=../../../Environments/IceIcExtendedEnvironments/env1.pdb
 REFERENCE_2=../../../Environments/IceIcExtendedEnvironments/env2.pdb
 MORE_THAN={RATIONAL R_0=0.5 NN=12 MM=24}
 MEAN
... <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_v_i_r_o_n_m_e_n_t_s_i_m_i_l_a_r_i_t_y.html">ENVIRONMENTSIMILARITY</a>

<span style="color:blue"># Avoid other structures</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_q6.html">Q6</a> SPECIES=1-48:3 SWITCH={CUBIC D_0=0.3 D_MAX=0.35} VMEAN LABEL=q6

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=1  ARG=* FILE=COLVAR
</pre>{% endraw %}
