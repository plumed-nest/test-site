**Project ID:** [plumID:20.018]({{ '/' | absolute_url }}eggs/20/018/)  
**Source:** na/plumed.inp  
**Originally used with PLUMED version:** 2.6-mod  
**Stable:** [raw zipped stdout](plumed.inp.plumed.stdout.txt.zip) - [stderr](plumed.inp.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.inp.plumed_master.stdout.txt.zip) - [stderr](plumed.inp.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> LENGTH=A TIME=fs ENERGY=96.485

<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_a_d.html">LOAD</a> FILE=../src/bias/ReweightGeomFES.cpp
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_a_d.html">LOAD</a> FILE=PairEntropy.cpp

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a> LABEL=ene
<a href="https://plumed.github.io/doc-master/user-doc/html/_v_o_l_u_m_e.html">VOLUME</a> LABEL=vol

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=ene,vol COEFFICIENTS=1.0,1.0/1602176.5 PERIODIC=NO LABEL=enthalpy
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=enthalpy COEFFICIENTS=1.0/250 PERIODIC=NO LABEL=sh

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIES=1-250 SWITCH={RATIONAL D_0=5.0 R_0=0.1 D_MAX=6.0} MOMENTS=2 LABEL=cn
<a href="https://plumed.github.io/doc-master/user-doc/html/_q6.html">Q6</a> SPECIES=1-250 SWITCH={RATIONAL D_0=5.0 R_0=0.1 D_MAX=6.0} MEAN LABEL=q6
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_c_a_l__a_v_e_r_a_g_e.html">LOCAL_AVERAGE</a> SPECIES=q6 SWITCH={RATIONAL D_0=5.0 R_0=0.1 D_MAX=6.0} MEAN LABEL=q6l

<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=q6l.mean AT=0.0 KAPPA=1.0 LABEL=dummy

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_a_i_r_e_n_t_r_o_p_y.html">PAIRENTROPY</a> ...
  ATOMS=1-250
  MAXR=6.5
  SIGMA=0.125
  NHIST=130
  LABEL=ss
... <a href="https://plumed.github.io/doc-master/user-doc/html/_p_a_i_r_e_n_t_r_o_p_y.html">PAIRENTROPY</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
  ARG=sh,ss
  SIGMA=0.002,0.10
  HEIGHT=0.025
  PACE=2500
  BIASFACTOR=30
  TEMP=375
  GRID_MIN=-1.10,-6.0
  GRID_MAX=-0.95,-1.0
  GRID_BIN=750,500
  CALC_RCT
  RCT_USTRIDE=1
  LABEL=b1
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__m_e_t_a_d.html">REWEIGHT_METAD</a>                TEMP=375 LABEL=bias
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__g_e_o_m_f_e_s.html">REWEIGHT_GEOMFES</a> ARG=ss       TEMP=375 LABEL=gss
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__g_e_o_m_f_e_s.html">REWEIGHT_GEOMFES</a> ARG=q6l.mean TEMP=375 LABEL=gq6l

<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ARG=ss GRID_MIN=-6.0 GRID_MAX=-1.0 GRID_BIN=1000 BANDWIDTH=0.02 LOGWEIGHTS=bias LABEL=hss
<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ARG=q6l.mean GRID_MIN=0.05 GRID_MAX=0.5 GRID_BIN=900 BANDWIDTH=0.004 LOGWEIGHTS=bias LABEL=hq6l
<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ARG=ss GRID_MIN=-6.0 GRID_MAX=-1.0 GRID_BIN=1000 BANDWIDTH=0.02 LOGWEIGHTS=bias,gss LABEL=hssg
<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ARG=q6l.mean GRID_MIN=0.05 GRID_MAX=0.5 GRID_BIN=900 BANDWIDTH=0.004 LOGWEIGHTS=bias,gq6l LABEL=hq6lg

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=hss   TEMP=375 LABEL=fss
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=hq6l  TEMP=375 LABEL=fq6l
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=hssg  TEMP=375 LABEL=fssg
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=hq6lg TEMP=375 LABEL=fq6lg

<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=fss   FILE=fesss   STRIDE=10000000
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=fq6l  FILE=fesq6l  STRIDE=10000000
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=fssg  FILE=fesssg  STRIDE=10000000
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=fq6lg FILE=fesq6lg STRIDE=10000000

<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=50000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=sh,ss,q6l.mean,b1.bias,b1.rct STRIDE=50000 FILE=colvar

</pre>{% endraw %}
