**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed37.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed37.dat.plumed.stdout.txt.zip) - [stderr](plumed37.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed37.dat.plumed_master.stdout.txt.zip) - [stderr](plumed37.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2338,2332 AXIS=2332,2353 VECTOR2=2353,2359
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2351,2340 AXIS=2340,2333 VECTOR2=2333,2361
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2340,2333 AXIS=2333,2361 VECTOR2=2361,2373
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2340,2349 AXIS=2349,2343 VECTOR2=2343,2336
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2342,2346 AXIS=2346,2377 VECTOR2=2377,2392
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2346,2377 AXIS=2377,2392 VECTOR2=2392,2388
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_37
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
