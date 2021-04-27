**Project ID:** [plumID:21.004]({{ '/' | absolute_url }}eggs/21/004/)  
**Source:** GSK/3/plumed_path.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [raw zipped stdout](plumed_path.dat.plumed.stdout.txt.zip) - [stderr](plumed_path.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_path.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_path.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=1-5640 ENTITY1=5641-5700 STRIDE=1

p: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_a_t_h_m_s_d.html">PATHMSD</a> REFERENCE=path.pdb  LAMBDA=230.00 NEIGH_STRIDE=4 NEIGH_SIZE=8

meta: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=p.sss,p.zzz SIGMA=0.2,0.01 HEIGHT=0.84 TEMP=300 BIASFACTOR=15 PACE=500 GRID_MIN=1,-0.015 GRID_MAX=69,0.18
uwall_z: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=p.zzz AT=0.05 KAPPA=400000.0
lwall_s_o: <a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=p.sss AT=1  KAPPA=20000.0
uwall_s_i: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=p.sss AT=70 KAPPA=20000.0

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=p.sss,p.zzz STRIDE=250 FILE=COLV_Path FMT=%8.4f
</pre>{% endraw %}
