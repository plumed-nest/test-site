**Project ID:** [plumID:19.040]({{ '/' | absolute_url }}eggs/19/040/)  
**Source:** metad_2d/plumed.dat  
**Originally used with PLUMED version:** 2.3  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>

phi1: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=5,7,9,15
phi2: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=15,17,19,25
phi3: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=25,27,29,35

<span style="color:blue">#cosphi1: MATHEVAL ARG=phi1 FUNC=0.5+cos(x-0.75) PERIODIC=NO</span>
<span style="color:blue">#cosphi2: MATHEVAL ARG=phi2 FUNC=0.5+cos(x-0.75) PERIODIC=NO</span>
<span style="color:blue">#cosphi3: MATHEVAL ARG=phi3 FUNC=0.5+cos(x-0.75) PERIODIC=NO</span>

metad: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=phi1,phi2 PACE=2000 HEIGHT=3 SIGMA=0.1,0.1 FILE=HILLS BIASFACTOR=10.0 TEMP=300.0

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=250 ARG=phi1,phi2,phi3,metad.bias FILE=COLVAR

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
