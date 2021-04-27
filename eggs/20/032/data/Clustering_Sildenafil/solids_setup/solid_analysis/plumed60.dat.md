**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed60.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed60.dat.plumed.stdout.txt.zip) - [stderr](plumed60.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed60.dat.plumed_master.stdout.txt.zip) - [stderr](plumed60.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=3787,3781 AXIS=3781,3802 VECTOR2=3802,3808
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=3800,3789 AXIS=3789,3782 VECTOR2=3782,3810
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=3789,3782 AXIS=3782,3810 VECTOR2=3810,3822
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=3789,3798 AXIS=3798,3792 VECTOR2=3792,3785
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=3791,3795 AXIS=3795,3826 VECTOR2=3826,3841
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=3795,3826 AXIS=3826,3841 VECTOR2=3841,3837
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_60
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
