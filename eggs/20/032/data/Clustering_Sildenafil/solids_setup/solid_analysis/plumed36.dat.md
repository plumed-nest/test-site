**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed36.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed36.dat.plumed.stdout.txt.zip) - [stderr](plumed36.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed36.dat.plumed_master.stdout.txt.zip) - [stderr](plumed36.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2275,2269 AXIS=2269,2290 VECTOR2=2290,2296
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2288,2277 AXIS=2277,2270 VECTOR2=2270,2298
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2277,2270 AXIS=2270,2298 VECTOR2=2298,2310
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2277,2286 AXIS=2286,2280 VECTOR2=2280,2273
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2279,2283 AXIS=2283,2314 VECTOR2=2314,2329
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2283,2314 AXIS=2314,2329 VECTOR2=2329,2325
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_36
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
