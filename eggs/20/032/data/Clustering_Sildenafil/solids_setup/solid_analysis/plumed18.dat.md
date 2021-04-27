**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed18.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed18.dat.plumed.stdout.txt.zip) - [stderr](plumed18.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed18.dat.plumed_master.stdout.txt.zip) - [stderr](plumed18.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1141,1135 AXIS=1135,1156 VECTOR2=1156,1162
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1154,1143 AXIS=1143,1136 VECTOR2=1136,1164
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1143,1136 AXIS=1136,1164 VECTOR2=1164,1176
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1143,1152 AXIS=1152,1146 VECTOR2=1146,1139
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1145,1149 AXIS=1149,1180 VECTOR2=1180,1195
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1149,1180 AXIS=1180,1195 VECTOR2=1195,1191
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_18
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
