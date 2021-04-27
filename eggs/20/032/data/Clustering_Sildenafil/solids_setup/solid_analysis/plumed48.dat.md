**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed48.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed48.dat.plumed.stdout.txt.zip) - [stderr](plumed48.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed48.dat.plumed_master.stdout.txt.zip) - [stderr](plumed48.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=3031,3025 AXIS=3025,3046 VECTOR2=3046,3052
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=3044,3033 AXIS=3033,3026 VECTOR2=3026,3054
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=3033,3026 AXIS=3026,3054 VECTOR2=3054,3066
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=3033,3042 AXIS=3042,3036 VECTOR2=3036,3029
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=3035,3039 AXIS=3039,3070 VECTOR2=3070,3085
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=3039,3070 AXIS=3070,3085 VECTOR2=3085,3081
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_48
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
