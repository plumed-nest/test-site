**Project ID:** [plumID:19.059]({{ '/' | absolute_url }}eggs/19/059/)  
**Source:** plumed_be-common.dat  
**Originally used with PLUMED version:** 2.2.3  
**Stable:** [raw zipped stdout](plumed_be-common.dat.plumed.stdout.txt.zip) - [stderr](plumed_be-common.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_be-common.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_be-common.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>
<span style="color:blue"># randomize the exchange (not between consecutive indeces, here just 2 replicas, so it is not relevant)</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_a_n_d_o_m__e_x_c_h_a_n_g_e_s.html">RANDOM_EXCHANGES</a>
<span style="color:blue"># set up the two torsion collective variables </span>
<span style="color:blue"># omega (use cv1 so it will be compatible with the METAGUI analysis plugin)</span>
cv1: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=19,40,42,45
<span style="color:blue"># psi (use cv2 so it will be compatible with the METAGUI analysis plugin)</span>
cv2: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=41,45,53,55

</pre>{% endraw %}
