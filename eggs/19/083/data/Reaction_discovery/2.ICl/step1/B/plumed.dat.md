**Project ID:** [plumID:19.083]({{ '/' | absolute_url }}eggs/19/083/)  
**Source:** Reaction_discovery/2.ICl/step1/B/plumed.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> LENGTH=A

H: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=1,2
I: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=3,5
Cl: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=4,6

hh: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIES=H SWITCH={RATIONAL D_0=0.0 R_0=1.1 NN=6 MM=8} MEAN
II: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIES=I SWITCH={RATIONAL D_0=0.0 R_0=3.0 NN=6 MM=8} MEAN
ClCl: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIES=Cl SWITCH={RATIONAL D_0=0.0 R_0=2.3 NN=6 MM=8} MEAN
HCl: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIESA=H SPECIESB=Cl SWITCH={RATIONAL D_0=0.0 R_0=1.6 NN=6 MM=8} MIN={BETA=20.0} MAX={BETA=0.02}
ClH: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIESA=Cl SPECIESB=H SWITCH={RATIONAL D_0=0.0 R_0=1.6 NN=6 MM=8} MIN={BETA=20.0} MAX={BETA=0.02}
HI: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIESA=H SPECIESB=I SWITCH={RATIONAL D_0=0.0 R_0=1.9 NN=6 MM=8} MIN={BETA=20.0} MAX={BETA=0.02}
IH: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIESA=I SPECIESB=H SWITCH={RATIONAL D_0=0.0 R_0=1.9 NN=6 MM=8} MIN={BETA=20.0} MAX={BETA=0.02}
ICl: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIESA=I SPECIESB=Cl SWITCH={RATIONAL D_0=0.0 R_0=2.6 NN=6 MM=8} MIN={BETA=20.0} MAX={BETA=0.02}
ClI: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIESA=Cl SPECIESB=I SWITCH={RATIONAL D_0=0.0 R_0=2.6 NN=6 MM=8} MIN={BETA=20.0} MAX={BETA=0.02}

d1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=hh.mean COEFFICIENTS=1.0232 PERIODIC=NO
d2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=II.mean COEFFICIENTS=1.1790 PERIODIC=NO
d3: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=ClCl.mean COEFFICIENTS=2.1364 PERIODIC=NO
d4: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=HCl.max COEFFICIENTS=0.7082 PERIODIC=NO
d5: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=HCl.min COEFFICIENTS=0.8116 PERIODIC=NO
d6: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=ClH.max COEFFICIENTS=0.6879 PERIODIC=NO
d7: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=ClH.min COEFFICIENTS=0.7994 PERIODIC=NO
d8: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=HI.max COEFFICIENTS=1.1615 PERIODIC=NO
d9: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=HI.min COEFFICIENTS=1.7905 PERIODIC=NO
d10: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=IH.max COEFFICIENTS=1.2714 PERIODIC=NO
d11: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=IH.min COEFFICIENTS=1.6849 PERIODIC=NO
d12: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=ICl.max COEFFICIENTS=0.8310 PERIODIC=NO
d13: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=ICl.min COEFFICIENTS=0.9355 PERIODIC=NO
d14: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=ClI.max COEFFICIENTS=0.8257 PERIODIC=NO
d15: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=ClI.min COEFFICIENTS=0.9352 PERIODIC=NO

sdg1full: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3,d4,d5,d6,d7,d8,d9,d10,d11,d12,d13,d14,d15 COEFFICIENTS=0.6688,-0.0250,-0.2889,-0.3031,-0.5252,0.2230,-0.1102,-0.0069,0.0331,-0.0102,-0.0103,0.1540,-0.0335,0.0968,0.0583 PERIODIC=NO

svd13m1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3,d4,d5,d6,d7,d8,d9,d10,d11,d12,d13,d14,d15 COEFFICIENTS=-0.4446,0.0049,0.0288,0.1219,0.0686,0.0886,0.0323,0.1243,0.0676,-0.0530,-0.0781,0.4969,0.3439,-0.4511,-0.4189 PERIODIC=NO  
svd13m2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3,d4,d5,d6,d7,d8,d9,d10,d11,d12,d13,d14,d15 COEFFICIENTS=-0.0450,0.0427,0.2969,-0.4559,0.4762,-0.0061,0.1473,-0.3869,-0.1632,0.2848,0.2102,-0.0487,0.2557,-0.2622,-0.1160 PERIODIC=NO  
svd11m1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3,d4,d5,d6,d7,d8,d9,d10,d11,d12,d13,d14,d15 COEFFICIENTS=-0.8075,0.0186,0.2521,0.1816,0.2349,0.0562,0.3967,0.0364,-0.0429,0.0242,-0.0034,-0.1252,-0.0373,-0.1007,-0.0662 PERIODIC=NO  
svd11m2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3,d4,d5,d6,d7,d8,d9,d10,d11,d12,d13,d14,d15 COEFFICIENTS=0.1102,0.1135,0.5696,-0.1055,0.2089,-0.1612,0.2692,-0.2625,0.2177,-0.1559,-0.0388,-0.4719,0.2804,-0.2171,0.0822 PERIODIC=NO  
svd9m1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3,d4,d5,d6,d7,d8,d9,d10,d11,d12,d13,d14,d15  COEFFICIENTS=0.7820,-0.0074,-0.0974,-0.2334,0.0800,-0.1052,-0.1291,-0.2370,0.3061,-0.0213,-0.1431,-0.0234,0.2626,-0.0026,0.2235 PERIODIC=NO  
svd9m2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3,d4,d5,d6,d7,d8,d9,d10,d11,d12,d13,d14,d15  COEFFICIENTS=0.0079,-0.2227,0.0969,-0.0597,-0.3591,0.1200,-0.5246,0.4716,-0.4417,0.1350,0.2572,0.1127,-0.0455,0.0354,0.0322 PERIODIC=NO  

  
sdg1filter075: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3,d4,d5,d6,d7,d8,d9,d10,d11,d12,d13,d14,d15 COEFFICIENTS=-0.4916,0.0056,0.0378,0.2220,0.1772,0.0,-0.0576,-0.0072,0.0050,0.0775,0.0,0.4842,0.2992,-0.4425,-0.3835 PERIODIC=NO  
sdg2filter075: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3,d4,d5,d6,d7,d8,d9,d10,d11,d12,d13,d14,d15 COEFFICIENTS=0.0269,-0.0375,-0.2456,0.3938,-0.3926,0.0,-0.1366,0.0201,-0.0019,0.0464,0.0,-0.1701,-0.5095,0.4204,0.3766 PERIODIC=NO  
sdg1filter095: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3,d4,d5,d6,d7,d8,d9,d10,d11,d12,d13,d14,d15 COEFFICIENTS=0.7429,-0.0276,-0.3225,0.0,-0.4192,-0.0218,-0.3448,-0.0248,0.0316,0.0,-0.0045,0.1832,-0.0276,0.0958,0.0550 PERIODIC=NO  
sdg1filter090: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3,d4,d5,d6,d7,d8,d9,d10,d11,d12,d13,d14,d15 COEFFICIENTS=0.7026,-0.0342,-0.3478,0.0,-0.3629,0.0,-0.3840,-0.0031,0.0186,0.0,-0.0052,0.2806,0.1303,0.0,-0.0945 PERIODIC=NO  
svd13: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3,d4,d5,d6,d7,d8,d9,d10,d11,d12,d13,d14,d15 COEFFICIENTS=0.7435,-0.0278,-0.3230,0.0052,-0.4295,-0.0315,-0.3276,-0.0540,0.0093,0.0297,0.0162,0.1870,-0.0130,0.0911,0.0412 PERIODIC=NO  
svd11: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3,d4,d5,d6,d7,d8,d9,d10,d11,d12,d13,d14,d15 COEFFICIENTS=0.7739,-0.0297,-0.3295,-0.1430,-0.2591,-0.0257,-0.3954,-0.0026,0.0093,0.0020,-0.0007,0.1858,-0.0170,0.0995,0.0471 PERIODIC=NO  

dHCl: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=H GROUPB=Cl MAX={BETA=0.02} NOPBC
dHI: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=H GROUPB=I MAX={BETA=0.02} NOPBC
dICl: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=I GROUPB=Cl MAX={BETA=0.02} NOPBC
wallHCl: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=dHCl.max AT=9.0 KAPPA=200.0 EXP=2 EPS=1
wallHI: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=dHI.max AT=9.0 KAPPA=200.0 EXP=2 EPS=1 
wallICl: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=dICl.max AT=9.0 KAPPA=200.0 EXP=2 EPS=1 

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
   ARG=svd13m1,svd13m2 SIGMA=0.05,0.05 HEIGHT=1.5 PACE=100 BIASFACTOR=60 TEMP=400.0 LABEL=restraint 
   WALKERS_N=3
   WALKERS_ID=1
   WALKERS_DIR=../
   WALKERS_RSTRIDE=50
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=* STRIDE=20 FILE=COLVAR
<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=20

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
