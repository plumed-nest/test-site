**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed33.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed33.dat.plumed.stdout.txt.zip) - [stderr](plumed33.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed33.dat.plumed_master.stdout.txt.zip) - [stderr](plumed33.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2086,2080 AXIS=2080,2101 VECTOR2=2101,2107
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2099,2088 AXIS=2088,2081 VECTOR2=2081,2109
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2088,2081 AXIS=2081,2109 VECTOR2=2109,2121
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2088,2097 AXIS=2097,2091 VECTOR2=2091,2084
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2090,2094 AXIS=2094,2125 VECTOR2=2125,2140
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2094,2125 AXIS=2125,2140 VECTOR2=2140,2136
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_33
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
