**Project ID:** [plumID:19.049]({{ '/' | absolute_url }}eggs/19/049/)  
**Source:** plumed_lj_gas_liquid.dat  
**Originally used with PLUMED version:** not specified  
**Stable:** [raw zipped stdout](plumed_lj_gas_liquid.dat.plumed.stdout.txt.zip) - [stderr](plumed_lj_gas_liquid.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_lj_gas_liquid.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_lj_gas_liquid.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># Calculate the coordination numbers of the 100 atoms in the system</span>
lq: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIES=1-100 SWITCH={CUBIC D_0=0.45  D_MAX=0.55} LOWMEM
<span style="color:blue"># Construct a contact matrix between the atoms in the system   </span>
cm: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t__m_a_t_r_i_x.html">CONTACT_MATRIX</a> ATOMS=lq  SWITCH={CUBIC D_0=0.45  D_MAX=0.55} 
<span style="color:blue"># Use depth first clustering to identify the sizes of the clusters                     </span>
dfs: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_f_s_c_l_u_s_t_e_r_i_n_g.html">DFSCLUSTERING</a> MATRIX=cm 
<span style="color:blue"># Compute the sum of the coordination numbers for the atoms in the largest cluster                                                         </span>
clust1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_l_u_s_t_e_r__p_r_o_p_e_r_t_i_e_s.html">CLUSTER_PROPERTIES</a> CLUSTERS=dfs CLUSTER=1 SUM  
<span style="color:blue"># Apply a metadynamics bias on the sum of the coordination number for the atoms </span>
<span style="color:blue"># in the largest cluster so as to force droplets of liquid to condense and evaporate </span>
mt: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
 ARG=clust1.sum SIGMA=10. HEIGHT=2. PACE=500 
 TEMP=80.7 BIASFACTOR=50 GRID_MIN=0 GRID_MAX=6000
... 
<span style="color:blue"># Calculate the number of atoms in the largest cluster </span>
ss: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_l_u_s_t_e_r__n_a_t_o_m_s.html">CLUSTER_NATOMS</a> CLUSTERS=dfs CLUSTER=1
<span style="color:blue"># Output the number of atoms in the largest cluster to a file</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=ss FILE=colvar
</pre>{% endraw %}
