**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed91.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed91.dat.plumed.stdout.txt.zip) - [stderr](plumed91.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed91.dat.plumed_master.stdout.txt.zip) - [stderr](plumed91.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5740,5734 AXIS=5734,5755 VECTOR2=5755,5761
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5753,5742 AXIS=5742,5735 VECTOR2=5735,5763
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5742,5735 AXIS=5735,5763 VECTOR2=5763,5775
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5742,5751 AXIS=5751,5745 VECTOR2=5745,5738
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5744,5748 AXIS=5748,5779 VECTOR2=5779,5794
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5748,5779 AXIS=5779,5794 VECTOR2=5794,5790
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_91
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
