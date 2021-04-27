**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed93.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed93.dat.plumed.stdout.txt.zip) - [stderr](plumed93.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed93.dat.plumed_master.stdout.txt.zip) - [stderr](plumed93.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5866,5860 AXIS=5860,5881 VECTOR2=5881,5887
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5879,5868 AXIS=5868,5861 VECTOR2=5861,5889
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5868,5861 AXIS=5861,5889 VECTOR2=5889,5901
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5868,5877 AXIS=5877,5871 VECTOR2=5871,5864
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5870,5874 AXIS=5874,5905 VECTOR2=5905,5920
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5874,5905 AXIS=5905,5920 VECTOR2=5920,5916
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_93
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
