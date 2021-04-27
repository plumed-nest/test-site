**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed32.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed32.dat.plumed.stdout.txt.zip) - [stderr](plumed32.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed32.dat.plumed_master.stdout.txt.zip) - [stderr](plumed32.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2023,2017 AXIS=2017,2038 VECTOR2=2038,2044
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2036,2025 AXIS=2025,2018 VECTOR2=2018,2046
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2025,2018 AXIS=2018,2046 VECTOR2=2046,2058
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2025,2034 AXIS=2034,2028 VECTOR2=2028,2021
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2027,2031 AXIS=2031,2062 VECTOR2=2062,2077
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2031,2062 AXIS=2062,2077 VECTOR2=2077,2073
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_32
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
