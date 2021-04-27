**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
**Source:** regtest/pycv/rt-jax1/plumed.dat  
**Originally used with PLUMED version:** 2.5.2-mod  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># LOAD FILE=PythonCV.dylib</span>

cv1: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_y_t_h_o_n_c_v.html">PYTHONCV</a> ATOMS=1,4 IMPORT=jaxcv FUNCTION=cv1

cv1n: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1,4

<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_d_e_r_i_v_a_t_i_v_e_s.html">DUMPDERIVATIVES</a> ARG=cv1  FILE=GRAD_cv1  FMT=%8.4f
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_d_e_r_i_v_a_t_i_v_e_s.html">DUMPDERIVATIVES</a> ARG=cv1n FILE=GRAD_cv1n FMT=%8.4f

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FILE=colvar.out ARG=*



</pre>{% endraw %}
