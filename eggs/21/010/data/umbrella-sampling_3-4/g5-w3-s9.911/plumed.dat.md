**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
**Source:** umbrella-sampling_3-4/g5-w3-s9.911/plumed.dat  
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

<a href="https://plumed.github.io/doc-master/user-doc/html/_s_p_a_t_h_c_o_o_r_d_t_a_b_l_e.html">SPATHCOORDTABLE</a> NSP 4 LIST <C> <O> <N> <H> NN 8 MM 14 R_0 3.40 3.40 3.40 2.83 3.40 3.40 2.83 3.40 2.83 2.65 LAMBDA 19.8011 
                                   
<a href="https://plumed.github.io/doc-master/user-doc/html/_z_p_a_t_h_c_o_o_r_d_t_a_b_l_e.html">ZPATHCOORDTABLE</a> NSP 4 LIST <C> <O> <N> <H> NN 8 MM 14 R_0 3.40 3.40 3.40 2.83 3.40 3.40 2.83 3.40 2.83 2.65 LAMBDA 19.8011 

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


<span style="color:blue"># dist C-C</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> LIST 1 2
<span style="color:blue"># # dist N-N</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> LIST 84 85
<span style="color:blue"># # dist C-N</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> LIST 2 84
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> LIST 2 85
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> LIST 1 84
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> LIST 1 85
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_w_a_l_l.html">LWALL</a>  CV 1  LIMIT    9.911  KAPPA    0.094  EXP 2
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_w_a_l_l.html">UWALL</a>  CV 1  LIMIT    9.911  KAPPA    0.094  EXP 2

<a href="https://plumed.github.io/doc-master/user-doc/html/_l_w_a_l_l.html">LWALL</a>  CV 2  LIMIT  -10.  KAPPA  50     EXP 2
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_w_a_l_l.html">UWALL</a>  CV 2  LIMIT    2 KAPPA  50     EXP 2
 
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_m_e_t_a.html">ENDMETA</a>
</pre>{% endraw %}
