**Project ID:** [plumID:21.009]({{ '/' | absolute_url }}eggs/21/009/)  
**Source:** npt-fes/plumed.inp  
**Originally used with PLUMED version:** 2.6  
**Stable:** [raw zipped stdout](plumed.inp.plumed.stdout.txt.zip) - [stderr](plumed.inp.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.inp.plumed_master.stdout.txt.zip) - [stderr](plumed.inp.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> LENGTH=A

<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_a_d.html">LOAD</a> FILE=../codes/ReweightGeomFES.cpp

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> ...
  LABEL=coord
  SPECIES=1-512
  SWITCH={RATIONAL R_0=5.0 D_MAX=10.0}
  MORE_THAN={RATIONAL R_0=5.0 D_MAX=5.5}
  LOWMEM
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> ...
  LABEL=coord1
  SPECIES=1-512
  R_0=5.0
  MORE_THAN={RATIONAL R_0=5.0 D_MAX=5.5}
  MOMENTS=2,3
  LOWMEM
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=coord.morethan AT=64 KAPPA=1.0 LABEL=wall

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
  ARG=coord.morethan
  SIGMA=5000
  ADAPTIVE=DIFF
  SIGMA_MIN=0.025
  SIGMA_MAX=5.000
  HEIGHT=0.5
  PACE=10000
  BIASFACTOR=15
  TEMP=80.7
  GRID_MIN=0.0
  GRID_MAX=140.0
  GRID_BIN=14000
  CALC_RCT
  RCT_USTRIDE=40
  LABEL=b1
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__m_e_t_a_d.html">REWEIGHT_METAD</a>   TEMP=80.7 LABEL=bias
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__g_e_o_m_f_e_s.html">REWEIGHT_GEOMFES</a> TEMP=80.7 ARG=coord.morethan LABEL=gd1

<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ...
  ARG=coord.morethan
  GRID_MIN=-0.2
  GRID_MAX=64
  GRID_BIN=6420
  BANDWIDTH=0.1
  LOGWEIGHTS=bias
  CLEAR=40000000
  LABEL=hh
... <a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ...
  ARG=coord.morethan
  GRID_MIN=-0.2
  GRID_MAX=64
  GRID_BIN=6420
  BANDWIDTH=0.1
  LOGWEIGHTS=bias,gd1
  CLEAR=40000000
  LABEL=hhg
... <a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=hh  TEMP=80.7 LABEL=ff
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=hhg TEMP=80.7 LABEL=ffg

<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=ff  FILE=fes  STRIDE=40000000
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=ffg FILE=fesg STRIDE=40000000

<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=200000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=coord.morethan,coord1.morethan,coord1.moment-2,coord1.moment-3,b1.bias STRIDE=2000 FILE=colvar

</pre>{% endraw %}
