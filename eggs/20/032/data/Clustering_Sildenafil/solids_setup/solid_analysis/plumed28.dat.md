**Project ID:** [plumID:20.032]({{ '/' | absolute_url }}eggs/20/032/)  
**Source:** Clustering_Sildenafil/solids_setup/solid_analysis/plumed28.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed28.dat.plumed.stdout.txt.zip) - [stderr](plumed28.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed28.dat.plumed_master.stdout.txt.zip) - [stderr](plumed28.dat.plumed_master.stderr)  

{% raw %}<pre>
tA: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1771,1765 AXIS=1765,1786 VECTOR2=1786,1792
tB: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1784,1773 AXIS=1773,1766 VECTOR2=1766,1794
tC: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1773,1766 AXIS=1766,1794 VECTOR2=1794,1806
tD: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1773,1782 AXIS=1782,1776 VECTOR2=1776,1769
tE: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1775,1779 AXIS=1779,1810 VECTOR2=1810,1825
tF: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=1779,1810 AXIS=1810,1825 VECTOR2=1825,1821
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=tA,tB,tC,tD,tE,tF FILE=cluster_data_28
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
