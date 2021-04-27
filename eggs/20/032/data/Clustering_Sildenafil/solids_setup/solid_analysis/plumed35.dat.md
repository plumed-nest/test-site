**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed35.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed35.dat.plumed.stdout.txt.zip) - [stderr](plumed35.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed35.dat.plumed_master.stdout.txt.zip) - [stderr](plumed35.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2212,2206 AXIS=2206,2227 VECTOR2=2227,2233
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2225,2214 AXIS=2214,2207 VECTOR2=2207,2235
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2214,2207 AXIS=2207,2235 VECTOR2=2235,2247
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2214,2223 AXIS=2223,2217 VECTOR2=2217,2210
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2216,2220 AXIS=2220,2251 VECTOR2=2251,2266
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2220,2251 AXIS=2251,2266 VECTOR2=2266,2262
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_35
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
