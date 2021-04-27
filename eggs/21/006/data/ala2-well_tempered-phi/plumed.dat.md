**Project ID:** [plumID:21.006]({{ '/' | absolute_url }}eggs/21/006/)  
**Source:** ala2-well_tempered-phi/plumed.dat  
**Originally used with PLUMED version:** 2.8  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>

<span style="color:blue">#+++++++++++++++++++++++++++++++++++++++++++++++++++#</span>
<span style="color:blue">#                                                   #</span>
<span style="color:blue">#  This input generates a well-tempered simulation  #</span>
<span style="color:blue">#  that samples along the phi collective variable   #</span>
<span style="color:blue">#                                                   #</span>
<span style="color:blue">#+++++++++++++++++++++++++++++++++++++++++++++++++++#</span>

phi: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=5,7,9,15
psi: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=7,9,15,17
ene: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a>

opes: <a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_e_s__m_e_t_a_d.html">OPES_METAD</a> ...
  ARG=phi
  FILE=Kernels.data
  PACE=500
  BARRIER=50
  SIGMA=0.15
  STATE_WFILE=State.data
  NLIST
...

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FMT=%g STRIDE=500 FILE=Colvar.data ARG=phi,psi,ene,opes.bias,opes.rct,opes.zed,opes.nker

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
<span style="color:blue"></span>
<span style="color:blue">If no SIGMA is provided, it will be automatically guessed.</span>
<span style="color:blue">The option NLIST activates a neighbor list that speeds up the computation.</span>
<span style="color:blue"></span>
<span style="color:blue">The main advantage of using OPES_METAD over a multiumbrella OPES_EXPANDED is that it is much easier to handle multiple collective variables.</span>
</pre>{% endraw %}
