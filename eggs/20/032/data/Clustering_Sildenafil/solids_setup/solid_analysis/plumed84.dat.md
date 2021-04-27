**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed84.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed84.dat.plumed.stdout.txt.zip) - [stderr](plumed84.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed84.dat.plumed_master.stdout.txt.zip) - [stderr](plumed84.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5299,5293 AXIS=5293,5314 VECTOR2=5314,5320
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5312,5301 AXIS=5301,5294 VECTOR2=5294,5322
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5301,5294 AXIS=5294,5322 VECTOR2=5322,5334
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5301,5310 AXIS=5310,5304 VECTOR2=5304,5297
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5303,5307 AXIS=5307,5338 VECTOR2=5338,5353
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5307,5338 AXIS=5338,5353 VECTOR2=5353,5349
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_84
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
