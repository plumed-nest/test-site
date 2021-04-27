**Project ID:** [plumID:20.010]({{ '/' | absolute_url }}eggs/20/010/)  
**Source:** Equilibration/16molecules/Distributions/plumed.dat  
**Originally used with PLUMED version:** 2.6-dev  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>

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

<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ...
  DATA=refcv
  GRID_MIN=-0.5
  GRID_MAX=1.5
  GRID_BIN=1000
  BANDWIDTH=0.025
  LABEL=hh
  STRIDE=1
... <a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=hh FILE=histo STRIDE=100

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=1  ARG=* FILE=COLVAR
</pre>{% endraw %}
