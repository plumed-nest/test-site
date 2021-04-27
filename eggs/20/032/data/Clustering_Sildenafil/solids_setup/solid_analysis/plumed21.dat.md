**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed21.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed21.dat.plumed.stdout.txt.zip) - [stderr](plumed21.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed21.dat.plumed_master.stdout.txt.zip) - [stderr](plumed21.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1330,1324 AXIS=1324,1345 VECTOR2=1345,1351
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1343,1332 AXIS=1332,1325 VECTOR2=1325,1353
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1332,1325 AXIS=1325,1353 VECTOR2=1353,1365
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1332,1341 AXIS=1341,1335 VECTOR2=1335,1328
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1334,1338 AXIS=1338,1369 VECTOR2=1369,1384
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1338,1369 AXIS=1369,1384 VECTOR2=1384,1380
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_21
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
