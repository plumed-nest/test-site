**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed70.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed70.dat.plumed.stdout.txt.zip) - [stderr](plumed70.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed70.dat.plumed_master.stdout.txt.zip) - [stderr](plumed70.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=4417,4411 AXIS=4411,4432 VECTOR2=4432,4438
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=4430,4419 AXIS=4419,4412 VECTOR2=4412,4440
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=4419,4412 AXIS=4412,4440 VECTOR2=4440,4452
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=4419,4428 AXIS=4428,4422 VECTOR2=4422,4415
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=4421,4425 AXIS=4425,4456 VECTOR2=4456,4471
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=4425,4456 AXIS=4456,4471 VECTOR2=4471,4467
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_70
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
