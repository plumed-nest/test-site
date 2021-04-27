**Project ID:** [plumID:19.000]({{ '/' | absolute_url }}eggs/19/000/)  
**Source:** sodium/plumed-ves.dat  
**Originally used with PLUMED version:** 2.6-dev  
**Stable:** [raw zipped stdout](plumed-ves.dat.plumed.stdout.txt.zip) - [stderr](plumed-ves.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed-ves.dat.plumed_master.stdout.txt.zip) - [stderr](plumed-ves.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_a_d.html">LOAD</a> FILE=DebyeStructureFactor.cpp
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> LENGTH=A

ene: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a>
cv: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_e_b_y_e__s_t_r_u_c_t_u_r_e__f_a_c_t_o_r.html">DEBYE_STRUCTURE_FACTOR</a> CUTOFF=10.5 ACTIVE_Q=2.070595

<a href="https://plumed.github.io/doc-master/user-doc/html/_v_e_s__d_e_l_t_a__f.html">VES_DELTA_F</a> ...
  LABEL=ves
  ARG=cv.*
  FILE_F0=fesA.data
  FILE_F1=fesB.data
  TEMP=350
  AV_STRIDE=500
  BIASFACTOR=20
  M_STEP=1
  PRINT_STRIDE=100
  ALPHA_FILE=Alpha.data
... <a href="https://plumed.github.io/doc-master/user-doc/html/_v_e_s__d_e_l_t_a__f.html">VES_DELTA_F</a>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FMT=%g STRIDE=500   FILE=Colvar.data ARG=cv.*,ene,ves.bias,ves.rct

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
<span style="color:blue">-- !!bash --</span>
<span style="color:blue">--- Active shells ---</span>
<span style="color:blue">awk -v n=1 -v trig=1 'BEGIN{printf "cv: DEBYE_STRUCTURE_FACTOR NOPBC ACTIVE_Q="}NR>10{der=$2-prev; if ($2>trig && der<0 && prev_der>0 && ++conta<=n) {printf val; if (conta<n) printf ","; else printf "\n"} prev=$2; prev_der=der; val=$1}' ../unb-bcc/DebyeSq.data</span>
<span style="color:blue"></span>
</pre>{% endraw %}
