**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed81.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed81.dat.plumed.stdout.txt.zip) - [stderr](plumed81.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed81.dat.plumed_master.stdout.txt.zip) - [stderr](plumed81.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5110,5104 AXIS=5104,5125 VECTOR2=5125,5131
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5123,5112 AXIS=5112,5105 VECTOR2=5105,5133
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5112,5105 AXIS=5105,5133 VECTOR2=5133,5145
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5112,5121 AXIS=5121,5115 VECTOR2=5115,5108
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5114,5118 AXIS=5118,5149 VECTOR2=5149,5164
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5118,5149 AXIS=5149,5164 VECTOR2=5164,5160
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_81
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
