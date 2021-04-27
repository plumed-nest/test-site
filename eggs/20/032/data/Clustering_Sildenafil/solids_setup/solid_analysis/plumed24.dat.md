**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed24.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed24.dat.plumed.stdout.txt.zip) - [stderr](plumed24.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed24.dat.plumed_master.stdout.txt.zip) - [stderr](plumed24.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1519,1513 AXIS=1513,1534 VECTOR2=1534,1540
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1532,1521 AXIS=1521,1514 VECTOR2=1514,1542
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1521,1514 AXIS=1514,1542 VECTOR2=1542,1554
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1521,1530 AXIS=1530,1524 VECTOR2=1524,1517
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1523,1527 AXIS=1527,1558 VECTOR2=1558,1573
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1527,1558 AXIS=1558,1573 VECTOR2=1573,1569
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_24
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
