**Project ID:** [plumID:19.021]({{ '/' | absolute_url }}eggs/19/021/)  
**Source:** ./Trajectories/EDS-flattening-atomistic/flatten-gactin-2cv-us/run_gatpu_us_cacb_k5000/actin-gatpu_ionized.run.20000000.plumed.dat  
**Originally used with PLUMED version:** 2.5b  
**Stable:** [raw zipped stdout](actin-gatpu_ionized.run.20000000.plumed.dat.plumed.stdout.txt.zip) - [stderr](actin-gatpu_ionized.run.20000000.plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](actin-gatpu_ionized.run.20000000.plumed.dat.plumed_master.stdout.txt.zip) - [stderr](actin-gatpu_ionized.run.20000000.plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue">#INCLUDE FILE=../../actin-gatpu_cv_backbonecb.txt</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_i_n_c_l_u_d_e.html">INCLUDE</a> FILE=<a href="actin-gatpu_cv_cacb.txt.html">actin-gatpu_cv_cacb.txt</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=CA1 LABEL=b1
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=CA2 LABEL=b2
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=CA3 LABEL=b3
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=CA4 LABEL=b4

<span style="color:blue">#cleft_dist</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=b2,b4 LABEL=cleft_dist
<a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=b2,b1,b3,b4 LABEL=dihedral

dcn: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=dihedral POWERS=1 COEFFICIENTS=-1 PERIODIC=NO

<span style="color:blue">#bias mean </span>
us: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=cleft_dist,dcn AT=2.06155,0.110262 KAPPA=5000,5000 STRIDE=2

<span style="color:blue">#write every 10 ps</span>
<span style="color:blue">#</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=cleft_dist,dihedral,us.bias,us.force2 FILE=actin-gatpu_ionized.run.20000000.colvars.dat STRIDE=5000
</pre>{% endraw %}
