**Project ID:** [plumID:21.006]({{ '/' | absolute_url }}eggs/21/006/)  
**Source:** ala2-multithermal/plumed.dat  
**Originally used with PLUMED version:** 2.8  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>

<span style="color:blue">#+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++#</span>
<span style="color:blue">#                                                                 #</span>
<span style="color:blue">#  This input generates a multicanonical simulation that samples  #</span>
<span style="color:blue">#  the temperature range 300K-1000K in a single simulation        #</span>
<span style="color:blue">#                                                                 #</span>
<span style="color:blue">#+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++#</span>

phi: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=5,7,9,15
psi: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=7,9,15,17
ene: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a>

ecv: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_c_v__m_u_l_t_i_t_h_e_r_m_a_l.html">ECV_MULTITHERMAL</a> ARG=ene MAX_TEMP=1000 STEPS_TEMP=4
opes: <a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_e_s__e_x_p_a_n_d_e_d.html">OPES_EXPANDED</a> ARG=ecv.* PACE=500 FILE=DeltaFs.data STATE_WFILE=State.data

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FMT=%g STRIDE=500 FILE=Colvar.data ARG=phi,psi,ene,opes.bias

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
<span style="color:blue"></span>
<span style="color:blue">If the number of STEPS_TEMP is not provided, it will be automatically guessed.</span>
<span style="color:blue">The resulting trajectory can be reweighted at any temperature in the range.</span>
</pre>{% endraw %}
