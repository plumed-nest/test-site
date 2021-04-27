**Project ID:** [plumID:21.013]({{ '/' | absolute_url }}eggs/21/013/)  
**Source:** ch4-base/symm-sample/plumed.inp  
**Originally used with PLUMED version:** 2.6  
**Stable:** [raw zipped stdout](plumed.inp.plumed.stdout.txt.zip) - [stderr](plumed.inp.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.inp.plumed_master.stdout.txt.zip) - [stderr](plumed.inp.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> LENGTH=A TIME=fs ENERGY=kcal/mol

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=1 GROUPB=2 D_0=0.85 R_0=0.25 NN=1 LABEL=vib1
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=1 GROUPB=3 D_0=0.85 R_0=0.25 NN=1 LABEL=vib2

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIESA=2-5 SPECIESB=1 D_0=0.85 R_0=0.25 NN=1 MEAN MOMENTS=2 LABEL=nm
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=nm.moment-2 AT=0.0 KAPPA=200000000 LABEL=restraint

<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ...
  ARG=nm.mean
  GRID_MIN=0.0
  GRID_MAX=1.0
  GRID_BIN=2000
  BANDWIDTH=0.005
  LABEL=targetdist
... <a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=targetdist FILE=histo STRIDE=500000

<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=100000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=vib1,vib2,nm.moment-2,nm.mean STRIDE=50000 FILE=colvar

</pre>{% endraw %}
