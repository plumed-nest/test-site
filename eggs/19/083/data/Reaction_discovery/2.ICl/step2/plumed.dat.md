**Project ID:** [plumID:19.083]({{ '/' | absolute_url }}eggs/19/083/)  
**Source:** Reaction_discovery/2.ICl/step2/plumed.dat  
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

svd13: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3,d4,d5,d6,d7,d8,d9,d10,d11,d12,d13,d14,d15 COEFFICIENTS=0.7435,-0.0278,-0.3230,0.0052,-0.4295,-0.0315,-0.3276,-0.0540,0.0093,0.0297,0.0162,0.1870,-0.0130,0.0911,0.0412 PERIODIC=NO  
svd11: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3,d4,d5,d6,d7,d8,d9,d10,d11,d12,d13,d14,d15 COEFFICIENTS=0.7739,-0.0297,-0.3295,-0.1430,-0.2591,-0.0257,-0.3954,-0.0026,0.0093,0.0020,-0.0007,0.1858,-0.0170,0.0995,0.0471 PERIODIC=NO  
svd9:  <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3,d4,d5,d6,d7,d8,d9,d10,d11,d12,d13,d14,d15 COEFFICIENTS=0.8395,-0.0959,-0.0923,-0.2187,-0.0523,-0.0162,-0.3158,-0.0256,0.0579,0.0008,0.0004,0.0280,0.2146,-0.0464,0.2719 PERIODIC=NO  
svd7:  <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3,d4,d5,d6,d7,d8,d9,d10,d11,d12,d13,d14,d15 COEFFICIENTS=-0.0743,-0.1207,-0.1905,-0.1565,-0.2149,0.0360,-0.4456,0.1727,-0.1967,0.0591,0.0559,0.0772,0.4405,-0.1388,0.6154 PERIODIC=NO  
svd5:  <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3,d4,d5,d6,d7,d8,d9,d10,d11,d12,d13,d14,d15 COEFFICIENTS=-0.0223,-0.1612,0.2841,-0.2182,-0.1949,-0.3663,-0.0153,-0.0309,0.0018,0.0264,-0.0796,0.4268,0.3542,0.5620,0.2033 PERIODIC=NO  
svd3:  <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3,d4,d5,d6,d7,d8,d9,d10,d11,d12,d13,d14,d15 COEFFICIENTS=-0.0043,0.3781,-0.0278,-0.3167,-0.2908,-0.6031,0.0578,0.0246,0.1205,-0.2184,0.4635,0.0417,0.0964,0.0185,0.1236 PERIODIC=NO  
svd1:  <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3,d4,d5,d6,d7,d8,d9,d10,d11,d12,d13,d14,d15 COEFFICIENTS=-0.0170,0.0092,-0.2062,-0.1258,-0.1245,-0.1567,-0.0838,0.1953,-0.1107,0.1000,0.0367,0.5470,0.3433,0.5465,0.3417 PERIODIC=NO  

sdg1filter095: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3,d4,d5,d6,d7,d8,d9,d10,d11,d12,d13,d14,d15 COEFFICIENTS=0.7429,-0.0276,-0.3225,0.0,-0.4192,-0.0218,-0.3448,-0.0248,0.0316,0.0,-0.0045,0.1832,-0.0276,0.0958,0.0550 PERIODIC=NO  
sdg1filter090: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3,d4,d5,d6,d7,d8,d9,d10,d11,d12,d13,d14,d15 COEFFICIENTS=0.7026,-0.0342,-0.3478,0.0,-0.3629,0.0,-0.3840,-0.0031,0.0186,0.0,-0.0052,0.2806,0.1303,0.0,-0.0945 PERIODIC=NO  
sdg1filter080: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3,d4,d5,d6,d7,d8,d9,d10,d11,d12,d13,d14,d15 COEFFICIENTS=0.7129,-0.0308,-0.3414,0.0,-0.3708,0.0,-0.3858,0.0,0.0141,0.0,0.0,0.2963,0.0,0.0,-0.0026 PERIODIC=NO  
sdg1filter070: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3,d4,d5,d6,d7,d8,d9,d10,d11,d12,d13,d14,d15 COEFFICIENTS=0.6918,-0.0317,-0.3351,0.0,-0.5711,0.0,0.0,0.0,-0.0040,0.0,0.0,0.2864,0.0,0.0,0.0036 PERIODIC=NO  
sdg1filter060: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3,d4,d5,d6,d7,d8,d9,d10,d11,d12,d13,d14,d15 COEFFICIENTS=0.7606,-0.0474,-0.0355,0.0,-0.6226,0.0,0.0,0.0,-0.0050,0.0,0.0,0.0,0.0,0.0,0.1741 PERIODIC=NO  

dHCl: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=H GROUPB=Cl MAX={BETA=0.02} NOPBC
dHI: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=H GROUPB=I MAX={BETA=0.02} NOPBC
dICl: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=I GROUPB=Cl MAX={BETA=0.02} NOPBC
wallHCl: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=dHCl.max AT=9.0 KAPPA=200.0 EXP=2 EPS=1
wallHI: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=dHI.max AT=9.0 KAPPA=200.0 EXP=2 EPS=1 
wallICl: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=dICl.max AT=9.0 KAPPA=200.0 EXP=2 EPS=1 

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
   ARG=svd13 SIGMA=0.05 HEIGHT=1.5 PACE=100 LABEL=restraint 
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=* STRIDE=20 FILE=COLVAR
<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=20

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
