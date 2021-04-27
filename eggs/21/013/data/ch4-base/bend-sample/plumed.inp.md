**Project ID:** [plumID:21.013]({{ '/' | absolute_url }}eggs/21/013/)  
**Source:** ch4-base/bend-sample/plumed.inp  
**Originally used with PLUMED version:** 2.6  
**Stable:** [raw zipped stdout](plumed.inp.plumed.stdout.txt.zip) - [stderr](plumed.inp.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.inp.plumed_master.stdout.txt.zip) - [stderr](plumed.inp.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> LENGTH=A TIME=fs ENERGY=kcal/mol

<a href="https://plumed.github.io/doc-master/user-doc/html/_a_n_g_l_e_s.html">ANGLES</a> GROUPA=1 GROUPB=2-5 BETWEEN={GAUSSIAN LOWER=0.5pi UPPER=0.7pi} SWITCH={RATIONAL D_0=1.50 R_0=0.25} LABEL=ang

<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ...
  ARG=ang.between
  GRID_MIN=1.0
  GRID_MAX=4.5
  GRID_BIN=3500
  BANDWIDTH=0.005
  LABEL=targetdist
... <a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=targetdist FILE=histo STRIDE=500000

<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=100000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=ang.between STRIDE=50000 FILE=colvar

</pre>{% endraw %}
