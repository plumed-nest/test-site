**Project ID:** [plumID:19.000]({{ '/' | absolute_url }}eggs/19/000/)  
**Source:** model/plumed-ves.dat  
**Originally used with PLUMED version:** 2.6-dev  
**Stable:** [raw zipped stdout](plumed-ves.dat.plumed.stdout.txt.zip) - [stderr](plumed-ves.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed-ves.dat.plumed_master.stdout.txt.zip) - [stderr](plumed-ves.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> NATURAL

ene: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a>
p: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_o_s_i_t_i_o_n.html">POSITION</a> ATOM=1

<a href="https://plumed.github.io/doc-master/user-doc/html/_v_e_s__d_e_l_t_a__f.html">VES_DELTA_F</a> ...
  LABEL=ves
  ARG=p.x
  TEMP=1
  FILE_F0=fesA.data
  FILE_F1=fesB.data
  BIASFACTOR=10.0
  AV_STRIDE=500
  M_STEP=0.05
  PRINT_STRIDE=100
  ALPHA_FILE=Alpha.data
... <a href="https://plumed.github.io/doc-master/user-doc/html/_v_e_s__d_e_l_t_a__f.html">VES_DELTA_F</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FMT=%g STRIDE=500 FILE=Colvar.data ARG=p.x,p.y,ves.bias,ves.rct,ene

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
<span style="color:blue"></span>
</pre>{% endraw %}
