**Project ID:** [plumID:19.047]({{ '/' | absolute_url }}eggs/19/047/)  
**Source:** cyclo/normal/plumed_v2.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [raw zipped stdout](plumed_v2.dat.plumed.stdout.txt.zip) - [stderr](plumed_v2.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_v2.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_v2.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=1-24
p1: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_o_p_e_r_t_y_m_a_p.html">PROPERTYMAP</a> REFERENCE=reference.pdb PROPERTY=S1,S2,S3 LAMBDA=300.0
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=p1.S1,p1.S2,p1.S3 SIGMA=0.02,0.02,0.02 HEIGHT=0.2 PACE=1000 LABEL=restraint
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=p1.S1,p1.S2,p1.S3,p1.zzz,restraint.bias STRIDE=100 FILE=COLVAR FMT=%8.4f
</pre>{% endraw %}
