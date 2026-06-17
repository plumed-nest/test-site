**Project ID:** [plumID:24.013]({{ '/' | absolute_url }}eggs/24/013/)  
**Source:** plumed_Argon_forward.dat  
**Originally used with PLUMED version:** 2.9  
**Stable:** [zipped raw stdout](plumed_Argon_forward.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_Argon_forward.dat.plumed.stderr.txt.zip) - [stderr](plumed_Argon_forward.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed_Argon_forward.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_Argon_forward.dat.plumed_master.stderr.txt.zip) - [stderr](plumed_Argon_forward.dat.plumed_master.stderr)  

{% raw %}
<div class="plumedInputContainer">
<div class="plumedpreheader">
<div class="headerInfo" id="value_details_data/plumed_Argon_forward.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div class="containerBadge">
<div class="headerBadge"><a href="plumed_Argon_forward.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-failed-red.svg" alt="tested onv2.10" /></a></div>
<div class="headerBadge"><a href="plumed_Argon_forward.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-failed-red.svg" alt="tested onmaster" /></a></div>
</div>
</div>
<pre class="plumedlisting">
<span style="color:blue" class="comment">#DEBUG</span>
<span class="plumedtooltip" style="color:green">RESTART<span class="right">Activate restart. <a href="https://www.plumed.org/doc-master/user-doc/html/RESTART" style="color:green">More details</a><i></i></span></span>
<span style="display:none;" id="data/plumed_Argon_forward.dat">The RESTART action with label <b></b> calculates something</span><span class="plumedtooltip" style="color:green">ENERGY<span class="right">Calculate the total potential energy of the simulation box. <a href="https://www.plumed.org/doc-master/user-doc/html/ENERGY" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/plumed_Argon_forward.datene" onclick='showPath("data/plumed_Argon_forward.dat","data/plumed_Argon_forward.datene","data/plumed_Argon_forward.datene","brown")'>ene</b>
<br/><span style="display:none;" id="data/plumed_Argon_forward.datene">The ENERGY action with label <b>ene</b> calculates something</span><span class="plumedtooltip" style="color:green">COORDINATIONNUMBER<span class="right">Calculate the coordination numbers of atoms so that you can then calculate functions of the distribution of <a href="https://www.plumed.org/doc-master/user-doc/html/COORDINATIONNUMBER" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/plumed_Argon_forward.datcoord" onclick='showPath("data/plumed_Argon_forward.dat","data/plumed_Argon_forward.datcoord","data/plumed_Argon_forward.datcoord","brown")'>coord</b> <span class="plumedtooltip">SPECIES<span class="right">the list of atoms for which the symmetry function is being calculated and the atoms that can be in the environments<i></i></span></span>=1-512 <span class="plumedtooltip">SWITCH<span class="right">the switching function that it used in the construction of the contact matrix. Options for this keyword are explained in the documentation for <a href="https://www.plumed.org/doc-master/user-doc/html/LESS_THAN">LESS_THAN</a>.<i></i></span></span>={RATIONAL R_0=0.5 D_MAX=0.55} <span class="plumedtooltip">MORE_THAN<span class="right">calculate the number of variables that are more than a certain target value. Options for this keyword are explained in the documentation for <a href="https://www.plumed.org/doc-master/user-doc/html/MORE_THAN">MORE_THAN</a>.<i></i></span></span>
RATIONAL <span class="plumedtooltip">R_0<span class="right">The r_0 parameter of the switching function<i></i></span></span>=5.0 D_MAX=10.0} TOL=0.001 

<span style="display:none;" id="data/plumed_Argon_forward.datcoord">The COORDINATIONNUMBER action with label <b>coord</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">coord.morethan</td><td>the number of colvars that have a value more than a threshold</td></tr><tr><td width="5%">coord.value</td><td>the coordination numbers of the specified atoms</td></tr></table></span><span class="plumedtooltip" style="color:green">METAD<span class="right">Used to performed metadynamics on one or more collective variables. <a href="https://www.plumed.org/doc-master/user-doc/html/METAD" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the labels of the scalars on which the bias will act<i></i></span></span>=<b name="data/plumed_Argon_forward.datcoord">coord.morethan</b> <span class="plumedtooltip">SIGMA<span class="right">the widths of the Gaussian hills<i></i></span></span>=0.25 <span class="plumedtooltip">HEIGHT<span class="right">the heights of the Gaussian hills<i></i></span></span>=0.005 <span class="plumedtooltip">PACE<span class="right">the frequency for hill addition<i></i></span></span>=5000 <span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/plumed_Argon_forward.datmeta" onclick='showPath("data/plumed_Argon_forward.dat","data/plumed_Argon_forward.datmeta","data/plumed_Argon_forward.datmeta","brown")'>meta</b> <span class="plumedtooltip">TEMP<span class="right">the system temperature - this is only needed if you are doing well-tempered metadynamics<i></i></span></span>=72.017 <span class="plumedtooltip">BIASFACTOR<span class="right">use well tempered metadynamics and use this bias factor<i></i></span></span>
5 
<br/><span style="display:none;" id="data/plumed_Argon_forward.datmeta">The METAD action with label <b>meta</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">meta.bias</td><td>the instantaneous value of the bias potential</td></tr></table></span><span class="plumedtooltip" style="color:green">COMMITTOR<span class="right">Does a committor analysis. <a href="https://www.plumed.org/doc-master/user-doc/html/COMMITTOR" style="color:green">More details</a><i></i></span></span> ...
  <span class="plumedtooltip">ARG<span class="right">the labels of the values which is being used to define the committor surface<i></i></span></span>=<b name="data/plumed_Argon_forward.datcoord">coord.morethan</b>
  <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the CVs are analyzed<i></i></span></span>=10
  BASIN_A_LOWER=200 
  BASIN_A_UPPER=512 
  BASIN_B_LOWER=140
  BASIN_B_UPPER=512
... COMMITTOR

<br/><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/PRINT" style="color:green">More details</a><i></i></span></span> ...
 <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=<b name="data/plumed_Argon_forward.datcoord">coord.morethan</b>,<b name="data/plumed_Argon_forward.datene">ene</b>,<b name="data/plumed_Argon_forward.datmeta">meta.bias</b>
 <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=100
 <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=COLVAR.data
... PRINT
</pre></div>

{% endraw %}
