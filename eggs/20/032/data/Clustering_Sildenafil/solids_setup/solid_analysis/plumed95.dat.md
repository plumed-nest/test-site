**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed95.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed95.dat.plumed.stdout.txt.zip) - [stderr](plumed95.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed95.dat.plumed_master.stdout.txt.zip) - [stderr](plumed95.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5992,5986 AXIS=5986,6007 VECTOR2=6007,6013
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=6005,5994 AXIS=5994,5987 VECTOR2=5987,6015
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5994,5987 AXIS=5987,6015 VECTOR2=6015,6027
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5994,6003 AXIS=6003,5997 VECTOR2=5997,5990
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5996,6000 AXIS=6000,6031 VECTOR2=6031,6046
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=6000,6031 AXIS=6031,6046 VECTOR2=6046,6042
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_95
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
