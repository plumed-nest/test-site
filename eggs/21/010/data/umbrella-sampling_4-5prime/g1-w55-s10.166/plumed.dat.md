**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
**Source:** umbrella-sampling_4-5prime/g1-w55-s10.166/plumed.dat  
**Originally used with PLUMED version:** 1.3  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_l_l_s.html">HILLS</a> RESTART HEIGHT 0.000 W_STRIDE 50
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> W_STRIDE 10

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_-_>.html">C-></a>
<a href="https://plumed.github.io/doc-master/user-doc/html/1.html">1</a> 2 
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_<_-.html">C<-</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_o_-_>.html">O-></a>
 <a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_o_p.html">LOOP</a> 3 83 1
<a href="https://plumed.github.io/doc-master/user-doc/html/_o_<_-.html">O<-</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_n_-_>.html">N-></a>
<a href="https://plumed.github.io/doc-master/user-doc/html/84.html">84</a> 85 
<a href="https://plumed.github.io/doc-master/user-doc/html/_n_<_-.html">N<-</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_h_-_>.html">H-></a>
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_o_p.html">LOOP</a> 86 251 1
<a href="https://plumed.github.io/doc-master/user-doc/html/_h_<_-.html">H<-</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_o_o_-_>.html">OO-></a>
<a href="https://plumed.github.io/doc-master/user-doc/html/3.html">3</a> 4 5 6 7 8 9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30 31 32 33 34 35 36 37 38 39 40 41 42 43 44 45 46 47 48 49 50 51 52 53 54 55 57 58 59 60 61 62 63 64 65 66 67 68 69 70 71 72 73 74 75 76 77 78 79 80 81 82 8<a href="https://plumed.github.io/doc-master/user-doc/html/3.html">3</a>
<a href="https://plumed.github.io/doc-master/user-doc/html/_o_o_<_-.html">OO<-</a>


<a href="https://plumed.github.io/doc-master/user-doc/html/_s_p_a_t_h_c_o_o_r_d_t_a_b_l_e.html">SPATHCOORDTABLE</a> NSP 4 LIST <C> <O> <N> <H> NN 8 MM 14 R_0 3.40 3.40 3.40 2.83 3.40 3.40 2.83 3.40 2.83 2.65 LAMBDA 6.76214 
                                   
<a href="https://plumed.github.io/doc-master/user-doc/html/_z_p_a_t_h_c_o_o_r_d_t_a_b_l_e.html">ZPATHCOORDTABLE</a> NSP 4 LIST <C> <O> <N> <H> NN 8 MM 14 R_0 3.40 3.40 3.40 2.83 3.40 3.40 2.83 3.40 2.83 2.65 LAMBDA 6.76214 

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d.html">COORD</a> LIST 1 2 NN 8 MM 14 R_0 3.40
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d.html">COORD</a> LIST 1 <O> NN 8 MM 14 R_0 3.40
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d.html">COORD</a> LIST 1 <N> NN 8 MM 14 R_0 3.40
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d.html">COORD</a> LIST 1 <H> NN 8 MM 14 R_0 2.83
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d.html">COORD</a> LIST 2 1 NN 8 MM 14 R_0 3.40
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d.html">COORD</a> LIST 2 <O> NN 8 MM 14 R_0 3.40
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d.html">COORD</a> LIST 2 <N> NN 8 MM 14 R_0 3.40
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d.html">COORD</a> LIST 2 <H> NN 8 MM 14 R_0 2.83
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d.html">COORD</a> LIST 84 <C> NN 8 MM 14 R_0 3.40
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d.html">COORD</a> LIST 84 <O> NN 8 MM 14 R_0 3.40
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d.html">COORD</a> LIST 84 85 NN 8 MM 14 R_0 3.40
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d.html">COORD</a> LIST 84 <H> NN 8 MM 14 R_0 2.83
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d.html">COORD</a> LIST 85 <C> NN 8 MM 14 R_0 3.40
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d.html">COORD</a> LIST 85 <O> NN 8 MM 14 R_0 3.40
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d.html">COORD</a> LIST 85 84 NN 8 MM 14 R_0 3.40
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d.html">COORD</a> LIST 85 <H> NN 8 MM 14 R_0 2.83

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d.html">COORD</a> LIST 56 <C> NN 8 MM 14 R_0 3.40
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d.html">COORD</a> LIST 56 <OO> NN 8 MM 14 R_0 3.40
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d.html">COORD</a> LIST 56 <N> NN 8 MM 14 R_0 3.40
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d.html">COORD</a> LIST 56 <H> NN 8 MM 14 R_0 2.83

<span style="color:blue">#SEDANCHOR</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_w_a_l_l.html">LWALL</a>  CV 1  LIMIT   10.166  KAPPA    0.129  EXP 2
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_w_a_l_l.html">UWALL</a>  CV 1  LIMIT   10.166  KAPPA    0.129  EXP 2

<a href="https://plumed.github.io/doc-master/user-doc/html/_l_w_a_l_l.html">LWALL</a>  CV 2  LIMIT  -10.  KAPPA  100    EXP 2
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_w_a_l_l.html">UWALL</a>  CV 2  LIMIT    0.28 KAPPA 100     EXP 2
 
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_m_e_t_a.html">ENDMETA</a>
</pre>{% endraw %}
