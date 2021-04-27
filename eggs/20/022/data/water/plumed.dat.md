**Project ID:** [plumID:20.022]({{ '/' | absolute_url }}eggs/20/022/)  
**Source:** water/plumed.dat  
**Originally used with PLUMED version:** 2.8  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_a_d.html">LOAD</a> FILE=LennardJones.cpp

<span style="color:blue">#+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++#</span>
<span style="color:blue">#                                                                       #</span>
<span style="color:blue">#  This input generates a simulation that samples all the intermediate  #</span>
<span style="color:blue">#  states needed for performing thermodynamic integration               #</span>
<span style="color:blue">#                                                                       #</span>
<span style="color:blue">#+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++#</span>

eneWAT: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a>
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_e_n_n_a_r_d_j_o_n_e_s.html">LENNARDJONES</a> ...
 LABEL=eneLJ
 GROUPA=1-1152:3
 SIGMA=0.31536
 EPSILON=0.64852
 RCUT=0.85
 NLIST
 NL_CUTOFF=1.0
 NL_STRIDE=10
... <a href="https://plumed.github.io/doc-master/user-doc/html/_l_e_n_n_a_r_d_j_o_n_e_s.html">LENNARDJONES</a>
DeltaU: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=eneLJ,eneWAT FUNC=x-y PERIODIC=NO

ecv: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_c_v__l_i_n_e_a_r.html">ECV_LINEAR</a> ARG=DeltaU TEMP=443
opes: <a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_e_s__e_x_p_a_n_d_e_d.html">OPES_EXPANDED</a> ARG=ecv.* PACE=100

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=eneWAT,eneLJ,DeltaU,opes.* STRIDE=100 FILE=COLVAR

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
<span style="color:blue"></span>
</pre>{% endraw %}
