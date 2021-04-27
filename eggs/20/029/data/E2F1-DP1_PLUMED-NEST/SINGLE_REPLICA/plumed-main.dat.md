**Project ID:** [plumID:20.029]({{ '/' | absolute_url }}eggs/20/029/)  
**Source:** E2F1-DP1_PLUMED-NEST/SINGLE_REPLICA/plumed-main.dat  
**Originally used with PLUMED version:** 2.6  
**Stable:** [raw zipped stdout](plumed-main.dat.plumed.stdout.txt.zip) - [stderr](plumed-main.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed-main.dat.plumed_master.stdout.txt.zip) - [stderr](plumed-main.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">MOLINFO</a> STRUCTURE=aacg.pdb
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=1-2885,2885-1712:-1,6605-6945,6945-2886:-1,2886-3812,6946-7896   

<a href="https://plumed.github.io/doc-master/user-doc/html/_i_n_c_l_u_d_e.html">INCLUDE</a> FILE=<a href="plumed_beads.dat.html">plumed_beads.dat</a>
<a href="https://plumed.github.io/doc-master/user-doc/html/_i_n_c_l_u_d_e.html">INCLUDE</a> FILE=<a href="plumed-restraints.dat.html">plumed-restraints.dat</a> 
<a href="https://plumed.github.io/doc-master/user-doc/html/_i_n_c_l_u_d_e.html">INCLUDE</a> FILE=<a href="plumed-SAXS_12q.dat.html">plumed-SAXS_12q.dat</a>
</pre>{% endraw %}
