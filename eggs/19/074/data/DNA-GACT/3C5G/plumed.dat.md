**Project ID:** [plumID:19.074]({{ '/' | absolute_url }}eggs/19/074/)  
**Source:** DNA-GACT/3C5G/plumed.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>
<span style="color:blue"># plumed 2 syntax here, automatically translated from the original input file</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=1-240
d: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1,240
co: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=120,119 GROUPB=138,137 D_0=0.30 R_0=0.10 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=98 GROUPB=157 D_0=0.55 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=77 GROUPB=177 D_0=0.55 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=55 GROUPB=196 D_0=0.55 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=34 GROUPB=216 D_0=0.55 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=12 GROUPB=235 D_0=0.55 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=138 GROUPB=157 D_0=0.70 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=157 GROUPB=177 D_0=0.70 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=177 GROUPB=196 D_0=0.70 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=196 GROUPB=216 D_0=0.70 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=216 GROUPB=235 D_0=0.70 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=120 GROUPB=98 D_0=0.70 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=98 GROUPB=77 D_0=0.70 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=77 GROUPB=55 D_0=0.70 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=55 GROUPB=34 D_0=0.70 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=34 GROUPB=12 D_0=0.70 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=co AT=2 KAPPA=500 EXP=2 EPS=1
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=d KAPPA=0 AT=1.67 SLOPE=-2.55

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
<span style="color:blue">DISTANCE LIST 1 240</span>
<span style="color:blue"></span>
<span style="color:blue"><span style="color:blue">#2 </span></span>
<span style="color:blue">COORD LIST <g1> <g2> NN 6 MM 12 D_0 0.30 R_0 0.10 PAIR</span>
<span style="color:blue"></span>
<span style="color:blue">g1-></span>
<span style="color:blue">120 119</span>
<span style="color:blue">g1<-</span>
<span style="color:blue"></span>
<span style="color:blue">g2-></span>
<span style="color:blue">138 137 </span>
<span style="color:blue">g2<-</span>
<span style="color:blue"></span>
<span style="color:blue"><span style="color:blue">#3</span></span>
<span style="color:blue">COORD LIST 98 157 NN 6 MM 12 D_0 0.55 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 77 177 NN 6 MM 12 D_0 0.55 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 55 196 NN 6 MM 12 D_0 0.55 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 34 216 NN 6 MM 12 D_0 0.55 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 12 235 NN 6 MM 12 D_0 0.55 R_0 0.00001 PAIR</span>
<span style="color:blue"></span>
<span style="color:blue"></span>
<span style="color:blue"><span style="color:blue">#8 3prime strand in this pulling framework</span></span>
<span style="color:blue">COORD LIST 138 157 NN 6 MM 12 D_0 0.70 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 157 177 NN 6 MM 12 D_0 0.70 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 177 196 NN 6 MM 12 D_0 0.70 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 196 216 NN 6 MM 12 D_0 0.70 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 216 235 NN 6 MM 12 D_0 0.70 R_0 0.00001 PAIR</span>
<span style="color:blue"></span>
<span style="color:blue"><span style="color:blue">#13 5prime strand in this pulling framework</span></span>
<span style="color:blue">COORD LIST 120 98 NN 6 MM 12 D_0 0.70 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 98 77 NN 6 MM 12 D_0 0.70 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 77 55 NN 6 MM 12 D_0 0.70 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 55 34 NN 6 MM 12 D_0 0.70 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 34 12 NN 6 MM 12 D_0 0.70 R_0 0.00001 PAIR</span>
<span style="color:blue"></span>
<span style="color:blue">LWALL LIMIT 2 KAPPA 500.0 EXP 2.0 EPS 1.0 OFF 0.0 CV 2</span>
<span style="color:blue">UMBRELLA CV 1 KAPPA 0 AT 1.67 SLOPE -2.55</span>
<span style="color:blue"></span>
<span style="color:blue"></span>
<span style="color:blue"></span>
</pre>{% endraw %}
