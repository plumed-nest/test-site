**Project ID:** [plumID:19.021]({{ '/' | absolute_url }}eggs/19/021/)  
**Source:** ./Trajectories/EDS-flattening-enm/us-flatten-dihed-mean/gatp-enm-12site_FEStart_eq175ns.flatten_us_k500/gatp-enm-12site_FEStart_eq175ns.flatten_us_k500.50ps.run.20000000.plumed.dat  
**Originally used with PLUMED version:** 2.5b  
**Stable:** [raw zipped stdout](gatp-enm-12site_FEStart_eq175ns.flatten_us_k500.50ps.run.20000000.plumed.dat.plumed.stdout.txt.zip) - [stderr](gatp-enm-12site_FEStart_eq175ns.flatten_us_k500.50ps.run.20000000.plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](gatp-enm-12site_FEStart_eq175ns.flatten_us_k500.50ps.run.20000000.plumed.dat.plumed_master.stdout.txt.zip) - [stderr](gatp-enm-12site_FEStart_eq175ns.flatten_us_k500.50ps.run.20000000.plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue">#cleft_dist</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=2,4 LABEL=cleft_dist
<a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=2,1,3,4 LABEL=dihedral

dcn: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=dihedral POWERS=1 COEFFICIENTS=-1 PERIODIC=NO

<span style="color:blue">#bias mean </span>
us: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=dcn AT=0.110262 KAPPA=500

<span style="color:blue">#write every 100 ps</span>
<span style="color:blue">#</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=cleft_dist,dcn,us.bias,us.force2 FILE=gatp-enm-12site_FEStart_eq175ns.flatten_us_k500.50ps.run.20000000.colvars.dat STRIDE=1000
</pre>{% endraw %}
