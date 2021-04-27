**Project ID:** [plumID:19.030]({{ '/' | absolute_url }}eggs/19/030/)  
**Source:** plumed_2.dat  
**Originally used with PLUMED version:** 2.5.1  
**Stable:** [raw zipped stdout](plumed_2.dat.plumed.stdout.txt.zip) - [stderr](plumed_2.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_2.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_2.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=1-176
helix1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=1-88
helix2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=89-176

dist: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=helix1,helix2

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=dist SIGMA=0.05 HEIGHT=0.05 PACE=5000 TEMP=323 BIASFACTOR=10 GRID_MIN=-0.5 GRID_MAX=7.5 GRID_BIN=400 FILE=HILLS

<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=dist AT=4.5 KAPPA=3000 LABEL=uwall
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=dist AT=0.0 KAPPA=3000 LABEL=lwall

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=* STRIDE=100 FILE=COLVAR
</pre>{% endraw %}
