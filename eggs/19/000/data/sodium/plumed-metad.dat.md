**Project ID:** [plumID:19.000]({{ '/' | absolute_url }}eggs/19/000/)  
**Source:** sodium/plumed-metad.dat  
**Originally used with PLUMED version:** 2.6-dev  
**Stable:** [raw zipped stdout](plumed-metad.dat.plumed.stdout.txt.zip) - [stderr](plumed-metad.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed-metad.dat.plumed_master.stdout.txt.zip) - [stderr](plumed-metad.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_a_d.html">LOAD</a> FILE=DebyeStructureFactor.cpp
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> LENGTH=A

ene: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a>
cv: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_e_b_y_e__s_t_r_u_c_t_u_r_e__f_a_c_t_o_r.html">DEBYE_STRUCTURE_FACTOR</a> CUTOFF=10.5 ACTIVE_Q=2.070595

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
  LABEL=metad
  ARG=cv.*
  FILE=Hills.data
  TEMP=350
  PACE=500
  SIGMA=0.02
  HEIGHT=10
  BIASFACTOR=20
  GRID_MIN=1.3
  GRID_MAX=2.8
  GRID_BIN=200
  CALC_RCT
  WALKERS_MPI
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=500  FMT=%g FILE=Colvar.data ARG=cv.*,ene,metad.bias,metad.rct

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
<span style="color:blue"></span>
</pre>{% endraw %}
