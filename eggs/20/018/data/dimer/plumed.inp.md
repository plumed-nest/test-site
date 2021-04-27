**Project ID:** [plumID:20.018]({{ '/' | absolute_url }}eggs/20/018/)  
**Source:** dimer/plumed.inp  
**Originally used with PLUMED version:** 2.6-mod  
**Stable:** [raw zipped stdout](plumed.inp.plumed.stdout.txt.zip) - [stderr](plumed.inp.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.inp.plumed_master.stdout.txt.zip) - [stderr](plumed.inp.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> NATURAL

<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_a_d.html">LOAD</a> FILE=../src/bias/ReweightGeomFES.cpp

<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1,2 LABEL=dist
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=1 GROUPB=2 R_0=1.0 D_0=0.75 NN=1 LABEL=coord

<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=dist AT=7.0 KAPPA=1.0 LABEL=walls

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
  ARG=coord
  SIGMA=0.01
  HEIGHT=0.25
  PACE=2500
  BIASFACTOR=10
  TEMP=1.5
  GRID_MIN=0.0
  GRID_MAX=1.0
  GRID_BIN=500
  CALC_RCT
  RCT_USTRIDE=1
  LABEL=b1
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__m_e_t_a_d.html">REWEIGHT_METAD</a> TEMP=1.5 LABEL=bias
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__g_e_o_m_f_e_s.html">REWEIGHT_GEOMFES</a> TEMP=1.5 ARG=coord LABEL=geom

<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ...
  ARG=dist
  GRID_MIN=0.0
  GRID_MAX=10.0
  GRID_BIN=1000
  BANDWIDTH=0.05
  LOGWEIGHTS=bias
  LABEL=hdist
... <a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ...
  ARG=coord
  GRID_MIN=0.0
  GRID_MAX=1.0
  GRID_BIN=200
  BANDWIDTH=0.02
  LOGWEIGHTS=bias
  LABEL=hcoord
... <a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ...
  ARG=coord
  GRID_MIN=0.0
  GRID_MAX=1.0
  GRID_BIN=200
  BANDWIDTH=0.02
  LOGWEIGHTS=bias,geom
  LABEL=hcoordg
... <a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=hdist TEMP=1.5 LABEL=fdist
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=hcoord TEMP=1.5 LABEL=fcoord
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=hcoordg TEMP=1.5 LABEL=fcoordg

<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=fdist FILE=fesdist STRIDE=500000
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=fcoord FILE=fescoord STRIDE=500000
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=fcoordg FILE=fescoordg STRIDE=500000

<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=dist,coord,b1.bias,b1.rct STRIDE=1000 FILE=colvar

</pre>{% endraw %}
