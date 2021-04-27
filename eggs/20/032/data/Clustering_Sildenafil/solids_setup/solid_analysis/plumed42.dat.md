**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed42.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed42.dat.plumed.stdout.txt.zip) - [stderr](plumed42.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed42.dat.plumed_master.stdout.txt.zip) - [stderr](plumed42.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2653,2647 AXIS=2647,2668 VECTOR2=2668,2674
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2666,2655 AXIS=2655,2648 VECTOR2=2648,2676
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2655,2648 AXIS=2648,2676 VECTOR2=2676,2688
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2655,2664 AXIS=2664,2658 VECTOR2=2658,2651
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2657,2661 AXIS=2661,2692 VECTOR2=2692,2707
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=2661,2692 AXIS=2692,2707 VECTOR2=2707,2703
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_42
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
