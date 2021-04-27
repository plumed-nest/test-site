**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed50.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed50.dat.plumed.stdout.txt.zip) - [stderr](plumed50.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed50.dat.plumed_master.stdout.txt.zip) - [stderr](plumed50.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=3157,3151 AXIS=3151,3172 VECTOR2=3172,3178
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=3170,3159 AXIS=3159,3152 VECTOR2=3152,3180
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=3159,3152 AXIS=3152,3180 VECTOR2=3180,3192
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=3159,3168 AXIS=3168,3162 VECTOR2=3162,3155
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=3161,3165 AXIS=3165,3196 VECTOR2=3196,3211
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=3165,3196 AXIS=3196,3211 VECTOR2=3211,3207
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_50
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
