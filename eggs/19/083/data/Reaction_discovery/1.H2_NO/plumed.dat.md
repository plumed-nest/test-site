**Project ID:** [plumID:19.083]({{ '/' | absolute_url }}eggs/19/083/)  
**Source:** Reaction_discovery/1.H2_NO/plumed.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> LENGTH=A

N: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=1,3
O: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=2,4
H: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=5,6,7,8

hh: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIES=H SWITCH={RATIONAL D_0=0.0 R_0=1.1 NN=6 MM=8} MEAN
nn: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIES=N SWITCH={RATIONAL D_0=0.0 R_0=1.5 NN=6 MM=8} MEAN
oo: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIES=O SWITCH={RATIONAL D_0=0.0 R_0=1.7 NN=6 MM=8} MEAN
no: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIESA=N SPECIESB=O SWITCH={RATIONAL D_0=0.0 R_0=1.6 NN=6 MM=8} MIN={BETA=20.0} MAX={BETA=0.02}
on: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIESA=O SPECIESB=N SWITCH={RATIONAL D_0=0.0 R_0=1.6 NN=6 MM=8} MIN={BETA=20.0} MAX={BETA=0.02}
nh: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIESA=N SPECIESB=H SWITCH={RATIONAL D_0=0.0 R_0=1.4 NN=6 MM=8} MIN={BETA=20.0} MAX={BETA=0.02}
hn: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIESA=H SPECIESB=N SWITCH={RATIONAL D_0=0.0 R_0=1.4 NN=6 MM=8} MIN={BETA=20.0} MAX={BETA=0.02}
oh: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIESA=O SPECIESB=H SWITCH={RATIONAL D_0=0.0 R_0=1.4 NN=6 MM=8} MIN={BETA=20.0} MAX={BETA=0.02}
ho: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIESA=H SPECIESB=O SWITCH={RATIONAL D_0=0.0 R_0=1.4 NN=6 MM=8} MIN={BETA=20.0} MAX={BETA=0.02}

d1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=hh.mean COEFFICIENTS=1.00 PERIODIC=NO
d2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=nn.mean COEFFICIENTS=1.0734 PERIODIC=NO
d3: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=oo.mean COEFFICIENTS=1.6782 PERIODIC=NO
d4: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=no.max COEFFICIENTS=0.7097 PERIODIC=NO
d5: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=no.min COEFFICIENTS=0.7637 PERIODIC=NO
d6: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=on.max COEFFICIENTS=0.7121 PERIODIC=NO
d7: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=on.min COEFFICIENTS=0.7643 PERIODIC=NO
d8: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=nh.max COEFFICIENTS=0.9618 PERIODIC=NO
d9: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=nh.min COEFFICIENTS=1.1010 PERIODIC=NO
d10: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=hn.max COEFFICIENTS=1.3052 PERIODIC=NO
d11: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=hn.min COEFFICIENTS=2.5949 PERIODIC=NO
d12: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=oh.max COEFFICIENTS=0.3617 PERIODIC=NO
d13: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=oh.min COEFFICIENTS=0.4227 PERIODIC=NO
d14: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=ho.max COEFFICIENTS=0.6276 PERIODIC=NO
d15: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=ho.min COEFFICIENTS=0.8866 PERIODIC=NO

<span style="color:blue">#the following are 32,33,34</span>
svd14: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3,d4,d5,d6,d7,d8,d9,d10,d11,d12,d13,d14,d15 COEFFICIENTS=0.0,-0.02114,0.00334,-0.23391,-0.64088,0.21637,0.69767,0.00113,-0.00213,-0.00001,0.00025,0.00206,-0.00739,-0.00457,-0.02124 PERIODIC=NO
svd13: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3,d4,d5,d6,d7,d8,d9,d10,d11,d12,d13,d14,d15 COEFFICIENTS=0.0,-0.39547,0.06121,-0.20744,0.60671,-0.11341,0.47938,0.02201,-0.03897,-0.00129,0.00439,0.03726,-0.13914,-0.08409,-0.39524 PERIODIC=NO
svd12: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3,d4,d5,d6,d7,d8,d9,d10,d11,d12,d13,d14,d15 COEFFICIENTS=0.0,-0.40711,0.06514,-0.17925,0.61216,-0.15080,0.50432,0.02309,-0.04043,-0.00128,0.00438,-0.02035,-0.27076,-0.03965,-0.26189 PERIODIC=NO

dNN: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=N GROUPB=N MAX={BETA=0.02} NOPBC
dNH: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=N GROUPB=H MAX={BETA=0.02} NOPBC
dOO: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=O GROUPB=O MAX={BETA=0.02} NOPBC
wallNN: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=dNN.max AT=9.0 KAPPA=200.0 EXP=2 EPS=1 
wallNH: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=dNH.max AT=9.0 KAPPA=200.0 EXP=2 EPS=1 
wallNaN: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=dOO.max AT=9.0 KAPPA=200.0 EXP=2 EPS=1

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
   ARG=svd13 SIGMA=0.05 HEIGHT=3.0 PACE=100 LABEL=restraint 
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=* STRIDE=20 FILE=COLVAR
<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=20

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
