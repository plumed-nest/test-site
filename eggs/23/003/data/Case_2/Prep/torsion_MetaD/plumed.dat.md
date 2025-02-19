**Project ID:** [plumID:23.003]({{ '/' | absolute_url }}eggs/23/003/)  
**Source:** Case_2/Prep/torsion_MetaD/plumed.dat  
**Originally used with PLUMED version:** 2.8  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/Case_2/Prep/torsion_MetaD/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-passing-green.svg" alt="tested onv2.10" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<b name="data/Case_2/Prep/torsion_MetaD/plumed.dattheta" onclick='showPath("data/Case_2/Prep/torsion_MetaD/plumed.dat","data/Case_2/Prep/torsion_MetaD/plumed.dattheta","data/Case_2/Prep/torsion_MetaD/plumed.dattheta","black")'>theta</b><span style="display:none;" id="data/Case_2/Prep/torsion_MetaD/plumed.dattheta">The TORSION action with label <b>theta</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">theta</td><td width="5%"><font color="black">scalar</font></td><td>the TORSION involving these atoms</td></tr></table></span>: <span class="plumedtooltip" style="color:green">TORSION<span class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=1,2,3,4
  
<span class="plumedtooltip" style="color:green">METAD<span class="right">Used to performed metadynamics on one or more collective variables. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_e_t_a_d.html" style="color:green">More details</a><i></i></span></span> ...

<span class="plumedtooltip">ARG<span class="right">the labels of the scalars on which the bias will act<i></i></span></span>=<b name="data/Case_2/Prep/torsion_MetaD/plumed.dattheta">theta</b>
<span class="plumedtooltip">SIGMA<span class="right">the widths of the Gaussian hills<i></i></span></span>=0.5
<span class="plumedtooltip">HEIGHT<span class="right">the heights of the Gaussian hills<i></i></span></span>=2.4777090399459767     <span style="color:blue" class="comment"># kJ/mol</span>
<span class="plumedtooltip">PACE<span class="right">the frequency for hill addition<i></i></span></span>=500        <span style="color:blue" class="comment"># should be nstexpanded</span>
<span class="plumedtooltip">GRID_MIN<span class="right">the lower bounds for the grid<i></i></span></span>=-pi
<span class="plumedtooltip">GRID_MAX<span class="right">the upper bounds for the grid<i></i></span></span>=pi
<span class="plumedtooltip">GRID_BIN<span class="right">the number of bins for the grid<i></i></span></span>=100
<span class="plumedtooltip">TEMP<span class="right">the system temperature - this is only needed if you are doing well-tempered metadynamics<i></i></span></span>=298
<span class="plumedtooltip">BIASFACTOR<span class="right">use well tempered metadynamics and use this bias factor<i></i></span></span>=10
<span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/Case_2/Prep/torsion_MetaD/plumed.datmetad" onclick='showPath("data/Case_2/Prep/torsion_MetaD/plumed.dat","data/Case_2/Prep/torsion_MetaD/plumed.datmetad","data/Case_2/Prep/torsion_MetaD/plumed.datmetad","black")'>metad</b><span style="display:none;" id="data/Case_2/Prep/torsion_MetaD/plumed.datmetad">The METAD action with label <b>metad</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">metad.bias</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the bias potential</td></tr></table></span>
<span class="plumedtooltip">FILE<span class="right"> a file in which the list of added hills is stored<i></i></span></span>=HILLS
... METAD
<br/><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=10 <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=<b name="data/Case_2/Prep/torsion_MetaD/plumed.dattheta">theta</b>,<b name="data/Case_2/Prep/torsion_MetaD/plumed.datmetad">metad.bias</b> <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=COLVAR
</pre>
{% endraw %}
