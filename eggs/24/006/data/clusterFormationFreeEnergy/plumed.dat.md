**Project ID:** [plumID:24.006]({{ '/' | absolute_url }}eggs/24/006/)  
**Source:** clusterFormationFreeEnergy/plumed.dat  
**Originally used with PLUMED version:** 2.8  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/clusterFormationFreeEnergy/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-failed-red.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<div class="tooltip" style="color:blue"># vim:ft=plumed<div class="right">Enables syntax highlighting for PLUMED files in vim. See <a href="https://www.plumed.org/doc-master/user-doc/html/_vim_syntax.html">here for more details. </a><i></i></div></div>
<div class="tooltip" style="color:green">UNITS<div class="right">This command sets the internal units for the code. <a href="https://www.plumed.org/doc-master/user-doc/html/_u_n_i_t_s.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">LENGTH<div class="right">the units of lengths<i></i></div></div>=A <div class="tooltip">TIME<div class="right">the units of time<i></i></div></div>=ps <div class="tooltip">ENERGY<div class="right">the units of energy<i></i></div></div>=eV  <span style="color:blue" class="comment">#KB=1.380649e-23 J/K </span>
<span style="display:none;" id="data/clusterFormationFreeEnergy/plumed.dat">The UNITS action with label <b></b> calculates something</span><b name="data/clusterFormationFreeEnergy/plumed.datc1" onclick='showPath("data/clusterFormationFreeEnergy/plumed.dat","data/clusterFormationFreeEnergy/plumed.datc1","data/clusterFormationFreeEnergy/plumed.datc1","brown")'>c1</b>: <div class="tooltip" style="color:green">COORDINATIONNUMBER<div class="right">Calculate the coordination numbers of atoms so that you can then calculate functions of the distribution of <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">SPECIES<div class="right">this keyword is used for colvars such as coordination number<i></i></div></div>=1-300:3 <div class="tooltip">SWITCH<div class="right">the switching function that it used in the construction of the contact matrix<i></i></div></div>={RATIONAL R_0=1 D_0=3.5 D_MAX=4.5} <div class="tooltip">LOWMEM<div class="right"> this flag does nothing and is present only to ensure back-compatibility<i></i></div></div>
<span style="display:none;" id="data/clusterFormationFreeEnergy/plumed.datc1">The COORDINATIONNUMBER action with label <b>c1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr></table></span><b name="data/clusterFormationFreeEnergy/plumed.datmat" onclick='showPath("data/clusterFormationFreeEnergy/plumed.dat","data/clusterFormationFreeEnergy/plumed.datmat","data/clusterFormationFreeEnergy/plumed.datmat","brown")'>mat</b>: <div class="tooltip" style="color:green">CONTACT_MATRIX<div class="right">Adjacency matrix in which two atoms are adjacent if they are within a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_t_a_c_t__m_a_t_r_i_x.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the atoms for which you would like to calculate the adjacency matrix<i></i></div></div>=<b name="data/clusterFormationFreeEnergy/plumed.datc1">c1</b> <div class="tooltip">SWITCH<div class="right">specify the switching function to use between two sets of indistinguishable atoms<i></i></div></div>={RATIONAL R_0=1 D_0=3.5 D_MAX=4.5}
<span style="display:none;" id="data/clusterFormationFreeEnergy/plumed.datmat">The CONTACT_MATRIX action with label <b>mat</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">mat.value</td><td>a matrix containing the weights for the bonds between each pair of atoms</td></tr></table></span><b name="data/clusterFormationFreeEnergy/plumed.datdfs" onclick='showPath("data/clusterFormationFreeEnergy/plumed.dat","data/clusterFormationFreeEnergy/plumed.datdfs","data/clusterFormationFreeEnergy/plumed.datdfs","brown")'>dfs</b>: <div class="tooltip" style="color:green">DFSCLUSTERING<div class="right">Find the connected components of the matrix using the depth first search clustering algorithm. <a href="https://www.plumed.org/doc-master/user-doc/html/_d_f_s_c_l_u_s_t_e_r_i_n_g.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">MATRIX<div class="right">the input matrix (can use ARG instead)<i></i></div></div>=<b name="data/clusterFormationFreeEnergy/plumed.datmat">mat</b> <div class="tooltip">LOWMEM<div class="right"> this flag does nothing and is present only to ensure back-compatibility<i></i></div></div>
<span style="display:none;" id="data/clusterFormationFreeEnergy/plumed.datdfs">The DFSCLUSTERING action with label <b>dfs</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">dfs.value</td><td>vector with length that is equal to the number of rows in the input matrix</td></tr></table></span><b name="data/clusterFormationFreeEnergy/plumed.datclust1" onclick='showPath("data/clusterFormationFreeEnergy/plumed.dat","data/clusterFormationFreeEnergy/plumed.datclust1","data/clusterFormationFreeEnergy/plumed.datclust1","brown")'>clust1</b>: <div class="tooltip" style="color:green">CLUSTER_PROPERTIES<div class="right">Calculate properties of the distribution of some quantities that are part of a connected component <a href="https://www.plumed.org/doc-master/user-doc/html/_c_l_u_s_t_e_r__p_r_o_p_e_r_t_i_e_s.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">CLUSTERS<div class="right">the label of the action that does the clustering<i></i></div></div>=<b name="data/clusterFormationFreeEnergy/plumed.datdfs">dfs</b> <div class="tooltip">CLUSTER<div class="right"> which cluster would you like to look at 1 is the largest cluster, 2 is the second largest, 3 is the the third largest and so on<i></i></div></div>=1 <div class="tooltip">SUM<div class="right"> calculate the sum of all the quantities<i></i></div></div> LOWMEM 
<span style="display:none;" id="data/clusterFormationFreeEnergy/plumed.datclust1">The CLUSTER_PROPERTIES action with label <b>clust1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">clust1.sum</td><td>the sum of the colvars</td></tr></table></span><b name="data/clusterFormationFreeEnergy/plumed.datnat" onclick='showPath("data/clusterFormationFreeEnergy/plumed.dat","data/clusterFormationFreeEnergy/plumed.datnat","data/clusterFormationFreeEnergy/plumed.datnat","brown")'>nat</b>: <div class="tooltip" style="color:green">CLUSTER_NATOMS<div class="right">Calculate the number of atoms in the cluster of interest <a href="https://www.plumed.org/doc-master/user-doc/html/_c_l_u_s_t_e_r__n_a_t_o_m_s.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">CLUSTERS<div class="right">the label of the action that does the clustering<i></i></div></div>=<b name="data/clusterFormationFreeEnergy/plumed.datdfs">dfs</b> <div class="tooltip">CLUSTER<div class="right"> which cluster would you like to look at 1 is the largest cluster, 2 is the second largest, 3 is the the third largest and so on<i></i></div></div>=1  
<span style="display:none;" id="data/clusterFormationFreeEnergy/plumed.datnat">The CLUSTER_NATOMS action with label <b>nat</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">nat.value</td><td>the number of atoms in the cluster</td></tr></table></span><b name="data/clusterFormationFreeEnergy/plumed.datmt" onclick='showPath("data/clusterFormationFreeEnergy/plumed.dat","data/clusterFormationFreeEnergy/plumed.datmt","data/clusterFormationFreeEnergy/plumed.datmt","brown")'>mt</b>: <div class="tooltip" style="color:green">METAD<div class="right">Used to performed metadynamics on one or more collective variables. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_e_t_a_d.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/clusterFormationFreeEnergy/plumed.datclust1">clust1.sum</b> ...
 <div class="tooltip">PACE<div class="right">the frequency for hill addition<i></i></div></div>=500 <div class="tooltip">HEIGHT<div class="right">the heights of the Gaussian hills<i></i></div></div>=0.02 <div class="tooltip">BIASFACTOR<div class="right">use well tempered metadynamics and use this bias factor<i></i></div></div>=50   
 <div class="tooltip">SIGMA<div class="right">the widths of the Gaussian hills<i></i></div></div>=1 <div class="tooltip">TEMP<div class="right">the system temperature - this is only needed if you are doing well-tempered metadynamics<i></i></div></div>=373  
 <div class="tooltip">FILE<div class="right"> a file in which the list of added hills is stored<i></i></div></div>=HILLS <div class="tooltip">GRID_MIN<div class="right">the lower bounds for the grid<i></i></div></div>=0 <div class="tooltip">GRID_MAX<div class="right">the upper bounds for the grid<i></i></div></div>=500 <div class="tooltip">CALC_RCT<div class="right"> calculate the c(t) reweighting factor and use that to obtain the normalized bias [rbias=bias-rct]<i></i></div></div>
...
<br/><span style="display:none;" id="data/clusterFormationFreeEnergy/plumed.datmt">The METAD action with label <b>mt</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">mt.bias</td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">mt.rbias</td><td>the instantaneous value of the bias normalized using the c(t) reweighting factor [rbias=bias-rct]</td></tr><tr><td width="5%">mt.rct</td><td>the reweighting factor c(t)</td></tr></table></span><div class="tooltip" style="color:green">UPPER_WALLS<div class="right">Defines a wall for the value of one or more collective variables, <a href="https://www.plumed.org/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the arguments on which the bias is acting<i></i></div></div>=<b name="data/clusterFormationFreeEnergy/plumed.datclust1">clust1.sum</b> <div class="tooltip">AT<div class="right">the positions of the wall<i></i></div></div>=250.0 <div class="tooltip">KAPPA<div class="right">the force constant for the wall<i></i></div></div>=0.1 <div class="tooltip">EXP<div class="right"> the powers for the walls<i></i></div></div>=2 <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/clusterFormationFreeEnergy/plumed.datuwall" onclick='showPath("data/clusterFormationFreeEnergy/plumed.dat","data/clusterFormationFreeEnergy/plumed.datuwall","data/clusterFormationFreeEnergy/plumed.datuwall","brown")'>uwall</b> 
<span style="display:none;" id="data/clusterFormationFreeEnergy/plumed.datuwall">The UPPER_WALLS action with label <b>uwall</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">uwall.bias</td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">uwall.force2</td><td>the instantaneous value of the squared force due to this bias potential</td></tr></table></span><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div> <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=COLVAR <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=500
</pre>
{% endraw %}