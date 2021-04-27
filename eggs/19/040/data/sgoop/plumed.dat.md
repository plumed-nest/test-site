**Project ID:** [plumID:19.040]({{ '/' | absolute_url }}eggs/19/040/)  
**Source:** sgoop/plumed.dat  
**Originally used with PLUMED version:** 2.3  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
phi1: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=5,7,9,15
psi1: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=7,9,15,17
phi2: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=15,17,19,25
psi2: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=17,19,25,27
phi3: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=25,27,29,35
psi3: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=27,29,35,37

cosphi1: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=phi1 FUNC=0.5+cos(x-1.25) PERIODIC=NO
cospsi1: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=psi1 FUNC=0.5+cos(x-1.25) PERIODIC=NO
cosphi2: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=phi2 FUNC=0.5+cos(x-1.25) PERIODIC=NO
cospsi2: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=psi2 FUNC=0.5+cos(x-1.25) PERIODIC=NO
cosphi3: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=phi3 FUNC=0.5+cos(x-1.25) PERIODIC=NO
cospsi3: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=psi3 FUNC=0.5+cos(x-1.25) PERIODIC=NO

meta_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=cosphi1,cospsi1,cosphi2,cospsi2,cosphi3,cospsi3 VAR=c1,c2,c3,c4,c5,c6 FUNC=0.62*c1+0.12*c2+0.57*c3+0.11*c4+0.51*c5+0.04*c6 PERIODIC=NO

metad: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=meta_coord PACE=500 HEIGHT=1.5 SIGMA=0.1 FILE=HILLS BIASFACTOR=10.0 TEMP=300.0

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=500 ARG=phi1,psi1,phi2,psi2,phi3,psi3,meta_coord,metad.bias FILE=COLVAR

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
