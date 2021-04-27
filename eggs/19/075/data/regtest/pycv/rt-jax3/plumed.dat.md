**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
**Source:** regtest/pycv/rt-jax3/plumed.dat  
**Originally used with PLUMED version:** 2.5.2-mod  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>

r:  <a href="https://plumed.github.io/doc-master/user-doc/html/_p_y_t_h_o_n_c_v.html">PYTHONCV</a> ATOMS=1,2,3 IMPORT=curvature FUNCTION=r
ir: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_y_t_h_o_n_f_u_n_c_t_i_o_n.html">PYTHONFUNCTION</a> ARG=r IMPORT=curvature FUNCTION=inv  PERIODIC=NO


<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_d_e_r_i_v_a_t_i_v_e_s.html">DUMPDERIVATIVES</a> ARG=r  FILE=GRADIENT_r  FMT=%8.4f
<span style="color:blue"># DUMPDERIVATIVES ARG=ir FILE=GRADIENT_ir FMT=%8.4f</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FILE=COLVAR ARG=* FMT=%8.4f



</pre>{% endraw %}
