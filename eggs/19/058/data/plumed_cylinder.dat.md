**Project ID:** [plumID:19.058]({{ '/' | absolute_url }}eggs/19/058/)  
**Source:** plumed_cylinder.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [raw zipped stdout](plumed_cylinder.dat.plumed.stdout.txt.zip) - [stderr](plumed_cylinder.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_cylinder.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_cylinder.dat.plumed_master.stderr)  

{% raw %}<pre>

<span style="color:blue"># com1 is the COM of one triangular face of the prism, com2 of the other. The orientation is given by the vector from com1 to com2 </span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=3,25,39 LABEL=com1
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=49,69,81 LABEL=com2

<span style="color:blue"># inplane distance between com1 and com2</span>
d1: <a href="https://plumed.github.io/doc-master/user-doc/html/_i_n_p_l_a_n_e_d_i_s_t_a_n_c_e_s.html">INPLANEDISTANCES</a> VECTORSTART=com1 VECTOREND=com2 GROUP=1-162 MIN={BETA=5} 

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_v_i_n_g_r_e_s_t_r_a_i_n_t.html">MOVINGRESTRAINT</a> ...
    ARG=d1.min
    STEP0=0      AT0=0.5  KAPPA0=0.0
    STEP1=20000  AT1=0.5  KAPPA1=50000.0
    LABEL=m1
    VERSE=L
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_v_i_n_g_r_e_s_t_r_a_i_n_t.html">MOVINGRESTRAINT</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=d1.*,m1.* FILE=colvar STRIDE=10
<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=10
</pre>{% endraw %}
