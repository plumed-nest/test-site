**Project ID:** [plumID:20.024]({{ '/' | absolute_url }}eggs/20/024/)  
**Source:** Hydrobromination/known_propene/plumed.dat  
**Originally used with PLUMED version:** 2.7  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_a_d.html">LOAD</a> FILE=../../GAMBES.cpp
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> LENGTH=A TIME=fs

d1:  <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=10,11 NOPBC
d2:  <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=11,1 NOPBC
d3:  <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=10,2 NOPBC
d4:  <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=11,2 NOPBC
d5:  <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=10,1 NOPBC
ene: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a>

s1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3,d4,d5 COEFFICIENTS=-0.523,0.726,0.401,-0.029,-0.193 POWERS=1,1,1,1,1 PERIODIC=NO
s2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3,d4,d5 COEFFICIENTS=0.573,-0.339,-0.183,-0.636,-0.345 POWERS=1,1,1,1,1 PERIODIC=NO

<a href="https://plumed.github.io/doc-master/user-doc/html/_g_a_m_b_e_s.html">GAMBES</a> ...
  ARG=d1 
  NSTATES=2
  FILENAME=gaussian
  PACE=500
  LABEL=ext
  BIAS_CUTOFF
  CUTOFF=100
  LAMBDA=0.1 
  TEMPERATURE=300
... <a href="https://plumed.github.io/doc-master/user-doc/html/_g_a_m_b_e_s.html">GAMBES</a>


<span style="color:blue">#..............................WALLS.................................................</span>
uwall: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=d1,d2,d3,d4,d5 AT=3.0,3.0,3.0,3.0,3.0 KAPPA=150.0,150.0,150.0,150.0,150.0  <span style="color:blue">#eps=1, exp=2, offset=0 : default values</span>

H1: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=3,4
H2: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=7,8,9
H: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=11
C_end: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=1,5
C_mid: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=2
Br: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=10
Ce1: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=1
Ce2: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=5
H_all: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=3,4,6,7,8,9,11

dCe1H1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=Ce1 GROUPB=H1 HIGHEST NOPBC
dCe2H2: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=Ce2 GROUPB=H2 HIGHEST NOPBC
dCmH1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=2,6 NOPBC
dHH: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=H_all GROUPB=H_all MIN={BETA=20} NOPBC

d13: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1,3 NOPBC
d14: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1,4 NOPBC
wallCe1H1: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=d13,d14 AT=1.4,1.4 KAPPA=150.0,150.0 EXP=2,2 EPS=1.0,1.0 OFFSET=0.2,0.2

d57: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=5,7 NOPBC
d58: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=5,8 NOPBC
d59: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=5,9 NOPBC
wallCe2H2: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=d57,d58,d59 AT=1.4,1.4,1.4 KAPPA=150.0,150.0,150.0 EXP=2,2,2 EPS=1.0,1.0,1.0 OFFSET=0.2,0.2,0.2
wallCmH1: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=dCmH1 AT=1.4 KAPPA=150.0 EXP=2 EPS=1.0 OFFSET=0.2
wallHH: <a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=dHH.* AT=1.4 KAPPA=150.0 EXP=2 EPS=1.0 <span style="color:blue">#OFFSET=1.3</span>
<span style="color:blue">##################################################</span>


<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=* STRIDE=10 FILE=COLVAR FMT=%8.4f
<span style="color:blue">#PRINT ARG=ext.probability.0,ext.probability.1,ext.probability.2 STRIDE=10 FILE=GAMBES FMT=%8.10f</span>

</pre>{% endraw %}
