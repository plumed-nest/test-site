**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed73.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed73.dat.plumed.stdout.txt.zip) - [stderr](plumed73.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed73.dat.plumed_master.stdout.txt.zip) - [stderr](plumed73.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=4606,4600 AXIS=4600,4621 VECTOR2=4621,4627
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=4619,4608 AXIS=4608,4601 VECTOR2=4601,4629
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=4608,4601 AXIS=4601,4629 VECTOR2=4629,4641
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=4608,4617 AXIS=4617,4611 VECTOR2=4611,4604
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=4610,4614 AXIS=4614,4645 VECTOR2=4645,4660
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=4614,4645 AXIS=4645,4660 VECTOR2=4660,4656
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_73
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
