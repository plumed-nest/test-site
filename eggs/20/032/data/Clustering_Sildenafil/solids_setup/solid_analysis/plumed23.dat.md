**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed23.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed23.dat.plumed.stdout.txt.zip) - [stderr](plumed23.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed23.dat.plumed_master.stdout.txt.zip) - [stderr](plumed23.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1456,1450 AXIS=1450,1471 VECTOR2=1471,1477
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1469,1458 AXIS=1458,1451 VECTOR2=1451,1479
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1458,1451 AXIS=1451,1479 VECTOR2=1479,1491
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1458,1467 AXIS=1467,1461 VECTOR2=1461,1454
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1460,1464 AXIS=1464,1495 VECTOR2=1495,1510
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1464,1495 AXIS=1495,1510 VECTOR2=1510,1506
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_23
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
