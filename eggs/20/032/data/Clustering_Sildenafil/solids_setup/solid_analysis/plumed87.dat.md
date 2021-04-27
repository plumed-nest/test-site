**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed87.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed87.dat.plumed.stdout.txt.zip) - [stderr](plumed87.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed87.dat.plumed_master.stdout.txt.zip) - [stderr](plumed87.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5488,5482 AXIS=5482,5503 VECTOR2=5503,5509
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5501,5490 AXIS=5490,5483 VECTOR2=5483,5511
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5490,5483 AXIS=5483,5511 VECTOR2=5511,5523
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5490,5499 AXIS=5499,5493 VECTOR2=5493,5486
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5492,5496 AXIS=5496,5527 VECTOR2=5527,5542
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5496,5527 AXIS=5527,5542 VECTOR2=5542,5538
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_87
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
