**Project ID:** [plumID:20.018]({{ '/' | absolute_url }}eggs/20/018/)  
**Source:** da-wt/plumed.inp  
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

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=4 GROUPB=5 D_0=1.0 R_0=1.0 NN=1 LABEL=cn1
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=1 GROUPB=6 D_0=1.0 R_0=1.0 NN=1 LABEL=cn2

<a href="https://plumed.github.io/doc-master/user-doc/html/_d_e_n_s_i_t_y.html">DENSITY</a> SPECIES=5,6 LABEL=ethylene
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_e_n_s_i_t_y.html">DENSITY</a> SPECIES=1-4 LABEL=diene

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1-4 LABEL=mol1
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=5-6 LABEL=mol2

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t__m_a_t_r_i_x.html">CONTACT_MATRIX</a> ...
  ATOMS=ethylene,diene
  SWITCH11={RATIONAL D_0=0.0 R_0=2.65}
  SWITCH12={RATIONAL D_0=0.0 R_0=2.65}
  SWITCH22={RATIONAL D_0=0.0 R_0=2.65}
  LABEL=mat1
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t__m_a_t_r_i_x.html">CONTACT_MATRIX</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t__m_a_t_r_i_x.html">CONTACT_MATRIX</a> ...
  ATOMS=ethylene,diene
  SWITCH11={RATIONAL D_0=0.0 R_0=2.12 NN=24}
  SWITCH12={RATIONAL D_0=0.0 R_0=2.12 NN=24}
  SWITCH22={RATIONAL D_0=0.0 R_0=2.12 NN=24}
  LABEL=mat2
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t__m_a_t_r_i_x.html">CONTACT_MATRIX</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIESA=ethylene SPECIESB=diene MEAN SWITCH={GAUSSIAN D_0=1.8 R_0=0.3} LABEL=cn

<a href="https://plumed.github.io/doc-master/user-doc/html/_s_p_r_i_n_t.html">SPRINT</a> MATRIX=mat1 LABEL=ss1
<a href="https://plumed.github.io/doc-master/user-doc/html/_s_p_r_i_n_t.html">SPRINT</a> MATRIX=mat2 LABEL=ss2
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=mol1,mol2 LABEL=dist
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3,d4,d6 COEFFICIENTS=-0.05,0.21,-0.08,0.69,0.69 PERIODIC=NO LABEL=hlda
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=cn1,cn2 COEFFICIENTS=0.5,0.5 PERIODIC=NO LABEL=simple
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=ss1.coord-0,ss1.coord-1 COEFFICIENTS=0.5,0.5 PERIODIC=NO LABEL=sprnt1
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=ss2.coord-0,ss2.coord-1 COEFFICIENTS=0.5,0.5 PERIODIC=NO LABEL=sprnt2

<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=d4,d6 AT=5.0,5.0 KAPPA=50,50 LABEL=walls
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=dist,sprnt1,sprnt2,cn.mean,simple AT=0,0,0,0,0 KAPPA=50,50,50,50,50 LABEL=fake

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
  ARG=hlda
  SIGMA=0.15
  HEIGHT=1.0
  PACE=1000
  BIASFACTOR=25
  TEMP=600
  GRID_MIN=1.0
  GRID_MAX=9.0
  GRID_BIN=1600
  CALC_RCT
  RCT_USTRIDE=1
  RESTART=YES
  LABEL=b1
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__b_i_a_s.html">REWEIGHT_BIAS</a>    ARG=b1.bias TEMP=600 LABEL=bias
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__g_e_o_m_f_e_s.html">REWEIGHT_GEOMFES</a> ARG=d4      TEMP=600 LABEL=gd4
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__g_e_o_m_f_e_s.html">REWEIGHT_GEOMFES</a> ARG=hlda    TEMP=600 LABEL=ghlda
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__g_e_o_m_f_e_s.html">REWEIGHT_GEOMFES</a> ARG=sprnt1  TEMP=600 LABEL=gsprnt1
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__g_e_o_m_f_e_s.html">REWEIGHT_GEOMFES</a> ARG=sprnt2  TEMP=600 LABEL=gsprnt2
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__g_e_o_m_f_e_s.html">REWEIGHT_GEOMFES</a> ARG=cn.mean TEMP=600 LABEL=gcn
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__g_e_o_m_f_e_s.html">REWEIGHT_GEOMFES</a> ARG=simple  TEMP=600 LABEL=gsimple
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__g_e_o_m_f_e_s.html">REWEIGHT_GEOMFES</a> ARG=d4,d6   TEMP=600 LABEL=g2d

<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ARG=d4         GRID_MIN=1.0 GRID_MAX=6.0         GRID_BIN=2000    BANDWIDTH=0.02      LOGWEIGHTS=bias LABEL=hd4
<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ARG=hlda       GRID_MIN=1.0 GRID_MAX=9.0         GRID_BIN=4000    BANDWIDTH=0.01      LOGWEIGHTS=bias LABEL=hhlda
<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ARG=sprnt1     GRID_MIN=0.0 GRID_MAX=4.0         GRID_BIN=2000    BANDWIDTH=0.02      LOGWEIGHTS=bias LABEL=hsprnt1
<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ARG=sprnt2     GRID_MIN=-0.1 GRID_MAX=2.4        GRID_BIN=2500    BANDWIDTH=0.02      LOGWEIGHTS=bias LABEL=hsprnt2
<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ARG=simple     GRID_MIN=0.1 GRID_MAX=0.8         GRID_BIN=3500    BANDWIDTH=0.001     LOGWEIGHTS=bias LABEL=hsimple
<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ARG=d4,d6      GRID_MIN=1.0,1.0 GRID_MAX=2.0,2.0 GRID_BIN=100,100 BANDWIDTH=0.04,0.04 LOGWEIGHTS=bias LABEL=h2db
<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ARG=d4,d6      GRID_MIN=2.0,2.0 GRID_MAX=6.0,6.0 GRID_BIN=80,80   BANDWIDTH=0.20,0.20 LOGWEIGHTS=bias LABEL=h2dd
<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ARG=d4,d6      GRID_MIN=2.0,2.0 GRID_MAX=2.2,2.2 GRID_BIN=100,100 BANDWIDTH=0.02,0.02 LOGWEIGHTS=bias LABEL=h2d
<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ARG=d4         GRID_MIN=1.0 GRID_MAX=6.0         GRID_BIN=2000    BANDWIDTH=0.02      LOGWEIGHTS=bias,gd4     LABEL=hd4g
<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ARG=hlda       GRID_MIN=1.0 GRID_MAX=9.0         GRID_BIN=4000    BANDWIDTH=0.01      LOGWEIGHTS=bias,ghlda   LABEL=hhldag
<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ARG=sprnt1     GRID_MIN=0.0 GRID_MAX=4.0         GRID_BIN=2000    BANDWIDTH=0.02      LOGWEIGHTS=bias,gsprnt1 LABEL=hsprnt1g
<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ARG=sprnt2     GRID_MIN=-0.1 GRID_MAX=2.4        GRID_BIN=2500    BANDWIDTH=0.02      LOGWEIGHTS=bias,gsprnt2 LABEL=hsprnt2g
<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ARG=simple     GRID_MIN=0.1 GRID_MAX=0.8         GRID_BIN=3500    BANDWIDTH=0.001     LOGWEIGHTS=bias,gsimple LABEL=hsimpleg
<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ARG=d4,d6      GRID_MIN=2.0,2.0 GRID_MAX=2.2,2.2 GRID_BIN=100,100 BANDWIDTH=0.02,0.02 LOGWEIGHTS=bias,g2d     LABEL=h2dg

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=hd4       TEMP=600 LABEL=fd4
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=hhlda     TEMP=600 LABEL=fhlda
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=hsprnt1   TEMP=600 LABEL=fsprnt1
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=hsprnt2   TEMP=600 LABEL=fsprnt2
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=hsimple   TEMP=600 LABEL=fsimple
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=h2db      TEMP=600 LABEL=f2db
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=h2dd      TEMP=600 LABEL=f2dd
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=h2d       TEMP=600 LABEL=f2d
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=hd4g       TEMP=600 LABEL=fd4g
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=hhldag     TEMP=600 LABEL=fhldag
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=hsprnt1g   TEMP=600 LABEL=fsprnt1g
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=hsprnt2g   TEMP=600 LABEL=fsprnt2g
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=hsimpleg   TEMP=600 LABEL=fsimpleg
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=h2dg       TEMP=600 LABEL=f2dg

<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=fd4     FILE=fesd4     STRIDE=5000000
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=fhlda   FILE=feshlda   STRIDE=5000000
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=fsprnt1 FILE=fessprnt1 STRIDE=5000000
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=fsprnt2 FILE=fessprnt2 STRIDE=5000000
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=fsimple FILE=fessimple STRIDE=5000000
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=f2db    FILE=fes2db    STRIDE=5000000
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=f2dd    FILE=fes2dd    STRIDE=5000000
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=f2d     FILE=fes2d     STRIDE=5000000
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=fd4g     FILE=fesd4g     STRIDE=5000000
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=fhldag   FILE=feshldag   STRIDE=5000000
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=fsprnt1g FILE=fessprnt1g STRIDE=5000000
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=fsprnt2g FILE=fessprnt2g STRIDE=5000000
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=fsimpleg FILE=fessimpleg STRIDE=5000000
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=f2dg     FILE=fes2dg     STRIDE=5000000

<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=d4,d6,hlda,dist,cn.mean,sprnt1,sprnt2,b1.bias,b1.rct STRIDE=200 FILE=colvar

</pre>{% endraw %}
