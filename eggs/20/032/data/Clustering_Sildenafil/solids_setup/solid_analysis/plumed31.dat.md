**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed31.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed31.dat.plumed.stdout.txt.zip) - [stderr](plumed31.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed31.dat.plumed_master.stdout.txt.zip) - [stderr](plumed31.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1960,1954 AXIS=1954,1975 VECTOR2=1975,1981
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1973,1962 AXIS=1962,1955 VECTOR2=1955,1983
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1962,1955 AXIS=1955,1983 VECTOR2=1983,1995
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1962,1971 AXIS=1971,1965 VECTOR2=1965,1958
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1964,1968 AXIS=1968,1999 VECTOR2=1999,2014
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1968,1999 AXIS=1999,2014 VECTOR2=2014,2010
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_31
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
