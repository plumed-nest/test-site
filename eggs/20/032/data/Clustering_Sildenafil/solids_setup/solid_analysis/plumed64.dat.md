**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed64.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed64.dat.plumed.stdout.txt.zip) - [stderr](plumed64.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed64.dat.plumed_master.stdout.txt.zip) - [stderr](plumed64.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=4039,4033 AXIS=4033,4054 VECTOR2=4054,4060
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=4052,4041 AXIS=4041,4034 VECTOR2=4034,4062
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=4041,4034 AXIS=4034,4062 VECTOR2=4062,4074
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=4041,4050 AXIS=4050,4044 VECTOR2=4044,4037
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=4043,4047 AXIS=4047,4078 VECTOR2=4078,4093
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=4047,4078 AXIS=4078,4093 VECTOR2=4093,4089
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_64
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
