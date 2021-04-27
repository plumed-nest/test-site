**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
**Source:** regtest/pycv/rt-multi-1/plumed.dat  
**Originally used with PLUMED version:** 2.5.2-mod  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>

cv1:  <a href="https://plumed.github.io/doc-master/user-doc/html/_p_y_t_h_o_n_c_v.html">PYTHONCV</a> ATOMS=1,3,4 IMPORT=distcv FUNCTION=cv COMPONENTS=d12,d13

cv12a: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1,3
cv13a: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1,4

<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_d_e_r_i_v_a_t_i_v_e_s.html">DUMPDERIVATIVES</a> ARG=cv1.py-d12 FILE=GRAD_cv1d12 FMT=%.4f
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_d_e_r_i_v_a_t_i_v_e_s.html">DUMPDERIVATIVES</a> ARG=cv1.py-d13 FILE=GRAD_cv1d13 FMT=%.4f
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_d_e_r_i_v_a_t_i_v_e_s.html">DUMPDERIVATIVES</a> ARG=cv12a FILE=GRAD_cv12a FMT=%.4f
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_d_e_r_i_v_a_t_i_v_e_s.html">DUMPDERIVATIVES</a> ARG=cv13a FILE=GRAD_cv13a FMT=%.4f

<span style="color:blue"># RESTRAINT AT=0 SLOPE=-1 ARG=cv1</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FILE=colvar.out ARG=*



</pre>{% endraw %}
