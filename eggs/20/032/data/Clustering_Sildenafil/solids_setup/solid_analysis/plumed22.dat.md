**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed22.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed22.dat.plumed.stdout.txt.zip) - [stderr](plumed22.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed22.dat.plumed_master.stdout.txt.zip) - [stderr](plumed22.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1393,1387 AXIS=1387,1408 VECTOR2=1408,1414
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1406,1395 AXIS=1395,1388 VECTOR2=1388,1416
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1395,1388 AXIS=1388,1416 VECTOR2=1416,1428
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1395,1404 AXIS=1404,1398 VECTOR2=1398,1391
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1397,1401 AXIS=1401,1432 VECTOR2=1432,1447
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1401,1432 AXIS=1432,1447 VECTOR2=1447,1443
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_22
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
