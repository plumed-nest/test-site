**Project ID:** [plumID:19.068]({{ '/' | absolute_url }}eggs/19/068/)  
**Source:** ala4/plumed-opes.dat  
**Originally used with PLUMED version:** 2.7  
**Stable:** [raw zipped stdout](plumed-opes.dat.plumed.stdout.txt.zip) - [stderr](plumed-opes.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed-opes.dat.plumed_master.stdout.txt.zip) - [stderr](plumed-opes.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>

phi1: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=5,7,9,15
phi2: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=15,17,19,25
phi3: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=25,27,29,35
psi1: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=7,9,15,17
psi2: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=17,19,25,27
psi3: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=27,29,35,37

opes: <a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_e_s__m_e_t_a_d.html">OPES_METAD</a> ...
  ARG=phi1,phi2,phi3,psi1,psi2,psi3
  FILE=Kernels.data
  TEMP=300.0
  PACE=500
  SIGMA=0.15,0.15,0.15,0.15,0.15,0.15
  BARRIER=50
  BIASFACTOR=10
  STATE_WFILE=State.data
  STATE_WSTRIDE=500000
  STORE_STATES
...

<span style="color:blue"># Since we are in 6D it is convenient to print the colvar more often</span>
<span style="color:blue"># (STRIDE=50 instead of STRIDE=500), it will help with the reweighting</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FMT=%g STRIDE=50 FILE=Colvar.data ARG=*

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
<span style="color:blue"></span>
<span style="color:blue">A better performing result can be obtained with the following simpler input:</span>
<span style="color:blue"></span>
<span style="color:blue">  opes: OPES_METAD ARG=phi1,phi2,phi3,psi1,psi2,psi3 PACE=50 BARRIER=50 NLIST</span>
<span style="color:blue"></span>
<span style="color:blue">but it was not used, to have a more fair comparison with standard metadynamics ala2 simulations.</span>
<span style="color:blue">(if not set, SIGMA is chosen adaptively, similarly to METAD ADAPTIVE=DIFF)</span>
</pre>{% endraw %}
