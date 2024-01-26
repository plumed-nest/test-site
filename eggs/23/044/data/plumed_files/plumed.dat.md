**Project ID:** [plumID:23.044]({{ '/' | absolute_url }}eggs/23/044/)  
**Source:** plumed_files/plumed.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/plumed_files/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<b name="data/plumed_files/plumed.datfull" onclick='showPath("data/plumed_files/plumed.dat","data/plumed_files/plumed.datfull")'>full</b>: <div class="tooltip" style="color:green">GROUP<div class="right">Define a group of atoms so that a particular list of atoms can be referenced with a single label in definitions of CVs or virtual atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_g_r_o_u_p.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the numerical indexes for the set of atoms in the group<i></i></div></div>=1-60
<b name="data/plumed_files/plumed.datcpp" onclick='showPath("data/plumed_files/plumed.dat","data/plumed_files/plumed.datcpp")'>cpp</b>: <div class="tooltip" style="color:green">GROUP<div class="right">Define a group of atoms so that a particular list of atoms can be referenced with a single label in definitions of CVs or virtual atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_g_r_o_u_p.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the numerical indexes for the set of atoms in the group<i></i></div></div>=198-297
<b name="data/plumed_files/plumed.datc1" onclick='showPath("data/plumed_files/plumed.dat","data/plumed_files/plumed.datc1")'>c1</b>: <div class="tooltip" style="color:green">COORDINATION<div class="right">Calculate coordination numbers. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">GROUPA<div class="right">First list of atoms<i></i></div></div>=<b name="data/plumed_files/plumed.datfull">full</b> <div class="tooltip">GROUPB<div class="right">Second list of atoms (if empty, N*(N-1)/2 pairs in GROUPA are counted)<i></i></div></div>=<b name="data/plumed_files/plumed.datcpp">cpp</b> <div class="tooltip">R_0<div class="right">The r_0 parameter of the switching function<i></i></div></div>=0.25 
<span style="display:none;" id="data/plumed_files/plumed.datc1">The COORDINATION action with label <b>c1</b> calculates a scalar quantity</span><div class="tooltip" style="color:green">METAD<div class="right">Used to performed metadynamics on one or more collective variables. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_e_t_a_d.html" style="color:green">More details</a><i></i></div></div> ...
 <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/plumed_files/plumed.datmetad" onclick='showPath("data/plumed_files/plumed.dat","data/plumed_files/plumed.datmetad")'>metad</b>
 <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/plumed_files/plumed.datc1">c1</b>
 <div class="tooltip">HEIGHT<div class="right">the heights of the Gaussian hills<i></i></div></div>=2
 <div class="tooltip">PACE<div class="right">the frequency for hill addition<i></i></div></div>=20000
 <div class="tooltip">SIGMA<div class="right">the widths of the Gaussian hills<i></i></div></div>=0.5
 <div class="tooltip">BIASFACTOR<div class="right">use well tempered metadynamics and use this bias factor<i></i></div></div>=20
 <div class="tooltip">GRID_MIN<div class="right">the lower bounds for the grid<i></i></div></div>=0
 <div class="tooltip">GRID_MAX<div class="right">the upper bounds for the grid<i></i></div></div>=100
 <div class="tooltip">GRID_BIN<div class="right">the number of bins for the grid<i></i></div></div>=400
 <div class="tooltip">FILE<div class="right"> a file in which the list of added hills is stored<i></i></div></div>=HILLS
 <div class="tooltip">ACCELERATION<div class="right"> Set to TRUE if you want to compute the metadynamics acceleration factor<i></i></div></div>
... METAD
<br/><span style="display:none;" id="data/plumed_files/plumed.datmetad">The METAD action with label <b>metad</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">metad.bias</td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">metad.acc</td><td>the metadynamics acceleration factor</td></tr></table></span><div class="tooltip" style="color:green">COMMITTOR<div class="right">Does a committor analysis. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_m_m_i_t_t_o_r.html" style="color:green">More details</a><i></i></div></div> ...
  <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/plumed_files/plumed.datc1">c1</b>
  <div class="tooltip">STRIDE<div class="right"> the frequency with which the CVs are analyzed<i></i></div></div>=500
  <div class="tooltip">BASIN_LL1<div class="right">List of lower limits for basin #<i></i></div></div>=-0.1
  <div class="tooltip">BASIN_UL1<div class="right">List of upper limits for basin #<i></i></div></div>=0.1
... COMMITTOR
<br/><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/plumed_files/plumed.datc1">c1</b>,<b name="data/plumed_files/plumed.datmetad">metad</b> <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=COLVAR <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=500
</pre>
{% endraw %}
