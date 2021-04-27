**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed90.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed90.dat.plumed.stdout.txt.zip) - [stderr](plumed90.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed90.dat.plumed_master.stdout.txt.zip) - [stderr](plumed90.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5677,5671 AXIS=5671,5692 VECTOR2=5692,5698
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5690,5679 AXIS=5679,5672 VECTOR2=5672,5700
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5679,5672 AXIS=5672,5700 VECTOR2=5700,5712
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5679,5688 AXIS=5688,5682 VECTOR2=5682,5675
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5681,5685 AXIS=5685,5716 VECTOR2=5716,5731
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5685,5716 AXIS=5716,5731 VECTOR2=5731,5727
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_90
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
