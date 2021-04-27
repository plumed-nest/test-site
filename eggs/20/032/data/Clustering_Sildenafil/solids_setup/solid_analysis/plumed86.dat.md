**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed86.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed86.dat.plumed.stdout.txt.zip) - [stderr](plumed86.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed86.dat.plumed_master.stdout.txt.zip) - [stderr](plumed86.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5425,5419 AXIS=5419,5440 VECTOR2=5440,5446
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5438,5427 AXIS=5427,5420 VECTOR2=5420,5448
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5427,5420 AXIS=5420,5448 VECTOR2=5448,5460
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5427,5436 AXIS=5436,5430 VECTOR2=5430,5423
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5429,5433 AXIS=5433,5464 VECTOR2=5464,5479
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5433,5464 AXIS=5464,5479 VECTOR2=5479,5475
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_86
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
