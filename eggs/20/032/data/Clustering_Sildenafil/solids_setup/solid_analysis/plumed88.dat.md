**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed88.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed88.dat.plumed.stdout.txt.zip) - [stderr](plumed88.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed88.dat.plumed_master.stdout.txt.zip) - [stderr](plumed88.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5551,5545 AXIS=5545,5566 VECTOR2=5566,5572
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5564,5553 AXIS=5553,5546 VECTOR2=5546,5574
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5553,5546 AXIS=5546,5574 VECTOR2=5574,5586
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5553,5562 AXIS=5562,5556 VECTOR2=5556,5549
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5555,5559 AXIS=5559,5590 VECTOR2=5590,5605
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5559,5590 AXIS=5590,5605 VECTOR2=5605,5601
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_88
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
