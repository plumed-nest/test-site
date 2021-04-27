**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed40.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed40.dat.plumed.stdout.txt.zip) - [stderr](plumed40.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed40.dat.plumed_master.stdout.txt.zip) - [stderr](plumed40.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2527,2521 AXIS=2521,2542 VECTOR2=2542,2548
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2540,2529 AXIS=2529,2522 VECTOR2=2522,2550
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2529,2522 AXIS=2522,2550 VECTOR2=2550,2562
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2529,2538 AXIS=2538,2532 VECTOR2=2532,2525
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2531,2535 AXIS=2535,2566 VECTOR2=2566,2581
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2535,2566 AXIS=2566,2581 VECTOR2=2581,2577
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_40
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
