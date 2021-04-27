**Project ID:** [plumID:19.047]({{ '/' | absolute_url }}eggs/19/047/)  
**Source:** trpcage/close/plumed.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=1-304
p1: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_o_p_e_r_t_y_m_a_p.html">PROPERTYMAP</a> REFERENCE=reframe.pdb PROPERTY=X,Y LAMBDA=50.0 NEIGH_SIZE=50 NEIGH_STRIDE=50 EPSILON=0.01
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=p1.X,p1.Y SIGMA=0.1,0.1 HEIGHT=0.5 PACE=1000 BIASFACTOR=15 TEMP=300 LABEL=restraint
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=p1.X,p1.Y,p1.zzz,restraint.bias STRIDE=1 FILE=COLVAR FMT=%8.4f
</pre>{% endraw %}
