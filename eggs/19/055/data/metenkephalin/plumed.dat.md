**Project ID:** [plumID:19.055]({{ '/' | absolute_url }}eggs/19/055/)  
**Source:** metenkephalin/plumed.dat  
**Originally used with PLUMED version:** 2.5.0  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
d1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1,60
d2: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=15,50
d3: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=68,50
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=d1,d2,d3 SIGMA=0.02,0.02,0.02 HEIGHT=3 PACE=1 WALKERS_MPI FLYING_GAUSSIAN FILE=HILLS LABEL=restraint
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=d1,d2,d3,restraint.bias STRIDE=10 FILE=colvar 
</pre>{% endraw %}
