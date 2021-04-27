**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed85.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed85.dat.plumed.stdout.txt.zip) - [stderr](plumed85.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed85.dat.plumed_master.stdout.txt.zip) - [stderr](plumed85.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5362,5356 AXIS=5356,5377 VECTOR2=5377,5383
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5375,5364 AXIS=5364,5357 VECTOR2=5357,5385
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5364,5357 AXIS=5357,5385 VECTOR2=5385,5397
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5364,5373 AXIS=5373,5367 VECTOR2=5367,5360
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5366,5370 AXIS=5370,5401 VECTOR2=5401,5416
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5370,5401 AXIS=5401,5416 VECTOR2=5416,5412
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_85
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
