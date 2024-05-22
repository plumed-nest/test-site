**Project ID:** [plumID:24.004]({{ '/' | absolute_url }}eggs/24/004/)  
**Source:** iron/plumed.start.dat  
**Originally used with PLUMED version:** 2.8.1  
**Stable:** [zipped raw stdout](plumed.start.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.start.dat.plumed.stderr.txt.zip) - [stderr](plumed.start.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.start.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.start.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.start.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/iron/plumed.start.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.start.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.start.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-failed-red.svg" alt="tested onmaster" /></a></td></tr><tr><td style="padding:1px"><img src="https://img.shields.io/badge/with-LOAD-yellow.svg" alt="tested on master" /></td></tr>
</table></div></div>
<pre style="width=97%;">
<div class="tooltip" style="color:green">LOAD<div class="right">Loads a library, possibly defining new actions. <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">FILE<div class="right">file to be loaded<i></i></div></div>=Graph.cpp
<br/><span style="color:blue" class="comment"># Define groups for the CV</span>
<span style="display:none;" id="data/iron/plumed.start.dat">The LOAD action with label <b></b> calculates something</span><b name="data/iron/plumed.start.datC" onclick='showPath("data/iron/plumed.start.dat","data/iron/plumed.start.datC","data/iron/plumed.start.datC","brown")'>C</b>: <div class="tooltip" style="color:green">GROUP<div class="right">Define a group of atoms so that a particular list of atoms can be referenced with a single label in definitions of CVs or virtual atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_g_r_o_u_p.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the numerical indexes for the set of atoms in the group<i></i></div></div>=1-285
 
<span style="color:blue" class="comment"># Define the CV</span>
<span style="display:none;" id="data/iron/plumed.start.datC">The GROUP action with label <b>C</b> calculates something</span><div class="tooltip" style="color:green">GRAPH<div class="right">This action is not part of PLUMED and was included by using a LOAD command <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></div></div> ...
 LABEL=<b name="data/iron/plumed.start.datmodel" onclick='showPath("data/iron/plumed.start.dat","data/iron/plumed.start.datmodel","data/iron/plumed.start.datmodel","brown")'>model</b>
 ATOMS=<b name="data/iron/plumed.start.datC">C</b>
 KCUT=50
 MODEL=model.pt
... GRAPH
<br/><div class="tooltip" style="color:green">METAD<div class="right">Used to performed metadynamics on one or more collective variables. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_e_t_a_d.html" style="color:green">More details</a><i></i></div></div> ...
 <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/iron/plumed.start.datmetad" onclick='showPath("data/iron/plumed.start.dat","data/iron/plumed.start.datmetad","data/iron/plumed.start.datmetad","brown")'>metad</b>
 <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=model.node-0,model.node-1
 <div class="tooltip">SIGMA<div class="right">the widths of the Gaussian hills<i></i></div></div>=0.6,0.6 
 <div class="tooltip">HEIGHT<div class="right">the heights of the Gaussian hills<i></i></div></div>=15 <span style="color:blue" class="comment"># this is 0.5kt at 1800 K </span>
 <div class="tooltip">FILE<div class="right"> a file in which the list of added hills is stored<i></i></div></div>=HILLS   <span style="color:blue" class="comment"># File where the information of the gaussians is printed</span>
 <div class="tooltip">BIASFACTOR<div class="right">use well tempered metadynamics and use this bias factor<i></i></div></div>=50
 <div class="tooltip">TEMP<div class="right">the system temperature - this is only needed if you are doing well-tempered metadynamics<i></i></div></div>=1800.0 
 <div class="tooltip">PACE<div class="right">the frequency for hill addition<i></i></div></div>=500
 <div class="tooltip">GRID_MIN<div class="right">the lower bounds for the grid<i></i></div></div>=1.0,1.0 <div class="tooltip">GRID_MAX<div class="right">the upper bounds for the grid<i></i></div></div>=15.0,15.0
 <div class="tooltip">CALC_RCT<div class="right"> calculate the c(t) reweighting factor and use that to obtain the normalized bias [rbias=bias-rct]<i></i></div></div>
... METAD
<br/><span style="display:none;" id="data/iron/plumed.start.datmetad">The METAD action with label <b>metad</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">metad.bias</td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">metad.rbias</td><td>the instantaneous value of the bias normalized using the c(t) reweighting factor [rbias=bias-rct]</td></tr><tr><td width="5%">metad.rct</td><td>the reweighting factor c(t)</td></tr></table></span><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=model.*,<b name="data/iron/plumed.start.datmetad">metad</b> <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=500 <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=COLVAR 
</pre>
{% endraw %}
