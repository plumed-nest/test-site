**Project ID:** [plumID:19.074]({{ '/' | absolute_url }}eggs/19/074/)  
**Source:** RNA-CGGC/plumed.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>
<span style="color:blue"># plumed 2 syntax here, automatically translated from the original input file</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=1-252
d: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=126,127
co: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=246,243 GROUPB=13,10 D_0=0.30 R_0=0.10 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=32 GROUPB=223 D_0=0.55 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=54 GROUPB=201 D_0=0.55 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=75 GROUPB=180 D_0=0.55 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=97 GROUPB=158 D_0=0.55 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=118 GROUPB=137 D_0=0.55 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=11 GROUPB=32 D_0=0.90 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=32 GROUPB=54 D_0=0.80 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=54 GROUPB=75 D_0=0.90 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=75 GROUPB=97 D_0=0.80 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=97 GROUPB=118 D_0=0.90 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=244 GROUPB=223 D_0=0.90 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=223 GROUPB=201 D_0=0.80 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=201 GROUPB=180 D_0=0.90 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=180 GROUPB=158 D_0=0.80 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=158 GROUPB=137 D_0=0.90 R_0=0.00001 PAIR
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=co AT=2 KAPPA=500 EXP=2 EPS=1
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=d KAPPA=0 AT=1.67 SLOPE=-2.91833

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
<span style="color:blue"></span>
<span style="color:blue"><span style="color:blue"># original input file with plumed 1.3 syntax follows</span></span>
<span style="color:blue"></span>
<span style="color:blue">PTMETAD</span>
<span style="color:blue">PRINT W_STRIDE 500</span>
<span style="color:blue">ALIGN_ATOMS LIST <align></span>
<span style="color:blue">align-></span>
<span style="color:blue">LOOP 1 252 1</span>
<span style="color:blue">align<-</span>
<span style="color:blue"></span>
<span style="color:blue"><span style="color:blue">#1</span></span>
<span style="color:blue">DISTANCE LIST 126 127</span>
<span style="color:blue"></span>
<span style="color:blue"><span style="color:blue">#2</span></span>
<span style="color:blue">COORD LIST <g1> <g2> NN 6 MM 12 D_0 0.30 R_0 0.10 PAIR</span>
<span style="color:blue"></span>
<span style="color:blue">g1-></span>
<span style="color:blue">246 243</span>
<span style="color:blue">g1<-</span>
<span style="color:blue"></span>
<span style="color:blue">g2-></span>
<span style="color:blue">13 10</span>
<span style="color:blue">g2<-</span>
<span style="color:blue"></span>
<span style="color:blue"><span style="color:blue">#3</span></span>
<span style="color:blue">COORD LIST 32 223 NN 6 MM 12 D_0 0.55 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 54 201 NN 6 MM 12 D_0 0.55 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 75 180 NN 6 MM 12 D_0 0.55 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 97 158 NN 6 MM 12 D_0 0.55 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 118 137 NN 6 MM 12 D_0 0.55 R_0 0.00001 PAIR</span>
<span style="color:blue"></span>
<span style="color:blue"><span style="color:blue">#8 3prime</span></span>
<span style="color:blue">COORD LIST 11 32 NN 6 MM 12 D_0 0.90 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 32 54 NN 6 MM 12 D_0 0.80 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 54 75 NN 6 MM 12 D_0 0.90 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 75 97 NN 6 MM 12 D_0 0.80 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 97 118 NN 6 MM 12 D_0 0.90 R_0 0.00001 PAIR</span>
<span style="color:blue"></span>
<span style="color:blue"><span style="color:blue">#13 5prime</span></span>
<span style="color:blue">COORD LIST 244 223 NN 6 MM 12 D_0 0.90 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 223 201 NN 6 MM 12 D_0 0.80 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 201 180 NN 6 MM 12 D_0 0.90 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 180 158 NN 6 MM 12 D_0 0.80 R_0 0.00001 PAIR</span>
<span style="color:blue">COORD LIST 158 137 NN 6 MM 12 D_0 0.90 R_0 0.00001 PAIR</span>
<span style="color:blue"></span>
<span style="color:blue">LWALL LIMIT 2 KAPPA 500.0 EXP 2.0 EPS 1.0 OFF 0.0 CV 2</span>
<span style="color:blue">UMBRELLA CV 1 KAPPA 0 AT 1.67 SLOPE -2.91833</span>
<span style="color:blue"></span>
<span style="color:blue"></span>
</pre>{% endraw %}
