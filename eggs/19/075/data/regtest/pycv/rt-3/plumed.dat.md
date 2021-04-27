**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
**Source:** regtest/pycv/rt-3/plumed.dat  
**Originally used with PLUMED version:** 2.5.2-mod  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>

cv1:  <a href="https://plumed.github.io/doc-master/user-doc/html/_p_y_t_h_o_n_c_v.html">PYTHONCV</a> ATOMS=1,4 IMPORT=distcv FUNCTION=cv
cv2:  <a href="https://plumed.github.io/doc-master/user-doc/html/_p_y_t_h_o_n_c_v.html">PYTHONCV</a> ATOMS=1,3 IMPORT=distcv FUNCTION=cv

cv1a: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1,4
cv2a: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1,3


<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FILE=colvar.out ARG=*



</pre>{% endraw %}
