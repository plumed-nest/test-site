**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed63.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed63.dat.plumed.stdout.txt.zip) - [stderr](plumed63.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed63.dat.plumed_master.stdout.txt.zip) - [stderr](plumed63.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=3976,3970 AXIS=3970,3991 VECTOR2=3991,3997
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=3989,3978 AXIS=3978,3971 VECTOR2=3971,3999
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=3978,3971 AXIS=3971,3999 VECTOR2=3999,4011
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=3978,3987 AXIS=3987,3981 VECTOR2=3981,3974
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=3980,3984 AXIS=3984,4015 VECTOR2=4015,4030
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=3984,4015 AXIS=4015,4030 VECTOR2=4030,4026
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_63
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
