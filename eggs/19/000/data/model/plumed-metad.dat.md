**Project ID:** [plumID:19.000]({{ '/' | absolute_url }}eggs/19/000/)  
**Source:** model/plumed-metad.dat  
**Originally used with PLUMED version:** 2.6-dev  
**Stable:** [raw zipped stdout](plumed-metad.dat.plumed.stdout.txt.zip) - [stderr](plumed-metad.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed-metad.dat.plumed_master.stdout.txt.zip) - [stderr](plumed-metad.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> NATURAL

ene: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a>
p: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_o_s_i_t_i_o_n.html">POSITION</a> ATOM=1

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
  LABEL=metad
  ARG=p.x
  FILE=Hills.data
  PACE=500
  HEIGHT=1.2
  SIGMA=0.35
  BIASFACTOR=10.0
  GRID_MIN=-3
  GRID_MAX=3
  GRID_BIN=100
  CALC_RCT
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FMT=%g STRIDE=500 FILE=Colvar.data ARG=p.x,p.y,metad.bias,metad.rct,ene

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
<span style="color:blue"></span>
<span style="color:blue"></span>
</pre>{% endraw %}
