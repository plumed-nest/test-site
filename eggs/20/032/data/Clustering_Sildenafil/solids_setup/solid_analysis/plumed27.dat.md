**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed27.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed27.dat.plumed.stdout.txt.zip) - [stderr](plumed27.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed27.dat.plumed_master.stdout.txt.zip) - [stderr](plumed27.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1708,1702 AXIS=1702,1723 VECTOR2=1723,1729
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1721,1710 AXIS=1710,1703 VECTOR2=1703,1731
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1710,1703 AXIS=1703,1731 VECTOR2=1731,1743
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1710,1719 AXIS=1719,1713 VECTOR2=1713,1706
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1712,1716 AXIS=1716,1747 VECTOR2=1747,1762
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1716,1747 AXIS=1747,1762 VECTOR2=1762,1758
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_27
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
