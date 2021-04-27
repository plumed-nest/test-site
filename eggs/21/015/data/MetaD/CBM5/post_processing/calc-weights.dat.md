**Project ID:** [plumID:21.015]({{ '/' | absolute_url }}eggs/21/015/)  
**Source:** MetaD/CBM5/post_processing/calc-weights.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [raw zipped stdout](calc-weights.dat.plumed.stdout.txt.zip) - [stderr](calc-weights.dat.plumed.stderr)  
**Master:** [raw zipped stdout](calc-weights.dat.plumed_master.stdout.txt.zip) - [stderr](calc-weights.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=721-887

a1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=798-801 
a2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=803-807 
a3: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=832-835 
achi: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1-720 


p1: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_o_s_i_t_i_o_n.html">POSITION</a> ATOM=a1 NOPBC
p2: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_o_s_i_t_i_o_n.html">POSITION</a> ATOM=a2 NOPBC
p3: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_o_s_i_t_i_o_n.html">POSITION</a> ATOM=a3 NOPBC
pchi: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_o_s_i_t_i_o_n.html">POSITION</a> ATOM=achi NOPBC


c: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=798-801,803-807,832-835 GROUPB=1-720 R_0=0.5 NLIST NL_CUTOFF=0.7 NL_STRIDE=100
distx: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=p1.x,p2.x,p3.x,pchi.x VAR=a,b,c,y FUNC=((y-a)^2+(y-b)^2+(y-c)^2)^0.5 PERIODIC=NO

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
ARG=c,distx
SIGMA=0.5,0.5
HEIGHT=0.0
TEMP=300
BIASFACTOR=50.0
PACE=500000000
FILE=HILLS
GRID_MIN=0.0,0.0
GRID_MAX=75.0,35.0
GRID_BIN=375,175
LABEL=metad
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>


bias: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__b_i_a_s.html">REWEIGHT_BIAS</a> TEMP=300
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=metad.bias STRIDE=1 FILE=bias RESTART=NO

</pre>{% endraw %}
