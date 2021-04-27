**Project ID:** [plumID:19.049]({{ '/' | absolute_url }}eggs/19/049/)  
**Source:** plumed_GeTe.dat  
**Originally used with PLUMED version:** not specified  
**Stable:** [raw zipped stdout](plumed_GeTe.dat.plumed.stdout.txt.zip) - [stderr](plumed_GeTe.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_GeTe.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_GeTe.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># Calculate the Steinhardt Q6 vector for each of the atoms in the system</span>
<span style="color:blue"># N.B. Fewer atoms are used here than were used in the paper for technical reasons</span>
q6: <a href="https://plumed.github.io/doc-master/user-doc/html/_q6.html">Q6</a> SPECIES=1-200 SWITCH={GAUSSIAN D_0=5.29 R_0=0.01 D_MAX=5.3} LOWMEM
<span style="color:blue"># Calculate the local Steinhardt parameter for each of the atoms in the system </span>
<span style="color:blue"># in the manner described by ten Wolde and Frenkel.</span>
lq6: <a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_c_a_l__q6.html">LOCAL_Q6</a> SPECIES=q6 SWITCH={GAUSSIAN D_0=5.29 R_0=0.01 D_MAX=5.3} LOWMEM
<span style="color:blue"># Now select only those atoms that have a local q6 parameter that is larger than a certain threshold</span>
flq6: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_f_i_l_t_e_r__m_o_r_e.html">MFILTER_MORE</a> DATA=lq6 SWITCH={GAUSSIAN D_0=0.19 R_0=0.01 D_MAX=0.2}
<span style="color:blue"># Calculate the coordination number for those atoms that have a local q6 parameter that is larger than a certain threshold</span>
cc: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIES=flq6 SWITCH={GAUSSIAN D_0=3.59 R_0=0.01 D_MAX=3.6}
<span style="color:blue"># Now select those atoms that are coordinated to six or more atoms that have a value for the local q6 parameter that is larger than </span>
<span style="color:blue"># a certain threshold</span>
fcc: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_f_i_l_t_e_r__m_o_r_e.html">MFILTER_MORE</a> DATA=cc SWITCH={GAUSSIAN D_0=5.99 R_0=0.01 D_MAX=6.0}
<span style="color:blue"># Compute a contact matrix for the atoms that were selected using the previous command</span>
mat: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t__m_a_t_r_i_x.html">CONTACT_MATRIX</a> ATOMS=fcc SWITCH={GAUSSIAN D_0=3.59 R_0=0.01 D_MAX=3.6}
<span style="color:blue"># Perform a depth first search clustering on this matrix</span>
dfs: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_f_s_c_l_u_s_t_e_r_i_n_g.html">DFSCLUSTERING</a> MATRIX=mat
<span style="color:blue"># Output the atoms in the largest cluster that was identified</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_o_u_t_p_u_t__c_l_u_s_t_e_r.html">OUTPUT_CLUSTER</a> CLUSTERS=dfs CLUSTER=1 FILE=cluster1.xyz
<span style="color:blue"># Calculate the number of clusters that contain 27 or more atoms that have ordered neighbors. </span>
nclust: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_l_u_s_t_e_r__d_i_s_t_r_i_b_u_t_i_o_n.html">CLUSTER_DISTRIBUTION</a> ... 
  CLUSTERS=dfs 
  TRANSFORM={GAUSSIAN D_0=5.99 R_0=0.01 D_MAX=6.0} 
  MORE_THAN={GAUSSIAN D_0=26.99 R_0=0.01 D_MAX=27}
... 
<span style="color:blue"># Output the number of clusters to a file</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=nclust.* FILE=colvar
</pre>{% endraw %}
