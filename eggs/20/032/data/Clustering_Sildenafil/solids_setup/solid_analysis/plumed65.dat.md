**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed65.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed65.dat.plumed.stdout.txt.zip) - [stderr](plumed65.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed65.dat.plumed_master.stdout.txt.zip) - [stderr](plumed65.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=4102,4096 AXIS=4096,4117 VECTOR2=4117,4123
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=4115,4104 AXIS=4104,4097 VECTOR2=4097,4125
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=4104,4097 AXIS=4097,4125 VECTOR2=4125,4137
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=4104,4113 AXIS=4113,4107 VECTOR2=4107,4100
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=4106,4110 AXIS=4110,4141 VECTOR2=4141,4156
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=4110,4141 AXIS=4141,4156 VECTOR2=4156,4152
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_65
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
