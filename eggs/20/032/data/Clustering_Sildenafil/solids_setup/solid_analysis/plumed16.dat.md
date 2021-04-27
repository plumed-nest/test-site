**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed16.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed16.dat.plumed.stdout.txt.zip) - [stderr](plumed16.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed16.dat.plumed_master.stdout.txt.zip) - [stderr](plumed16.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1015,1009 AXIS=1009,1030 VECTOR2=1030,1036
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1028,1017 AXIS=1017,1010 VECTOR2=1010,1038
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1017,1010 AXIS=1010,1038 VECTOR2=1038,1050
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1017,1026 AXIS=1026,1020 VECTOR2=1020,1013
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1019,1023 AXIS=1023,1054 VECTOR2=1054,1069
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1023,1054 AXIS=1054,1069 VECTOR2=1069,1065
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_16
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
