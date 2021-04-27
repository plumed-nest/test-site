**Project ID:** [plumID:20.021]({{ '/' | absolute_url }}eggs/20/021/)  
**Source:** plumed_K10.dat  
**Originally used with PLUMED version:** 2.6  
**Stable:** [raw zipped stdout](plumed_K10.dat.plumed.stdout.txt.zip) - [stderr](plumed_K10.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_K10.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_K10.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">MOLINFO</a> STRUCTURE=./ref.pdb 
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=1-661,661-500:-1,1300-1475,1475-662:-1


<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> ...
PAIR NOPBC
LABEL=pv-2067
SWITCH={RATIONAL R_0=0.65 D_MAX=1.3} NLIST NL_CUTOFF=1.4 NL_STRIDE=20
GROUPA=755,755,755,755,755,755,755,755,758,758,758,758,758,758,758,758,758,758,758,758,758,758,758,758,760,760,760,760,760,760,760,760,760,760,760,760,760,760,760,760,760,760,764,764,764,764,764,764,764,764,764,764,764,764,
GROUPB=717,808,830,832,1245,1247,1251,1288,278,808,811,813,817,827,830,832,836,1245,1247,1288,1298,1310,1359,1362,278,808,811,813,817,827,830,832,836,1245,1247,1288,1298,1301,1308,1310,1359,1362,278,830,832,836,1247,1288,1298,1359,1362,1365,1366,1367,
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a>

rpv-2067: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=pv-2067 SLOPE=0 KAPPA=10. AT=22.68

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> ...
PAIR NOPBC
LABEL=pv-2070
SWITCH={RATIONAL R_0=0.65 D_MAX=1.3} NLIST NL_CUTOFF=1.4 NL_STRIDE=20
GROUPA=808,808,808,808,808,808,808,808,808,808,808,808,808,808,808,811,811,811,811,811,811,811,811,811,811,811,811,811,811,811,811,811,811,813,813,813,813,813,813,813,813,813,813,813,813,813,813,813,813,813,813,813,813,817,817,817,817,817,817,817,817,817,817,817,817,817,817,817,817,817,817,
GROUPB=755,758,760,863,876,878,1074,1080,1126,1128,1132,1135,1247,1251,1310,436,758,760,878,1074,1076,1080,1126,1128,1135,1145,1148,1150,1154,1247,1251,1308,1310,436,758,760,1074,1080,1126,1128,1132,1145,1148,1150,1154,1245,1247,1251,1298,1301,1306,1308,1310,274,436,758,760,887,890,892,896,1074,1076,1080,1128,1145,1154,1301,1306,1308,1310,
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a>

rpv-2070: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=pv-2070 SLOPE=0 KAPPA=10. AT=31.95

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> ...
PAIR NOPBC
LABEL=pv-2087
SWITCH={RATIONAL R_0=0.65 D_MAX=1.3} NLIST NL_CUTOFF=1.4 NL_STRIDE=20
GROUPA=1090,1090,1090,1090,1093,1093,1093,1093,1093,1093,1093,1095,1095,1095,1095,1095,1095,1099,1099,1099,1099,1099,1099,
GROUPB=429,497,501,1040,429,492,495,497,501,1164,1170,427,429,492,495,497,501,429,492,495,497,501,1170,
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a>

rpv-2087: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=pv-2087 SLOPE=0 KAPPA=10. AT=20.93

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> ...
PAIR NOPBC
LABEL=pv-2096
SWITCH={RATIONAL R_0=0.65 D_MAX=1.3} NLIST NL_CUTOFF=1.4 NL_STRIDE=20
GROUPA=1242,1242,1242,1242,1242,1242,1242,1242,1242,1242,1245,1245,1245,1245,1245,1245,1245,1245,1245,1245,1245,1245,1245,1245,1245,1245,1247,1247,1247,1247,1247,1247,1247,1247,1247,1247,1247,1247,1247,1251,1251,1251,1251,1251,1251,1251,1251,1251,1251,1251,1251,1251,1251,1251,1251,
GROUPB=700,703,745,1148,1150,1197,1200,1201,1202,1288,703,745,755,758,760,813,1132,1145,1148,1150,1197,1200,1201,1202,1288,1298,703,745,755,758,760,764,808,811,813,1150,1202,1288,1298,745,755,808,811,813,1126,1128,1132,1135,1145,1148,1150,1197,1200,1201,1202,
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a>

rpv-2096: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=pv-2096 SLOPE=0 KAPPA=10. AT=44.55

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> ...
PAIR NOPBC
LABEL=pv-2099
SWITCH={RATIONAL R_0=0.65 D_MAX=1.3} NLIST NL_CUTOFF=1.4 NL_STRIDE=20
GROUPA=1288,1288,1288,1288,1288,1288,1288,1288,1288,1288,1288,1288,
GROUPB=700,703,711,755,758,760,764,1242,1245,1247,1337,1362,
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a>

rpv-2099: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=pv-2099 SLOPE=0 KAPPA=10. AT=.720

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> ...
PAIR NOPBC
LABEL=pv-1048
SWITCH={RATIONAL R_0=0.65 D_MAX=1.3} NLIST NL_CUTOFF=1.4 NL_STRIDE=20
GROUPA=141,141,141,141,144,144,144,146,146,146,
GROUPB=194,197,198,199,197,198,199,197,198,199,
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a>

rpv-1048: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=pv-1048 SLOPE=0 KAPPA=10. AT=3.60

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> ...
PAIR NOPBC
LABEL=pv-1049
SWITCH={RATIONAL R_0=0.65 D_MAX=1.3} NLIST NL_CUTOFF=1.4 NL_STRIDE=20
GROUPA=160,160,160,160,160,160,160,163,163,163,163,163,163,165,165,165,165,165,169,169,169,169,169,169,169,
GROUPB=208,211,213,777,780,781,782,211,213,777,780,781,782,774,777,780,781,782,211,213,774,777,780,781,782,
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a>

rpv-1049: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=pv-1049 SLOPE=0 KAPPA=10. AT=7.75

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> ...
PAIR NOPBC
LABEL=pv-1055
SWITCH={RATIONAL R_0=0.65 D_MAX=1.3} NLIST NL_CUTOFF=1.4 NL_STRIDE=20
GROUPA=250,250,250,250,250,250,250,250,250,250,250,253,253,253,253,253,253,253,253,253,253,253,253,253,255,255,255,255,255,255,255,255,255,255,259,259,259,259,259,259,259,259,259,259,259,259,259,259,259,259,
GROUPB=208,211,217,299,302,316,827,830,832,836,896,208,217,310,316,827,830,836,887,890,896,906,909,912,299,310,316,887,890,896,906,909,912,915,208,211,217,316,827,830,832,836,887,890,892,896,906,909,912,915,
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a>

rpv-1055: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=pv-1055 SLOPE=0 KAPPA=10. AT=41.50

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> ...
PAIR NOPBC
LABEL=pv-1067
SWITCH={RATIONAL R_0=0.65 D_MAX=1.3} NLIST NL_CUTOFF=1.4 NL_STRIDE=20
GROUPA=427,427,427,427,427,427,427,427,427,427,427,429,429,429,429,429,429,429,429,429,429,429,429,429,433,433,433,433,433,433,433,433,433,436,436,436,436,436,436,436,436,436,436,436,436,436,436,436,436,436,436,436,436,436,
GROUPB=492,495,501,1076,1095,1145,1148,1154,1304,1306,1308,492,495,501,1074,1076,1090,1093,1095,1099,1145,1148,1154,1306,383,386,392,1076,1154,1304,1306,1308,1310,383,386,388,392,811,813,817,892,896,1074,1076,1080,1145,1148,1154,1301,1302,1304,1306,1308,1310,
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a>

rpv-1067: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=pv-1067 SLOPE=0 KAPPA=10. AT=12.42

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> ...
PAIR NOPBC
LABEL=pv-1047
SWITCH={RATIONAL R_0=0.65 D_MAX=1.3} NLIST NL_CUTOFF=1.4 NL_STRIDE=20
GROUPA=131,131,
GROUPB=179,182,
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a>

rpv-1047: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=pv-1047 SLOPE=0 KAPPA=10. AT=.42

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> ...
PAIR NOPBC
LABEL=pv-1054
SWITCH={RATIONAL R_0=0.65 D_MAX=1.3} NLIST NL_CUTOFF=1.4 NL_STRIDE=20
GROUPA=239,239,239,239,239,239,239,239,239,242,242,242,242,242,242,242,
GROUPB=288,291,299,302,1431,1432,1433,1435,1437,291,302,1431,1432,1433,1435,1437,
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a>

rpv-1054: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=pv-1054 SLOPE=0 KAPPA=10. AT=3.84

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> ...
PAIR NOPBC
LABEL=pv-1062
SWITCH={RATIONAL R_0=0.65 D_MAX=1.3} NLIST NL_CUTOFF=1.4 NL_STRIDE=20
GROUPA=351,351,351,351,351,354,354,354,354,357,357,357,357,357,358,358,358,
GROUPB=324,327,328,329,402,327,328,329,402,402,467,469,470,473,469,470,473,
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a>

rpv-1062: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=pv-1062 SLOPE=0 KAPPA=10. AT=5.27

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> ...
PAIR NOPBC
LABEL=pv-1065
SWITCH={RATIONAL R_0=0.65 D_MAX=1.3} NLIST NL_CUTOFF=1.4 NL_STRIDE=20
GROUPA=402,402,402,402,402,402,402,402,402,402,402,402,
GROUPB=351,354,357,446,458,461,464,467,469,470,473,482,
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a>

rpv-1065: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=pv-1065 SLOPE=0 KAPPA=10. AT=.60










stat: <a href="https://plumed.github.io/doc-master/user-doc/html/_s_t_a_t_s.html">STATS</a> ARG=pv-2067,pv-2070,pv-2087,pv-2096,pv-2099,pv-1048,pv-1049,pv-1055,pv-1067,pv-1047,pv-1054,pv-1062,pv-1065 PARAMETERS=22.68,31.95,20.93,44.55,0.72,3.60,7.75,41.50,12.42,0.42,3.84,5.27,0.60
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=stat.* FILE=STAT STRIDE=500
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=pv-2067,pv-2070,pv-2087,pv-2096,pv-2099,pv-1048,pv-1049,pv-1055,pv-1067,pv-1047,pv-1054,pv-1062,pv-1065 FILE=COORDINATION STRIDE=500
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=rpv-2067.bias,rpv-2070.bias,rpv-2087.bias,rpv-2096.bias,rpv-2099.bias,rpv-1048.bias,rpv-1049.bias,rpv-1055.bias,rpv-1067.bias,rpv-1047.bias,rpv-1054.bias,rpv-1062.bias,rpv-1065.bias FILE=RESTRAINTS STRIDE=500
</pre>{% endraw %}
