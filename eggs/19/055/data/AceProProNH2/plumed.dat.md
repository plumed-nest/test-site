**Project ID:** [plumID:19.055]({{ '/' | absolute_url }}eggs/19/055/)  
**Source:** AceProProNH2/plumed.dat  
**Originally used with PLUMED version:** 2.5.0  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> LABEL=angle1 ATOMS=1,5,7,17
<a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> LABEL=angle2 ATOMS=17,19,21,31
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> LABEL=sc1 ARG=angle1 VAR=a1 FUNC=cos(a1/2.0) PERIODIC=NO
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> LABEL=sc2 ARG=angle2 VAR=a2 FUNC=cos(a2/2.0) PERIODIC=NO
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a>  LABEL=sc  ARG=sc1,sc2 POWERS=2,2 PERIODIC=NO
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=sc SIGMA=0.1 HEIGHT=4 PACE=1 WALKERS_MPI FLYING_GAUSSIAN FILE=HILLS LABEL=restraint
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=sc,restraint.bias STRIDE=100 FILE=COLVAR

</pre>{% endraw %}
