**Project ID:** [plumID:21.013]({{ '/' | absolute_url }}eggs/21/013/)  
**Source:** ch4-diss/ni111-bend/plumed.inp  
**Originally used with PLUMED version:** 2.6  
**Stable:** [raw zipped stdout](plumed.inp.plumed.stdout.txt.zip) - [stderr](plumed.inp.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.inp.plumed_master.stdout.txt.zip) - [stderr](plumed.inp.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> LENGTH=A TIME=fs ENERGY=kcal/mol

<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_a_d.html">LOAD</a> FILE=../../data/ReweightGeomFES.cpp

<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=66-69 GROUPB=65    MAX={BETA=0.010} LABEL=d1
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=65    GROUPB=1-64  MIN={BETA=100.0} LESS_THAN={RATIONAL R_0=2.5} LABEL=metalc
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=66-69 GROUPB=1-64  MIN={BETA=100.0} LESS_THAN={RATIONAL R_0=2.0} LABEL=metalh
<a href="https://plumed.github.io/doc-master/user-doc/html/_a_n_g_l_e_s.html">ANGLES</a>    GROUPA=65    GROUPB=66-69 BETWEEN={GAUSSIAN LOWER=0.5pi UPPER=0.7pi} SWITCH={RATIONAL D_0=1.50 R_0=0.25} LABEL=ang
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIESA=65    SPECIESB=66-69 R_0=1.75 NN=12        MEAN             LABEL=d3

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1.max,metalc.lessthan,metalh.lessthan,ang.between COEFFICIENTS=0.952,0.225,-0.091,-0.187 PERIODIC=NO LABEL=cv

<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=metalc.min,cv       AT=4.00,5.0  KAPPA=100,1 LABEL=wall1
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_w_a_l_l_s.html">UWALLS</a>      DATA=d1                 AT=1.80      KAPPA=250   LABEL=wall2
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=d3.mean,ang.between AT=2.95,1.25 KAPPA=1000,1000  LABEL=wall3

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_x_t_e_r_n_a_l.html">EXTERNAL</a> ARG=ang.between FILE=extbias LABEL=external

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
  ARG=cv
  SIGMA=0.05
  HEIGHT=0.25
  PACE=1000
  BIASFACTOR=25
  TEMP=500
  GRID_MIN=-3.0
  GRID_MAX=3.0
  GRID_BIN=1200
  CALC_RCT
  RCT_USTRIDE=1
  LABEL=b1
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__m_e_t_a_d.html">REWEIGHT_METAD</a>   TEMP=500 LABEL=bias
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__g_e_o_m_f_e_s.html">REWEIGHT_GEOMFES</a> TEMP=500 ARG=cv              LABEL=gcv
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__g_e_o_m_f_e_s.html">REWEIGHT_GEOMFES</a> TEMP=500 ARG=d1.max          LABEL=g1
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__g_e_o_m_f_e_s.html">REWEIGHT_GEOMFES</a> TEMP=500 ARG=metalc.lessthan LABEL=g2
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__g_e_o_m_f_e_s.html">REWEIGHT_GEOMFES</a> TEMP=500 ARG=ang.between     LABEL=g3
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__b_i_a_s.html">REWEIGHT_BIAS</a>    TEMP=500 ARG=wall1.bias,wall2.bias LABEL=wbias

<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ...
  ARG=cv
  GRID_MIN=-3.0
  GRID_MAX=3.0
  GRID_BIN=6000
  BANDWIDTH=0.01
  LOGWEIGHTS=bias,wbias
  CLEAR=5000000
  LABEL=hh
... <a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ...
  ARG=cv
  GRID_MIN=-3.0
  GRID_MAX=3.0
  GRID_BIN=6000
  BANDWIDTH=0.01
  LOGWEIGHTS=bias,wbias,gcv
  CLEAR=5000000
  LABEL=hhg
... <a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ...
  ARG=d1.max
  GRID_MIN=1.0
  GRID_MAX=3.5
  GRID_BIN=2500
  BANDWIDTH=0.01
  LOGWEIGHTS=bias,wbias,g1
  CLEAR=5000000
  LABEL=hh1
... <a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ...
  ARG=metalc.lessthan
  GRID_MIN=0.0
  GRID_MAX=5.0
  GRID_BIN=2500
  BANDWIDTH=0.02
  LOGWEIGHTS=bias,wbias,g2
  CLEAR=5000000
  LABEL=hh2
... <a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ...
  ARG=ang.between
  GRID_MIN=1.5
  GRID_MAX=4.5
  GRID_BIN=1500
  BANDWIDTH=0.02
  LOGWEIGHTS=bias,wbias,g3
  CLEAR=5000000
  LABEL=hh3
... <a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=hh  TEMP=500.0 LABEL=ff
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=hhg TEMP=500.0 LABEL=ffg
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=hh1 TEMP=500.0 LABEL=ff1
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=hh2 TEMP=500.0 LABEL=ff2
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=hh3 TEMP=500.0 LABEL=ff3

<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=ff  FILE=fes  STRIDE=1000000
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=ffg FILE=fesg STRIDE=1000000
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=ff1 FILE=fes1 STRIDE=1000000
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=ff2 FILE=fes2 STRIDE=1000000
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=ff3 FILE=fes3 STRIDE=1000000

<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=100000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=d1.max,metalc.lessthan,metalh.lessthan,ang.between,d3.mean,cv,b1.bias,b1.rct STRIDE=10000 FILE=colvar

</pre>{% endraw %}
