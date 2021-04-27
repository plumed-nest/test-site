**Project ID:** [plumID:19.054]({{ '/' | absolute_url }}eggs/19/054/)  
**Source:** plumed.dat  
**Originally used with PLUMED version:** 2.3  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> LENGTH=A TIME=0.001  <span style="color:blue">#Amstroeng, hartree, fs</span>

ene: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a>
d1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1,2 NOPBC 
d5: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1,6 NOPBC

c1:  <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d5 COEFFICIENTS=0.500,-0.500 PERIODIC=NO

h1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=2,3 NOPBC
h2: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=2,4 NOPBC
h3: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=2,5 NOPBC

<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=d1 AT=+4.0 KAPPA=150.0 EXP=2 LABEL=uwall_1
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=d5 AT=+4.0 KAPPA=150.0 EXP=2 LABEL=uwall_2
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=h1 AT=+1.7 KAPPA=150.0 EXP=2 LABEL=lwall_1
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=h2 AT=+1.7 KAPPA=150.0 EXP=2 LABEL=lwall_2
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=h3 AT=+1.7 KAPPA=150.0 EXP=2 LABEL=lwall_3


<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
 LABEL=metad
 ARG=c1
 PACE=50
 HEIGHT=2.0
 SIGMA=0.1
 FILE=HILLS
 BIASFACTOR=50
 TEMP=300.0
 CALC_RCT
 GRID_MIN=-4
 GRID_MAX=+4
 GRID_BIN=1000
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>


<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=1 FILE=COLVAR ARG=d1,d5,c1,metad.*,ene
<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=1

</pre>{% endraw %}
