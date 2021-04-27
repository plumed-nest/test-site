**Project ID:** [plumID:19.021]({{ '/' | absolute_url }}eggs/19/021/)  
**Source:** ./Trajectories/EDS-flattening-atomistic/flatten-trimer-angular-lm-t12/flatten_trimer_3phi_3dist_extraflat_ang_i100ps_lm0.01_p100/factin_3mono_ATP_flatten_ang_3phi_3dist_extraflat_i100ps_lm0.01_p100.run.10000000.plumed.dat  
**Originally used with PLUMED version:** 2.5b  
**Stable:** [raw zipped stdout](factin_3mono_ATP_flatten_ang_3phi_3dist_extraflat_i100ps_lm0.01_p100.run.10000000.plumed.dat.plumed.stdout.txt.zip) - [stderr](factin_3mono_ATP_flatten_ang_3phi_3dist_extraflat_i100ps_lm0.01_p100.run.10000000.plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](factin_3mono_ATP_flatten_ang_3phi_3dist_extraflat_i100ps_lm0.01_p100.run.10000000.plumed.dat.plumed_master.stdout.txt.zip) - [stderr](factin_3mono_ATP_flatten_ang_3phi_3dist_extraflat_i100ps_lm0.01_p100.run.10000000.plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_i_n_c_l_u_d_e.html">INCLUDE</a> FILE=<a href="fatp_3mono_cvs_cacb.txt.html">fatp_3mono_cvs_cacb.txt</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=A1-CA1 LABEL=A1-b1
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=A1-CA2 LABEL=A1-b2
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=A1-CA3 LABEL=A1-b3
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=A1-CA4 LABEL=A1-b4

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=A2-CA1 LABEL=A2-b1
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=A2-CA2 LABEL=A2-b2
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=A2-CA3 LABEL=A2-b3
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=A2-CA4 LABEL=A2-b4

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=A3-CA1 LABEL=A3-b1
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=A3-CA2 LABEL=A3-b2
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=A3-CA3 LABEL=A3-b3
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=A3-CA4 LABEL=A3-b4

<span style="color:blue">#cleft_dist</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=A1-b2,A1-b4 LABEL=cleft_A1
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=A2-b2,A2-b4 LABEL=cleft_A2
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=A3-b2,A3-b4 LABEL=cleft_A3

<a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=A1-b2,A1-b1,A1-b3,A1-b4 LABEL=dihedralm_A1
<a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=A2-b2,A2-b1,A2-b3,A2-b4 LABEL=dihedralm_A2
<a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=A3-b2,A3-b1,A3-b3,A3-b4 LABEL=dihedralm_A3
dihedral_A1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=dihedralm_A1 POWERS=1 COEFFICIENTS=-1 PERIODIC=NO
dihedral_A2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=dihedralm_A2 POWERS=1 COEFFICIENTS=-1 PERIODIC=NO
dihedral_A3: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=dihedralm_A3 POWERS=1 COEFFICIENTS=-1 PERIODIC=NO

<span style="color:blue">#dihedral2_A1: COMBINE ARG=dihedralm_A1 POWERS=2 COEFFICIENTS=1 PERIODIC=NO</span>
<span style="color:blue">#dihedral2_A2: COMBINE ARG=dihedralm_A2 POWERS=2 COEFFICIENTS=1 PERIODIC=NO</span>
<span style="color:blue">#dihedral2_A3: COMBINE ARG=dihedralm_A3 POWERS=2 COEFFICIENTS=1 PERIODIC=NO</span>

<span style="color:blue">#bias mean of 1,2</span>
eds: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_d_s.html">EDS</a> ARG=cleft_A1,cleft_A2,cleft_A3,dihedral_A1,dihedral_A2,dihedral_A3 CENTER=2.06155,2.06155,2.06155,0.110262,0.110262,0.110262 PERIOD=25000 OUT_RESTART=factin_3mono_ATP_flatten_ang_3phi_3dist_extraflat_i100ps_lm0.01_p100.run.10000000.restart.dat  INIT=0.0,0.0,0.0,0.0,0.0,0.0 RANGE=1.0,1.0,1.0,1.0,1.0,1.0 STRIDE=2 COVAR LM LM_MIXING=0.01

<span style="color:blue">#write every 10 ps</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=cleft_A1,dihedral_A1,cleft_A2,dihedral_A2,cleft_A3,dihedral_A3 FILE=factin_3mono_ATP_flatten_ang_3phi_3dist_extraflat_i100ps_lm0.01_p100.run.10000000.colvars.dat STRIDE=5000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=eds.cleft_A1_coupling,eds.dihedral_A1_coupling,eds.cleft_A2_coupling,eds.dihedral_A2_coupling,eds.cleft_A3_coupling,eds.dihedral_A3_coupling,eds.bias,eds.force2 FILE=factin_3mono_ATP_flatten_ang_3phi_3dist_extraflat_i100ps_lm0.01_p100.run.10000000.bias.dat STRIDE=5000
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_a_t_o_m_s.html">DUMPATOMS</a> STRIDE=5000 FILE=factin_3mono_ATP_flatten_ang_3phi_3dist_extraflat_i100ps_lm0.01_p100.run.10000000.cg4.xyz ATOMS=A1-b1,A1-b2,A1-b3,A1-b4,A2-b1,A2-b2,A2-b3,A2-b4,A3-b1,A3-b2,A3-b3,A3-b4
</pre>{% endraw %}
