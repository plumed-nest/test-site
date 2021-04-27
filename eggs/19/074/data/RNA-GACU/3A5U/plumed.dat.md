**Project ID:** [plumID:19.074]({{ '/' | absolute_url }}eggs/19/074/)  
**Source:** RNA-GACU/3A5U/plumed.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>
<span style="color:blue"># plumed 2 syntax here, automatically translated from the original input file</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=1-249
d: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=132,133
co: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=12,11 GROUPB=243,242 D_0=0.30 R_0=0.10 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=35 GROUPB=223 D_0=0.55 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=57 GROUPB=203 D_0=0.55 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=80 GROUPB=183 D_0=0.55 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=102 GROUPB=163 D_0=0.55 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=125 GROUPB=143 D_0=0.55 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=35 GROUPB=12 D_0=0.75 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=57 GROUPB=35 D_0=0.75 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=80 GROUPB=57 D_0=0.75 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=102 GROUPB=80 D_0=0.75 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=125 GROUPB=102 D_0=0.75 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=223 GROUPB=243 D_0=0.75 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=203 GROUPB=223 D_0=0.75 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=183 GROUPB=203 D_0=0.75 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=163 GROUPB=183 D_0=0.75 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=143 GROUPB=163 D_0=0.75 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=co AT=2 KAPPA=500 EXP=2 EPS=1
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=d KAPPA=0 AT=1.67 SLOPE=-2.57833

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
<span style="color:blue"></span>
<span style="color:blue"><span style="color:blue"># original input file with plumed 1.3 syntax follows</span></span>
<span style="color:blue"></span>
<span style="color:blue">PTMETAD</span>
<span style="color:blue">PRINT W_STRIDE 500</span>
<span style="color:blue">ALIGN_ATOMS LIST <align></span>
<span style="color:blue">align-></span>
<span style="color:blue">LOOP 1 249 1</span>
<span style="color:blue">align<-</span>
<span style="color:blue"></span>
<span style="color:blue"><span style="color:blue">#1</span></span>
<span style="color:blue">DISTANCE LIST 132 133</span>
<span style="color:blue"></span>
<span style="color:blue"><span style="color:blue">#2 </span></span>
<span style="color:blue">COORD LIST <g1> <g2> NN 6 MM 12 D_0 0.30 R_0 0.10 PAIR</span>
<span style="color:blue"></span>
<span style="color:blue">g1-></span>
<span style="color:blue">12 11</span>
<span style="color:blue">g1<-</span>
<span style="color:blue"></span>
<span style="color:blue">g2-></span>
<span style="color:blue">243 242</span>
<span style="color:blue">g2<-</span>
<span style="color:blue"></span>
<span style="color:blue"><span style="color:blue">#3</span></span>
<span style="color:blue">COORD LIST 35 223 NN 6 MM 12 D_0 0.55 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 57 203 NN 6 MM 12 D_0 0.55 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 80 183 NN 6 MM 12 D_0 0.55 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 102 163 NN 6 MM 12 D_0 0.55 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 125 143 NN 6 MM 12 D_0 0.55 R_0 0.00001 PAIR</span>
<span style="color:blue"></span>
<span style="color:blue"><span style="color:blue">#8 3prime strand in this pulling framework</span></span>
<span style="color:blue">COORD LIST 35 12 NN 6 MM 12 D_0 0.75 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 57 35 NN 6 MM 12 D_0 0.75 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 80 57 NN 6 MM 12 D_0 0.75 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 102 80 NN 6 MM 12 D_0 0.75 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 125 102 NN 6 MM 12 D_0 0.75 R_0 0.00001 PAIR</span>
<span style="color:blue"></span>
<span style="color:blue"><span style="color:blue">#13 5prime strand in this pulling framework</span></span>
<span style="color:blue">COORD LIST 223 243 NN 6 MM 12 D_0 0.75 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 203 223 NN 6 MM 12 D_0 0.75 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 183 203 NN 6 MM 12 D_0 0.75 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 163 183 NN 6 MM 12 D_0 0.75 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 143 163 NN 6 MM 12 D_0 0.75 R_0 0.00001 PAIR</span>
<span style="color:blue"></span>
<span style="color:blue">LWALL LIMIT 2 KAPPA 500.0 EXP 2.0 EPS 1.0 OFF 0.0 CV 2</span>
<span style="color:blue">UMBRELLA CV 1 KAPPA 0 AT 1.67 SLOPE -2.57833</span>
<span style="color:blue"></span>
<span style="color:blue"></span>
<span style="color:blue"></span>
</pre>{% endraw %}
