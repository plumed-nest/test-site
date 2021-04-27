**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
**Source:** regtest/pycv/rt-f1/plumed.dat  
**Originally used with PLUMED version:** 2.5.2-mod  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># LOAD FILE=PythonCV.dylib</span>

dAB: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1,4

dAB2: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_y_t_h_o_n_f_u_n_c_t_i_o_n.html">PYTHONFUNCTION</a> ARG=dAB IMPORT=pythonfunction FUNCTION=square PERIODIC=NO

dAB2n: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=dAB POWERS=2.0 PERIODIC=NO

<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_d_e_r_i_v_a_t_i_v_e_s.html">DUMPDERIVATIVES</a> ARG=dAB2  FILE=dAB2_grad    FMT=%.5f
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_d_e_r_i_v_a_t_i_v_e_s.html">DUMPDERIVATIVES</a> ARG=dAB2n FILE=dAB2n_grad   FMT=%.5f

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FILE=colvar.out ARG=*



</pre>{% endraw %}
