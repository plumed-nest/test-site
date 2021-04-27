**Project ID:** [plumID:19.042]({{ '/' | absolute_url }}eggs/19/042/)  
**Source:** 2_class/meta/plumed.dat  
**Originally used with PLUMED version:** 2.3  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue">#RESTART</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> LENGTH=A TIME=0.001  <span style="color:blue">#Amstroeng, hartree, fs</span>

energy: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a>


d1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1,2 NOPBC
d2: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=2,3 NOPBC
d3: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=3,4 NOPBC
d4: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=4,5 NOPBC
d5: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=5,6 NOPBC
d6: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=6,1 NOPBC

comb1:  <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3,d4,d5,d6 COEFFICIENTS=0.182,-0.456,0.106,-0.602,0.065,-0.617  PERIODIC=NO

<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=d4 AT=+5.0 KAPPA=150.0  EXP=2 LABEL=uwall_1
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=d6 AT=+5.0 KAPPA=150.0  EXP=2 LABEL=uwall_2

metad: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=comb1 PACE=100 HEIGHT=5.0 SIGMA=0.2 GRID_MIN=-15 GRID_MAX=15 GRID_BIN=2000 FILE=HILLS BIASFACTOR=80 TEMP=300.0

<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=1
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ...
 ARG=d1,d2,d3,d4,d5,d6,comb1,metad.*
 STRIDE=1
 FILE=COLVAR
... <a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a>
</pre>{% endraw %}
