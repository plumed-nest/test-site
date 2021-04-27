**Project ID:** [plumID:21.009]({{ '/' | absolute_url }}eggs/21/009/)  
**Source:** nvt-committor/recross/plumed.inp  
**Originally used with PLUMED version:** 2.6  
**Stable:** [raw zipped stdout](plumed.inp.plumed.stdout.txt.zip) - [stderr](plumed.inp.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.inp.plumed_master.stdout.txt.zip) - [stderr](plumed.inp.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> LENGTH=A

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> ...
  LABEL=coord
  SPECIES=1-512
  SWITCH={RATIONAL R_0=5.0 D_MAX=10.0}
  MORE_THAN={RATIONAL R_0=5.0 D_MAX=5.5}
  LOWMEM
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_m_i_t_t_o_r.html">COMMITTOR</a> ...
  ARG=coord.morethan
  STRIDE=1
  BASIN_LL1=0
  BASIN_UL1=24
  BASIN_LL2=24
  BASIN_UL2=60
  NOSTOP
  FILE=commit
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_m_i_t_t_o_r.html">COMMITTOR</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=200000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=coord.morethan STRIDE=2000 FILE=colvar

</pre>{% endraw %}
