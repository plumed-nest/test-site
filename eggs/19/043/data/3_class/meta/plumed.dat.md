**Project ID:** [plumID:19.043]({{ '/' | absolute_url }}eggs/19/043/)  
**Source:** 3_class/meta/plumed.dat  
**Originally used with PLUMED version:** 2.3  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue">#</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> LENGTH=A TIME=0.001  <span style="color:blue">#Amstroeng, fs</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>

d1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1,2 NOPBC 
d2: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1,3 NOPBC
d3: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1,6 NOPBC

hc: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=1 GROUPB=4,5 LESS_THAN={RATIONAL R_0=2.0 NN=6 MM=12}

d4: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1,4 NOPBC
d5: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1,5 NOPBC

<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=d1 AT=+7.5  KAPPA=150.0 EXP=2 LABEL=uwall_1
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=d2 AT=+7.5  KAPPA=150.0 EXP=2 LABEL=uwall_2
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=d3 AT=+7.5  KAPPA=150.0 EXP=2 LABEL=uwall_3
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=d4 AT=+1.25 KAPPA=500.0 EXP=2 LABEL=uwall_4
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=d5 AT=+1.25 KAPPA=500.0 EXP=2 LABEL=uwall_5

comb1:  <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3 COEFFICIENTS=0.555,-0.810,0.190 PERIODIC=NO
comb2:  <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3 COEFFICIENTS=0.600,0.234,-0.765 PERIODIC=NO

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
 LABEL=metad
 ARG=comb1,comb2
 PACE=50 
 HEIGHT=2.0 
 SIGMA=0.2 
 GRID_MIN=-15,-15
 GRID_MAX=15,15
 GRID_BIN=300,300
 FILE=HILLS
 BIASFACTOR=25  
 TEMP=300.0 
 ADAPTIVE=GEOM
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>


<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=10
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=1 FILE=COLVAR ARG=d1,d2,d3,comb1,comb2,d4,d5,metad.*

</pre>{% endraw %}
