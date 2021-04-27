**Project ID:** [plumID:20.026]({{ '/' | absolute_url }}eggs/20/026/)  
**Source:** plumed.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
rmsd_a: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_u_l_t_i__r_m_s_d.html">MULTI_RMSD</a> REFERENCE=OBP_lis_final.pdb TYPE=MULTI-OPTIMAL
rmsd_b: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_u_l_t_i__r_m_s_d.html">MULTI_RMSD</a> REFERENCE=OBP_lsd_final.pdb TYPE=MULTI-OPTIMAL
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=rmsd_a,rmsd_b  AT=0.375,0.425   KAPPA=100000.0,100000.0 LABEL=restraint
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=rmsd_a,rmsd_b,restraint.bias STRIDE=100 FILE=COLVAR 
</pre>{% endraw %}
