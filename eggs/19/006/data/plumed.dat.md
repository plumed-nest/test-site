**Project ID:** [plumID:19.006]({{ '/' | absolute_url }}eggs/19/006/)  
**Source:** plumed.dat  
**Originally used with PLUMED version:** 2.5.0  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> LABEL=phi ATOMS=5,7,9,15
<a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> LABEL=psi ATOMS=7,9,15,17
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=phi,psi SIGMA=0.3,0.3 HEIGHT=4 PACE=1 WALKERS_MPI FLYING_GAUSSIAN FILE=HILLS LABEL=restraint
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=phi,psi,restraint.bias STRIDE=100 FILE=COLVAR

</pre>{% endraw %}
