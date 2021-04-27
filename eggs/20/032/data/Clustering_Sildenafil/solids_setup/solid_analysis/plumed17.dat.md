**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed17.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed17.dat.plumed.stdout.txt.zip) - [stderr](plumed17.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed17.dat.plumed_master.stdout.txt.zip) - [stderr](plumed17.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1078,1072 AXIS=1072,1093 VECTOR2=1093,1099
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1091,1080 AXIS=1080,1073 VECTOR2=1073,1101
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1080,1073 AXIS=1073,1101 VECTOR2=1101,1113
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1080,1089 AXIS=1089,1083 VECTOR2=1083,1076
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1082,1086 AXIS=1086,1117 VECTOR2=1117,1132
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1086,1117 AXIS=1117,1132 VECTOR2=1132,1128
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_17
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
