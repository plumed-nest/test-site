**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
**Source:** regtest/pycv/rt-jax2/plumed.dat  
**Originally used with PLUMED version:** 2.5.2-mod  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>

cv1:  <a href="https://plumed.github.io/doc-master/user-doc/html/_p_y_t_h_o_n_c_v.html">PYTHONCV</a> ATOMS=1,4,3 IMPORT=jaxcv FUNCTION=cv1
cv1a: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_n_g_l_e.html">ANGLE</a> ATOMS=1,4,3
cv1n: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_y_t_h_o_n_c_v.html">PYTHONCV</a> ATOMS=1,4,3 IMPORT=jaxcv FUNCTION=cv1 NUMERICAL_DERIVATIVES

<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> AT=0 SLOPE=-1 ARG=cv1
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> AT=0 SLOPE=+1 ARG=cv1a

<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_d_e_r_i_v_a_t_i_v_e_s.html">DUMPDERIVATIVES</a> ARG=cv1  FILE=GRAD_cv1  FMT=%8.4f
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_d_e_r_i_v_a_t_i_v_e_s.html">DUMPDERIVATIVES</a> ARG=cv1a FILE=GRAD_cv1a FMT=%8.4f
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_d_e_r_i_v_a_t_i_v_e_s.html">DUMPDERIVATIVES</a> ARG=cv1n FILE=GRAD_cv1n FMT=%8.4f

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FILE=colvar.out ARG=*



</pre>{% endraw %}
