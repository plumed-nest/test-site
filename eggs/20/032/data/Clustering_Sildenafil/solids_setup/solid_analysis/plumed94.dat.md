**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed94.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed94.dat.plumed.stdout.txt.zip) - [stderr](plumed94.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed94.dat.plumed_master.stdout.txt.zip) - [stderr](plumed94.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5929,5923 AXIS=5923,5944 VECTOR2=5944,5950
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5942,5931 AXIS=5931,5924 VECTOR2=5924,5952
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5931,5924 AXIS=5924,5952 VECTOR2=5952,5964
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5931,5940 AXIS=5940,5934 VECTOR2=5934,5927
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5933,5937 AXIS=5937,5968 VECTOR2=5968,5983
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5937,5968 AXIS=5968,5983 VECTOR2=5983,5979
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_94
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
