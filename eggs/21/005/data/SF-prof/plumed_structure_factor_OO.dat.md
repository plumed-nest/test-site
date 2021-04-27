**Project ID:** [plumID:21.005]({{ '/' | absolute_url }}eggs/21/005/)  
**Source:** SF-prof/plumed_structure_factor_OO.dat  
**Originally used with PLUMED version:** 2.7-mod  
**Stable:** [raw zipped stdout](plumed_structure_factor_OO.dat.plumed.stdout.txt.zip) - [stderr](plumed_structure_factor_OO.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_structure_factor_OO.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_structure_factor_OO.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_a_d.html">LOAD</a> FILE=../codes/StructureFactor_sphericallyAveraged.cpp

<a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=2-324:3,3-324:3 LABEL=O

sf: <a href="https://plumed.github.io/doc-master/user-doc/html/_s_t_r_u_c_t_u_r_e__f_a_c_t_o_r__s_p_h_e_r_i_c_a_l_l_y__a_v_e_r_a_g_e_d.html">STRUCTURE_FACTOR_SPHERICALLY_AVERAGED</a> N2_MAX=250 ATOMS=O 

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FMT=%g STRIDE=1 FILE=COLVAR-sfOO ARG=sf.*


</pre>{% endraw %}
