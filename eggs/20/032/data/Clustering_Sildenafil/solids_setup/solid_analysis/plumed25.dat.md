**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed25.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed25.dat.plumed.stdout.txt.zip) - [stderr](plumed25.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed25.dat.plumed_master.stdout.txt.zip) - [stderr](plumed25.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1582,1576 AXIS=1576,1597 VECTOR2=1597,1603
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1595,1584 AXIS=1584,1577 VECTOR2=1577,1605
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1584,1577 AXIS=1577,1605 VECTOR2=1605,1617
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1584,1593 AXIS=1593,1587 VECTOR2=1587,1580
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1586,1590 AXIS=1590,1621 VECTOR2=1621,1636
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1590,1621 AXIS=1621,1636 VECTOR2=1636,1632
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_25
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
