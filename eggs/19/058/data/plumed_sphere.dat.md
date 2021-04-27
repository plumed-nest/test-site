**Project ID:** [plumID:19.058]({{ '/' | absolute_url }}eggs/19/058/)  
**Source:** plumed_sphere.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [raw zipped stdout](plumed_sphere.dat.plumed.stdout.txt.zip) - [stderr](plumed_sphere.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_sphere.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_sphere.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>

<span style="color:blue"># This should be the COM of whole molecule</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=1-216 LABEL=com

<span style="color:blue"># The difference between the largest and smallest distance</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=com GROUPB=1-216 MIN={BETA=10} MAX={BETA=.001} LABEL=d1

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
