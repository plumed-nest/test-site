**Project ID:** [plumID:24.020]({{ '/' | absolute_url }}eggs/24/020/)  
**Source:** ala2/imetad/plumed_z1z2_10000.dat  
**Originally used with PLUMED version:** 2.8.1  
**Stable:** [zipped raw stdout](plumed_z1z2_10000.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_z1z2_10000.dat.plumed.stderr.txt.zip) - [stderr](plumed_z1z2_10000.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed_z1z2_10000.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_z1z2_10000.dat.plumed_master.stderr.txt.zip) - [stderr](plumed_z1z2_10000.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/ala2/imetad/plumed_z1z2_10000.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed_z1z2_10000.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-failed-red.svg" alt="tested onv2.10" /></a></td></tr><tr><td style="padding:1px"><a href="plumed_z1z2_10000.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-failed-red.svg" alt="tested onmaster" /></a></td></tr><tr><td style="padding:1px"><img src="https://img.shields.io/badge/with-LOAD-yellow.svg" alt="tested on master" /></td></tr>
</table></div></div>
<pre style="width=97%;">
<span class="plumedtooltip" style="color:green">LOAD<span class="right">Loads a library, possibly defining new actions. <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">FILE<span class="right">file to be loaded<i></i></span></span>=Graph.cpp

<span style="color:blue" class="comment"># Calculate the collective variables</span>
<span style="display:none;" id="data/ala2/imetad/plumed_z1z2_10000.dat">The LOAD action with label <b></b> calculates something</span><b name="data/ala2/imetad/plumed_z1z2_10000.datHEAVY" onclick='showPath("data/ala2/imetad/plumed_z1z2_10000.dat","data/ala2/imetad/plumed_z1z2_10000.datHEAVY","data/ala2/imetad/plumed_z1z2_10000.datHEAVY","brown")'>HEAVY</b>: <span class="plumedtooltip" style="color:green">GROUP<span class="right">Define a group of atoms so that a particular list of atoms can be referenced with a single label in definitions of CVs or virtual atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_g_r_o_u_p.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS<span class="right">the numerical indexes for the set of atoms in the group<i></i></span></span>=2,5,6,7,9,11,15,16,17,19

<span style="display:none;" id="data/ala2/imetad/plumed_z1z2_10000.datHEAVY">The GROUP action with label <b>HEAVY</b> calculates something</span><b name="data/ala2/imetad/plumed_z1z2_10000.datphi" onclick='showPath("data/ala2/imetad/plumed_z1z2_10000.dat","data/ala2/imetad/plumed_z1z2_10000.datphi","data/ala2/imetad/plumed_z1z2_10000.datphi","brown")'>phi</b>: <span class="plumedtooltip" style="color:green">TORSION<span class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=5,7,9,15
<span style="display:none;" id="data/ala2/imetad/plumed_z1z2_10000.datphi">The TORSION action with label <b>phi</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">phi.value</td><td>the TORSION involving these atoms</td></tr></table></span><b name="data/ala2/imetad/plumed_z1z2_10000.datpsi" onclick='showPath("data/ala2/imetad/plumed_z1z2_10000.dat","data/ala2/imetad/plumed_z1z2_10000.datpsi","data/ala2/imetad/plumed_z1z2_10000.datpsi","brown")'>psi</b>: <span class="plumedtooltip" style="color:green">TORSION<span class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=7,9,15,17

<span style="display:none;" id="data/ala2/imetad/plumed_z1z2_10000.datpsi">The TORSION action with label <b>psi</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">psi.value</td><td>the TORSION involving these atoms</td></tr></table></span><span class="plumedtooltip" style="color:green">GRAPH<span class="right">This action is not part of PLUMED and was included by using a LOAD command <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></span></span> ...
 LABEL=<b name="data/ala2/imetad/plumed_z1z2_10000.datmodel" onclick='showPath("data/ala2/imetad/plumed_z1z2_10000.dat","data/ala2/imetad/plumed_z1z2_10000.datmodel","data/ala2/imetad/plumed_z1z2_10000.datmodel","brown")'>model</b>
 ATOMS=<b name="data/ala2/imetad/plumed_z1z2_10000.datHEAVY">HEAVY</b>
 RCUT=1.0
 MODEL=model.pt
... GRAPH
<br/><span class="plumedtooltip" style="color:green">METAD<span class="right">Used to performed metadynamics on one or more collective variables. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_e_t_a_d.html" style="color:green">More details</a><i></i></span></span> ...
 <span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/ala2/imetad/plumed_z1z2_10000.datmetad" onclick='showPath("data/ala2/imetad/plumed_z1z2_10000.dat","data/ala2/imetad/plumed_z1z2_10000.datmetad","data/ala2/imetad/plumed_z1z2_10000.datmetad","brown")'>metad</b>
 <span class="plumedtooltip">ARG<span class="right">the labels of the scalars on which the bias will act<i></i></span></span>=model.node-0,model.node-1
 <span class="plumedtooltip">TEMP<span class="right">the system temperature - this is only needed if you are doing well-tempered metadynamics<i></i></span></span>=300
 <span class="plumedtooltip">SIGMA<span class="right">the widths of the Gaussian hills<i></i></span></span>=0.4,0.4
 <span class="plumedtooltip">HEIGHT<span class="right">the heights of the Gaussian hills<i></i></span></span>=1.25
 <span class="plumedtooltip">FILE<span class="right"> a file in which the list of added hills is stored<i></i></span></span>=HILLS   <span style="color:blue" class="comment"># File where the information of the gaussians is printed</span>
 <span class="plumedtooltip">BIASFACTOR<span class="right">use well tempered metadynamics and use this bias factor<i></i></span></span>=5
 <span class="plumedtooltip">PACE<span class="right">the frequency for hill addition<i></i></span></span>=10000
 <span class="plumedtooltip">GRID_MIN<span class="right">the lower bounds for the grid<i></i></span></span>=-10.0,-20.0 
 <span class="plumedtooltip">GRID_MAX<span class="right">the upper bounds for the grid<i></i></span></span>=30.0,15.0 
 <span class="plumedtooltip">GRID_BIN<span class="right">the number of bins for the grid<i></i></span></span>=650,650
 <span class="plumedtooltip">ACCELERATION<span class="right"> Set to TRUE if you want to compute the metadynamics acceleration factor<i></i></span></span>
... METAD
<br/><span style="display:none;" id="data/ala2/imetad/plumed_z1z2_10000.datmetad">The METAD action with label <b>metad</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">metad.bias</td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">metad.acc</td><td>the metadynamics acceleration factor</td></tr></table></span><span class="plumedtooltip" style="color:green">COMMITTOR<span class="right">Does a committor analysis. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_m_m_i_t_t_o_r.html" style="color:green">More details</a><i></i></span></span> ...
   <span class="plumedtooltip">ARG<span class="right">the labels of the values which is being used to define the committor surface<i></i></span></span>=<b name="data/ala2/imetad/plumed_z1z2_10000.datphi">phi</b>
   <span class="plumedtooltip">BASIN_UL1<span class="right">List of upper limits for basin #<i></i></span></span>=1.5
   <span class="plumedtooltip">BASIN_LL1<span class="right">List of lower limits for basin #<i></i></span></span>=0.5
   <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the CVs are analyzed<i></i></span></span>=500
   <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output the reached basin<i></i></span></span>=PASS
...
<br/><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=<b name="data/ala2/imetad/plumed_z1z2_10000.datphi">phi</b>,<b name="data/ala2/imetad/plumed_z1z2_10000.datmetad">metad.bias</b>,<b name="data/ala2/imetad/plumed_z1z2_10000.datmetad">metad.acc</b> <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=500 <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=COLVAR
</pre>
{% endraw %}
