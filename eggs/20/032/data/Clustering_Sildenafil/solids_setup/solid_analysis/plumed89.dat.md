**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed89.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed89.dat.plumed.stdout.txt.zip) - [stderr](plumed89.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed89.dat.plumed_master.stdout.txt.zip) - [stderr](plumed89.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5614,5608 AXIS=5608,5629 VECTOR2=5629,5635
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5627,5616 AXIS=5616,5609 VECTOR2=5609,5637
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5616,5609 AXIS=5609,5637 VECTOR2=5637,5649
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5616,5625 AXIS=5625,5619 VECTOR2=5619,5612
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5618,5622 AXIS=5622,5653 VECTOR2=5653,5668
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5622,5653 AXIS=5653,5668 VECTOR2=5668,5664
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_89
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
