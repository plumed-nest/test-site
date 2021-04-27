**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed51.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed51.dat.plumed.stdout.txt.zip) - [stderr](plumed51.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed51.dat.plumed_master.stdout.txt.zip) - [stderr](plumed51.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=3220,3214 AXIS=3214,3235 VECTOR2=3235,3241
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=3233,3222 AXIS=3222,3215 VECTOR2=3215,3243
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=3222,3215 AXIS=3215,3243 VECTOR2=3243,3255
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=3222,3231 AXIS=3231,3225 VECTOR2=3225,3218
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=3224,3228 AXIS=3228,3259 VECTOR2=3259,3274
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=3228,3259 AXIS=3259,3274 VECTOR2=3274,3270
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_51
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
