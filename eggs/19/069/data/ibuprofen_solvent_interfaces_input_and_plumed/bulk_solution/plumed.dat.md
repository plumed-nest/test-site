**Project ID:** [plumID:19.069]({{ '/' | absolute_url }}eggs/19/069/)  
**Source:** ibuprofen_solvent_interfaces_input_and_plumed/bulk_solution/plumed.dat  
**Originally used with PLUMED version:** 2.3  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># celnter of mass of all solvent molecules</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_i_n_c_l_u_d_e.html">INCLUDE</a> FILE=<a href="COM_solvent.dat.html">COM_solvent.dat</a>
<span style="color:blue"># solvent group </span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_i_n_c_l_u_d_e.html">INCLUDE</a> FILE=<a href="groups.dat.html">groups.dat</a> 
<span style="color:blue"># defining distance </span>
d: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=s1 GROUPB=solvent  
<span style="color:blue">#printing all d.z </span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_m_u_l_t_i_c_o_l_v_a_r.html">DUMPMULTICOLVAR</a> DATA=d FILE=MULTICOLVAR.xyz
<span style="color:blue">#gyration radius</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_g_y_r_a_t_i_o_n.html">GYRATION</a> TYPE=RADIUS ATOMS=1-15 LABEL=rg
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=rg STRIDE=1 FILE=gyration

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
<span style="color:blue"></span>
</pre>{% endraw %}
