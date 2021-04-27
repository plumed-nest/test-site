**Project ID:** [plumID:20.018]({{ '/' | absolute_url }}eggs/20/018/)  
**Source:** da-tt/plumed.inp  
**Originally used with PLUMED version:** 2.6-mod  
**Stable:** [raw zipped stdout](plumed.inp.plumed.stdout.txt.zip) - [stderr](plumed.inp.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.inp.plumed_master.stdout.txt.zip) - [stderr](plumed.inp.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> LENGTH=A TIME=fs ENERGY=kcal/mol

<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_a_d.html">LOAD</a> FILE=../src/bias/ReweightGeomFES.cpp

<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1,2 LABEL=d1
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=2,3 LABEL=d2
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=3,4 LABEL=d3
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=4,5 LABEL=d4
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=5,6 LABEl=d5
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1,6 LABEL=d6

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3,d4,d6 COEFFICIENTS=-0.05,0.21,-0.08,0.69,0.69 PERIODIC=NO LABEL=hlda

<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=d4,d6 AT=5.0,5.0 KAPPA=50,50 LABEL=walls

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
  ARG=hlda
  SIGMA=0.15
  HEIGHT=1.0
  PACE=100
  TTBIASFACTOR=25
  CALC_TRANSITION_BIAS
  TRANSITIONWELL0=2.0
  TRANSITIONWELL1=5.0
  TEMP=600
  GRID_MIN=1.0
  GRID_MAX=9.0
  GRID_BIN=1600
  CALC_RCT
  RCT_USTRIDE=1
  LABEL=b1
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__b_i_a_s.html">REWEIGHT_BIAS</a> ARG=b1.bias    TEMP=600 LABEL=bias
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__g_e_o_m_f_e_s.html">REWEIGHT_GEOMFES</a> ARG=hlda    TEMP=600 LABEL=ghlda

<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ARG=hlda       GRID_MIN=1.0 GRID_MAX=9.0         GRID_BIN=4000    BANDWIDTH=0.01      LOGWEIGHTS=bias LABEL=hhlda
<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ARG=hlda       GRID_MIN=1.0 GRID_MAX=9.0         GRID_BIN=4000    BANDWIDTH=0.01      LOGWEIGHTS=bias,ghlda   LABEL=hhldag

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=hhlda     TEMP=600 LABEL=fhlda
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=hhldag     TEMP=600 LABEL=fhldag

<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=fhlda   FILE=feshlda   STRIDE=500000
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=fhldag   FILE=feshldag   STRIDE=500000

<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=d4,d6,hlda,b1.bias,b1.rct STRIDE=200 FILE=colvar

</pre>{% endraw %}
