**Project ID:** [plumID:19.074]({{ '/' | absolute_url }}eggs/19/074/)  
**Source:** DNA-CCGG/3C5G/plumed.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>
<span style="color:blue"># plumed 2 syntax here, automatically translated from the original input file</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=1-240
d: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=111,112
co: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=235,232 GROUPB=13,10 D_0=0.30 R_0=0.10 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=30 GROUPB=211 D_0=0.55 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=49 GROUPB=189 D_0=0.55 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=68 GROUPB=167 D_0=0.55 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=87 GROUPB=145 D_0=0.55 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=106 GROUPB=123 D_0=0.55 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=30 GROUPB=11 D_0=0.70 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=49 GROUPB=30 D_0=0.70 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=68 GROUPB=49 D_0=0.70 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=87 GROUPB=68 D_0=0.70 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=106 GROUPB=87 D_0=0.70 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=211 GROUPB=233 D_0=0.70 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=189 GROUPB=211 D_0=0.70 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=167 GROUPB=189 D_0=0.70 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=145 GROUPB=167 D_0=0.70 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=123 GROUPB=145 D_0=0.70 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=co AT=2 KAPPA=500 EXP=2 EPS=1
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=d KAPPA=0 AT=1.67 SLOPE=-2.606

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
<span style="color:blue"></span>
<span style="color:blue"><span style="color:blue"># original input file with plumed 1.3 syntax follows</span></span>
<span style="color:blue"></span>
<span style="color:blue">PTMETAD</span>
<span style="color:blue">PRINT W_STRIDE 500</span>
<span style="color:blue">ALIGN_ATOMS LIST <align></span>
<span style="color:blue">align-></span>
<span style="color:blue">LOOP 1 240 1</span>
<span style="color:blue">align<-</span>
<span style="color:blue"></span>
<span style="color:blue"><span style="color:blue">#1</span></span>
<span style="color:blue">DISTANCE LIST 111 112</span>
<span style="color:blue"></span>
<span style="color:blue"><span style="color:blue">#2 </span></span>
<span style="color:blue">COORD LIST <g1> <g2> NN 6 MM 12 D_0 0.30 R_0 0.10 PAIR</span>
<span style="color:blue"></span>
<span style="color:blue">g1-></span>
<span style="color:blue">235 232</span>
<span style="color:blue">g1<-</span>
<span style="color:blue"></span>
<span style="color:blue">g2-></span>
<span style="color:blue">13 10</span>
<span style="color:blue">g2<-</span>
<span style="color:blue"></span>
<span style="color:blue"><span style="color:blue">#3</span></span>
<span style="color:blue">COORD LIST 30 211 NN 6 MM 12 D_0 0.55 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 49 189 NN 6 MM 12 D_0 0.55 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 68 167 NN 6 MM 12 D_0 0.55 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 87 145 NN 6 MM 12 D_0 0.55 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 106 123 NN 6 MM 12 D_0 0.55 R_0 0.00001 PAIR</span>
<span style="color:blue"></span>
<span style="color:blue"><span style="color:blue">#8 3prime strand in this pulling framework</span></span>
<span style="color:blue">COORD LIST 30 11 NN 6 MM 12 D_0 0.70 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 49 30 NN 6 MM 12 D_0 0.70 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 68 49 NN 6 MM 12 D_0 0.70 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 87 68 NN 6 MM 12 D_0 0.70 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 106 87 NN 6 MM 12 D_0 0.70 R_0 0.00001 PAIR</span>
<span style="color:blue"></span>
<span style="color:blue"><span style="color:blue">#13 5prime strand in this pulling framework</span></span>
<span style="color:blue">COORD LIST 211 233 NN 6 MM 12 D_0 0.70 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 189 211 NN 6 MM 12 D_0 0.70 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 167 189 NN 6 MM 12 D_0 0.70 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 145 167 NN 6 MM 12 D_0 0.70 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 123 145 NN 6 MM 12 D_0 0.70 R_0 0.00001 PAIR</span>
<span style="color:blue"></span>
<span style="color:blue">LWALL LIMIT 2 KAPPA 500.0 EXP 2.0 EPS 1.0 OFF 0.0 CV 2</span>
<span style="color:blue">UMBRELLA CV 1 KAPPA 0 AT 1.67 SLOPE -2.606</span>
<span style="color:blue"></span>
<span style="color:blue"></span>
<span style="color:blue"></span>
</pre>{% endraw %}
