**Project ID:** [plumID:24.004]({{ '/' | absolute_url }}eggs/24/004/)  
**Source:** iron/plumed.start.dat  
**Originally used with PLUMED version:** 2.8.1  
**Stable:** [zipped raw stdout](plumed.start.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.start.dat.plumed.stderr.txt.zip) - [stderr](plumed.start.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.start.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.start.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.start.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/iron/plumed.start.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.start.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-failed-red.svg" alt="tested onv2.10" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.start.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-failed-red.svg" alt="tested onmaster" /></a></td></tr><tr><td style="padding:1px"><img src="https://img.shields.io/badge/with-LOAD-yellow.svg" alt="tested on master" /></td></tr>
</table></div></div>
<pre style="width=97%;">
<span class="plumedtooltip" style="color:green">LOAD<span class="right">Loads a library, possibly defining new actions. <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">FILE<span class="right">file to be loaded<i></i></span></span>=Graph.cpp

<span style="color:blue" class="comment"># Define groups for the CV</span>
<span style="display:none;" id="data/iron/plumed.start.dat">The LOAD action with label <b></b> calculates something</span><b name="data/iron/plumed.start.datC" onclick='showPath("data/iron/plumed.start.dat","data/iron/plumed.start.datC","data/iron/plumed.start.datC","brown")'>C</b>: <span class="plumedtooltip" style="color:green">GROUP<span class="right">Define a group of atoms so that a particular list of atoms can be referenced with a single label in definitions of CVs or virtual atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_g_r_o_u_p.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS<span class="right">the numerical indexes for the set of atoms in the group<i></i></span></span>=1-285
 
<span style="color:blue" class="comment"># Define the CV</span>
<span style="display:none;" id="data/iron/plumed.start.datC">The GROUP action with label <b>C</b> calculates something</span><span class="plumedtooltip" style="color:green">GRAPH<span class="right">This action is not part of PLUMED and was included by using a LOAD command <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></span></span> ...
 LABEL=<b name="data/iron/plumed.start.datmodel" onclick='showPath("data/iron/plumed.start.dat","data/iron/plumed.start.datmodel","data/iron/plumed.start.datmodel","brown")'>model</b>
 ATOMS=<b name="data/iron/plumed.start.datC">C</b>
 KCUT=50
 MODEL=model.pt
... GRAPH
<br/><span class="plumedtooltip" style="color:green">METAD<span class="right">Used to performed metadynamics on one or more collective variables. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_e_t_a_d.html" style="color:green">More details</a><i></i></span></span> ...
 <span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/iron/plumed.start.datmetad" onclick='showPath("data/iron/plumed.start.dat","data/iron/plumed.start.datmetad","data/iron/plumed.start.datmetad","brown")'>metad</b>
 <span class="plumedtooltip">ARG<span class="right">the labels of the scalars on which the bias will act<i></i></span></span>=model.node-0,model.node-1
 <span class="plumedtooltip">SIGMA<span class="right">the widths of the Gaussian hills<i></i></span></span>=0.6,0.6 
 <span class="plumedtooltip">HEIGHT<span class="right">the heights of the Gaussian hills<i></i></span></span>=15 <span style="color:blue" class="comment"># this is 0.5kt at 1800 K </span>
 <span class="plumedtooltip">FILE<span class="right"> a file in which the list of added hills is stored<i></i></span></span>=HILLS   <span style="color:blue" class="comment"># File where the information of the gaussians is printed</span>
 <span class="plumedtooltip">BIASFACTOR<span class="right">use well tempered metadynamics and use this bias factor<i></i></span></span>=50
 <span class="plumedtooltip">TEMP<span class="right">the system temperature - this is only needed if you are doing well-tempered metadynamics<i></i></span></span>=1800.0 
 <span class="plumedtooltip">PACE<span class="right">the frequency for hill addition<i></i></span></span>=500
 <span class="plumedtooltip">GRID_MIN<span class="right">the lower bounds for the grid<i></i></span></span>=1.0,1.0 <span class="plumedtooltip">GRID_MAX<span class="right">the upper bounds for the grid<i></i></span></span>=15.0,15.0
 <span class="plumedtooltip">CALC_RCT<span class="right"> calculate the c(t) reweighting factor and use that to obtain the normalized bias [rbias=bias-rct]<i></i></span></span>
... METAD
<br/><span style="display:none;" id="data/iron/plumed.start.datmetad">The METAD action with label <b>metad</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">metad.bias</td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">metad.rbias</td><td>the instantaneous value of the bias normalized using the c(t) reweighting factor [rbias=bias-rct]</td></tr><tr><td width="5%">metad.rct</td><td>the reweighting factor c(t)</td></tr></table></span><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=model.*,<b name="data/iron/plumed.start.datmetad">metad.*</b> <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=500 <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=COLVAR 
</pre>
{% endraw %}
