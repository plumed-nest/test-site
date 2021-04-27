**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed19.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed19.dat.plumed.stdout.txt.zip) - [stderr](plumed19.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed19.dat.plumed_master.stdout.txt.zip) - [stderr](plumed19.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1204,1198 AXIS=1198,1219 VECTOR2=1219,1225
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1217,1206 AXIS=1206,1199 VECTOR2=1199,1227
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1206,1199 AXIS=1199,1227 VECTOR2=1227,1239
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1206,1215 AXIS=1215,1209 VECTOR2=1209,1202
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1208,1212 AXIS=1212,1243 VECTOR2=1243,1258
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1212,1243 AXIS=1243,1258 VECTOR2=1258,1254
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_19
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
