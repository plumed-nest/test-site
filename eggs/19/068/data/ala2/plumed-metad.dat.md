**Project ID:** [plumID:19.068]({{ '/' | absolute_url }}eggs/19/068/)  
**Source:** ala2/plumed-metad.dat  
**Originally used with PLUMED version:** 2.7  
**Stable:** [raw zipped stdout](plumed-metad.dat.plumed.stdout.txt.zip) - [stderr](plumed-metad.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed-metad.dat.plumed_master.stdout.txt.zip) - [stderr](plumed-metad.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>

phi: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=5,7,9,15
psi: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=7,9,15,17

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
  LABEL=metad
  ARG=phi,psi
  FILE=Hills.data
  TEMP=300.0
  PACE=500
  HEIGHT=1.2
  SIGMA=0.35,0.35
  BIASFACTOR=10.0
  GRID_MIN=-pi,-pi
  GRID_MAX=pi,pi
  GRID_BIN=100,100
  CALC_MAX_BIAS
  CALC_RCT
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FMT=%g STRIDE=500 FILE=Colvar.data ARG=phi,psi,metad.bias,metad.rct,metad.maxbias

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
