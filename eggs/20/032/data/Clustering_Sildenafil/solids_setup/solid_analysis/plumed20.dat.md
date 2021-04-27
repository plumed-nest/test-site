**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed20.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed20.dat.plumed.stdout.txt.zip) - [stderr](plumed20.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed20.dat.plumed_master.stdout.txt.zip) - [stderr](plumed20.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1267,1261 AXIS=1261,1282 VECTOR2=1282,1288
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1280,1269 AXIS=1269,1262 VECTOR2=1262,1290
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1269,1262 AXIS=1262,1290 VECTOR2=1290,1302
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1269,1278 AXIS=1278,1272 VECTOR2=1272,1265
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1271,1275 AXIS=1275,1306 VECTOR2=1306,1321
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1275,1306 AXIS=1306,1321 VECTOR2=1321,1317
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_20
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
