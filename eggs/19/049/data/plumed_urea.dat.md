**Project ID:** [plumID:19.049]({{ '/' | absolute_url }}eggs/19/049/)  
**Source:** plumed_urea.dat  
**Originally used with PLUMED version:** not specified  
**Stable:** [raw zipped stdout](plumed_urea.dat.plumed.stdout.txt.zip) - [stderr](plumed_urea.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_urea.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_urea.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># Use the vector connecting the carbon and oxygen atoms of each urea</span>
<span style="color:blue"># molecule in the system to define the orientations of the molecules </span>
m1: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_e_c_u_l_e_s.html">MOLECULES</a> ...
  MOL1=1,2,1
  MOL2=9,10,9
...	 

<span style="color:blue"># Calculate the SMAC parameter for each of the molecules.  Essentially</span>
<span style="color:blue"># measures whether or not molecules in the first coordination sphere </span>
<span style="color:blue"># have a similar orientation to the central molecule.</span>
smac: <a href="https://plumed.github.io/doc-master/user-doc/html/_s_m_a_c.html">SMAC</a> ...
   SPECIES=m1 
   SWITCH={RATIONAL D_0=0.639 R_0=0.1 D_MAX=0.64} 
   KERNEL1={TRIANGULAR CENTER=0 SIGMA=0.8}
   KERNEL2={TRIANGULAR CENTER=pi SIGMA=0.7}
   SWITCH_COORD={RATIONAL R_0=0.001}
... 

<span style="color:blue"># Use a filter so as to ignore molecules that are not sat in a solid-like,</span>
<span style="color:blue"># ordered environment.</span>
ff: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_f_i_l_t_e_r__m_o_r_e.html">MFILTER_MORE</a> DATA=smac SWITCH={GAUSSIAN D_0=0.49 R_0=0.5 D_MAX=0.5}
<span style="color:blue"># Build a contact matrix for the molecules that are in a part of the simulation </span>
<span style="color:blue"># box where the structure is ordered</span>
c1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t__m_a_t_r_i_x.html">CONTACT_MATRIX</a> ATOMS=ff SWITCH={RATIONAL D_0=0.639 R_0=0.01 D_MAX=0.64} 
<span style="color:blue"># Perform depth first search clustering on the contact matrix</span>
dfs: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_f_s_c_l_u_s_t_e_r_i_n_g.html">DFSCLUSTERING</a> MATRIX=c1
<span style="color:blue"># Find the sum of the coordination numbers for the atoms in this largest cluster.</span>
cc1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_l_u_s_t_e_r__p_r_o_p_e_r_t_i_e_s.html">CLUSTER_PROPERTIES</a> ...
  CLUSTERS=dfs CLUSTER=1 
  MORE_THAN={GAUSSIAN D_0=0.49 R_0=0.5 D_MAX=0.5}
... 
<span style="color:blue"># Print information on the number of atoms in the cluster to a file.</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=cc1.* FILE=colvar
</pre>{% endraw %}
