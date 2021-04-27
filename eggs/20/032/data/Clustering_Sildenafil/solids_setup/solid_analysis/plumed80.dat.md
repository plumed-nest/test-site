**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed80.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed80.dat.plumed.stdout.txt.zip) - [stderr](plumed80.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed80.dat.plumed_master.stdout.txt.zip) - [stderr](plumed80.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5047,5041 AXIS=5041,5062 VECTOR2=5062,5068
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5060,5049 AXIS=5049,5042 VECTOR2=5042,5070
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5049,5042 AXIS=5042,5070 VECTOR2=5070,5082
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5049,5058 AXIS=5058,5052 VECTOR2=5052,5045
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5051,5055 AXIS=5055,5086 VECTOR2=5086,5101
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5055,5086 AXIS=5086,5101 VECTOR2=5101,5097
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_80
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
