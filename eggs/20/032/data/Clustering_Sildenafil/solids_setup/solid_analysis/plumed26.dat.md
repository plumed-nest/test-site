**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed26.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed26.dat.plumed.stdout.txt.zip) - [stderr](plumed26.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed26.dat.plumed_master.stdout.txt.zip) - [stderr](plumed26.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1645,1639 AXIS=1639,1660 VECTOR2=1660,1666
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1658,1647 AXIS=1647,1640 VECTOR2=1640,1668
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1647,1640 AXIS=1640,1668 VECTOR2=1668,1680
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1647,1656 AXIS=1656,1650 VECTOR2=1650,1643
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1649,1653 AXIS=1653,1684 VECTOR2=1684,1699
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1653,1684 AXIS=1684,1699 VECTOR2=1699,1695
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_26
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
