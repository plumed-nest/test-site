**Project ID:** [plumID:19.023]({{ '/' | absolute_url }}eggs/19/023/)  
**Source:** plumed.dat  
**Originally used with PLUMED version:** 2.3  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=1,5,6,7,9,11,15,16,17,19
<span style="color:blue">#variables</span>
phi: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=5,7,9,15
psi: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=7,9,15,17
rg: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_y_r_a_t_i_o_n.html">GYRATION</a> TYPE=RADIUS ATOMS=1,5,6,7,9,11,15,16,17,19
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=phi,psi,rg FILE=COLVAR STRIDE=100
<span style="color:blue">#Well-tempered MetaD lines, one for each CV. For each replica the value of the BIASFACTOR should be changed.</span>
a: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=phi SIGMA=0.3 TAU=12 PACE=500 BIASFACTOR=15 GRID_MIN=-pi GRID_MAX=pi FILE=HILLSphi
b: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=psi SIGMA=0.3 TAU=12 PACE=500 BIASFACTOR=15 GRID_MIN=-pi GRID_MAX=pi FILE=HILLSpsi
c: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=rg SIGMA=0.007 TAU=12 PACE=500 BIASFACTOR=15 GRID_MIN=0 GRID_MAX=0.4 FILE=HILLSrg
</pre>{% endraw %}
