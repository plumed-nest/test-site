**Project ID:** [plumID:20.030]({{ '/' | absolute_url }}eggs/20/030/)  
**Source:** plumed2.dat  
**Originally used with PLUMED version:** 2.6  
**Stable:** [raw zipped stdout](plumed2.dat.plumed.stdout.txt.zip) - [stderr](plumed2.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed2.dat.plumed_master.stdout.txt.zip) - [stderr](plumed2.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">MOLINFO</a> STRUCTURE=ref.pdb
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=1-1571

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> ...
PAIR NOPBC
LABEL=allpv-76
SWITCH={RATIONAL R_0=0.75 D_MAX=1.5 NN=18 MM=23} NLIST NL_CUTOFF=1.6 NL_STRIDE=20
GROUPA=1305,1308,1309,1310,1305,1308,1309,1309,1305,1308,1309,1305,1308,1309,1310,1305,1308,1309,1310,1308,1309,1310,1308,1309,1310,1308,1309,1310,1309,1309,1310,1310,1310,1310,1305,1305,1308,1308,1308,1308,1309,1309,1309,1309,1310,1310,1310,1310,
GROUPB=246,246,246,246,249,249,249,258,256,256,256,258,258,258,258,266,266,266,266,269,269,269,281,281,281,283,283,283,293,299,893,896,899,902,1357,1381,1357,1379,1380,1381,1357,1360,1379,1381,1376,1379,1380,1381,
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a>  LABEL=pv-76  ARG=allpv-76 COEFFICIENTS=0.0208333 PERIODIC=NO
rpv-76: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=pv-76 SLOPE=0 KAPPA=50000. AT=0.28

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> ...
PAIR NOPBC
LABEL=allpv-39
SWITCH={RATIONAL R_0=0.75 D_MAX=1.5 NN=18 MM=23} NLIST NL_CUTOFF=1.6 NL_STRIDE=20
GROUPA=684,684,684,684,684,684,686,686,690,690,690,
GROUPB=743,757,760,1347,1390,1393,1390,1393,1347,1390,1393,
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a>  LABEL=pv-39  ARG=allpv-39 COEFFICIENTS=0.0909091 PERIODIC=NO
rpv-39: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=pv-39 SLOPE=0 KAPPA=50000. AT=0.42

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> ...
PAIR NOPBC
LABEL=allpv-78
SWITCH={RATIONAL R_0=0.75 D_MAX=1.5 NN=18 MM=23} NLIST NL_CUTOFF=1.6 NL_STRIDE=20
GROUPA=1338,1338,1338,1347,1347,1338,1341,1343,1347,1341,1343,1338,1338,1338,1341,1341,1347,1347,
GROUPB=594,596,600,684,690,1284,1284,1284,1284,1287,1287,1295,1390,1393,1390,1393,1390,1393,
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a>  LABEL=pv-78  ARG=allpv-78 COEFFICIENTS=0.0555556 PERIODIC=NO
rpv-78: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=pv-78 SLOPE=0 KAPPA=50000. AT=0.49

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> ...
PAIR NOPBC
LABEL=allpv-81
SWITCH={RATIONAL R_0=0.75 D_MAX=1.5 NN=18 MM=23} NLIST NL_CUTOFF=1.6 NL_STRIDE=20
GROUPA=1390,1393,1390,1393,1390,1393,1390,1393,1390,1393,1393,1393,1393,1390,1393,1393,1390,1393,1390,1393,1390,1393,1390,1390,
GROUPB=684,684,686,686,690,690,743,743,745,745,757,760,762,824,824,1319,1338,1338,1341,1341,1347,1347,1435,1441,
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a>  LABEL=pv-81  ARG=allpv-81 COEFFICIENTS=0.0416667 PERIODIC=NO
rpv-81: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=pv-81 SLOPE=0 KAPPA=50000. AT=0.51

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> ...
PAIR NOPBC
LABEL=allpv-29
SWITCH={RATIONAL R_0=0.75 D_MAX=1.5 NN=18 MM=23} NLIST NL_CUTOFF=1.6 NL_STRIDE=20
GROUPA=517,519,514,514,514,514,514,514,517,517,517,517,517,517,519,519,519,519,519,519,523,523,523,523,
GROUPB=375,375,450,569,1360,1362,1366,1401,569,1360,1401,1416,1419,1421,1360,1401,1416,1419,1421,1425,1401,1404,1416,1482,
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a>  LABEL=pv-29  ARG=allpv-29 COEFFICIENTS=0.0416667 PERIODIC=NO
rpv-29: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=pv-29 SLOPE=0 KAPPA=50000. AT=0.74

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> ...
PAIR NOPBC
LABEL=allpv-47
SWITCH={RATIONAL R_0=0.75 D_MAX=1.5 NN=18 MM=23} NLIST NL_CUTOFF=1.6 NL_STRIDE=20
GROUPA=824,824,824,824,824,824,824,824,824,824,824,824,
GROUPB=745,757,905,1319,1322,1324,1376,1379,1390,1393,1435,1441,
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a>  LABEL=pv-47  ARG=allpv-47 COEFFICIENTS=0.0833333 PERIODIC=NO
rpv-47: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=pv-47 SLOPE=0 KAPPA=50000. AT=0.80

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> ...
PAIR NOPBC
LABEL=allpv-71
SWITCH={RATIONAL R_0=0.75 D_MAX=1.5 NN=18 MM=23} NLIST NL_CUTOFF=1.6 NL_STRIDE=20
GROUPA=1241,1239,1241,1239,1241,1239,1241,1239,1241,1241,1236,1239,1241,
GROUPB=591,594,594,596,596,600,600,1157,1157,1159,1295,1295,1295,
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a>  LABEL=pv-71  ARG=allpv-71 COEFFICIENTS=0.0769231 PERIODIC=NO
rpv-71: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=pv-71 SLOPE=0 KAPPA=50000. AT=0.86

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> ...
PAIR NOPBC
LABEL=allpv-58
SWITCH={RATIONAL R_0=0.75 D_MAX=1.5 NN=18 MM=23} NLIST NL_CUTOFF=1.6 NL_STRIDE=20
GROUPA=1015,1017,1015,1017,1024,1015,1017,1021,1024,1017,1015,1017,1021,1024,1024,1024,1024,1015,1015,1021,
GROUPB=258,258,256,256,450,453,453,453,453,455,459,459,459,459,469,472,475,1051,1057,1057,
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a>  LABEL=pv-58  ARG=allpv-58 COEFFICIENTS=0.05 PERIODIC=NO
rpv-58: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=pv-58 SLOPE=0 KAPPA=50000. AT=0.90

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> ...
PAIR NOPBC
LABEL=allpv-86
SWITCH={RATIONAL R_0=0.75 D_MAX=1.5 NN=18 MM=23} NLIST NL_CUTOFF=1.6 NL_STRIDE=20
GROUPA=1482,1473,1473,
GROUPB=523,1416,1419,
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a>  LABEL=pv-86  ARG=allpv-86 COEFFICIENTS=0.333333 PERIODIC=NO
rpv-86: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=pv-86 SLOPE=0 KAPPA=50000. AT=0.99

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> ...
PAIR NOPBC
LABEL=allpv-26
SWITCH={RATIONAL R_0=0.75 D_MAX=1.5 NN=18 MM=23} NLIST NL_CUTOFF=1.6 NL_STRIDE=20
GROUPA=453,455,459,453,455,459,453,455,459,453,455,459,455,455,455,450,450,453,455,450,453,455,459,450,450,450,453,453,453,453,453,453,455,455,455,455,459,459,459,459,459,
GROUPB=246,246,246,249,249,249,258,258,258,256,256,256,293,295,299,366,372,372,372,375,375,375,375,514,980,1024,980,1015,1017,1021,1024,1366,980,1017,1362,1366,980,1015,1017,1021,1024,
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a>  LABEL=pv-26  ARG=allpv-26 COEFFICIENTS=0.0243902 PERIODIC=NO
rpv-26: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=pv-26 SLOPE=0 KAPPA=50000. AT=1.00

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> ...
PAIR NOPBC
LABEL=allpv-79
SWITCH={RATIONAL R_0=0.75 D_MAX=1.5 NN=18 MM=23} NLIST NL_CUTOFF=1.6 NL_STRIDE=20
GROUPA=1357,1360,1357,1360,1362,1366,1366,1357,1360,1366,1357,1360,1362,1366,1360,1366,1366,1362,1366,1360,1362,1366,1360,1360,1362,1362,1362,1357,1360,1357,1360,1362,1357,1357,1357,1357,1360,1357,
GROUPB=246,246,249,249,249,249,254,256,256,256,258,258,258,258,295,295,453,455,455,514,514,514,517,519,533,536,538,594,594,596,596,596,600,1305,1308,1309,1309,1401,
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a>  LABEL=pv-79  ARG=allpv-79 COEFFICIENTS=0.0263158 PERIODIC=NO
rpv-79: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=pv-79 SLOPE=0 KAPPA=50000. AT=1.00

stat: <a href="https://plumed.github.io/doc-master/user-doc/html/_s_t_a_t_s.html">STATS</a> ARG=pv-76,pv-39,pv-78,pv-81,pv-29,pv-47,pv-71,pv-58,pv-86,pv-26,pv-79, PARAMETERS=0.28,0.42,0.49,0.51,0.74,0.80,0.86,0.90,0.99,1.00,1.00,
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=stat.* FILE=STAT STRIDE=500
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=pv-76,pv-39,pv-78,pv-81,pv-29,pv-47,pv-71,pv-58,pv-86,pv-26,pv-79, FILE=COORDINATION STRIDE=500
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=rpv-76.bias,rpv-39.bias,rpv-78.bias,rpv-81.bias,rpv-29.bias,rpv-47.bias,rpv-71.bias,rpv-58.bias,rpv-86.bias,rpv-26.bias,rpv-79.bias, FILE=RESTRAINTS STRIDE=500
</pre>{% endraw %}
