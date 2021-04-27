**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed30.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed30.dat.plumed.stdout.txt.zip) - [stderr](plumed30.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed30.dat.plumed_master.stdout.txt.zip) - [stderr](plumed30.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1897,1891 AXIS=1891,1912 VECTOR2=1912,1918
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1910,1899 AXIS=1899,1892 VECTOR2=1892,1920
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1899,1892 AXIS=1892,1920 VECTOR2=1920,1932
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1899,1908 AXIS=1908,1902 VECTOR2=1902,1895
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1901,1905 AXIS=1905,1936 VECTOR2=1936,1951
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1905,1936 AXIS=1936,1951 VECTOR2=1951,1947
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_30
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
