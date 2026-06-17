**Project ID:** [plumID:19.067]({{ '/' | absolute_url }}eggs/19/067/)  
**Source:** ache-pws/plumed-unbiased.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [zipped raw stdout](plumed-unbiased.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed-unbiased.dat.plumed.stderr.txt.zip) - [stderr](plumed-unbiased.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed-unbiased.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed-unbiased.dat.plumed_master.stderr.txt.zip) - [stderr](plumed-unbiased.dat.plumed_master.stderr)  

{% raw %}
<div class="plumedInputContainer">
<div class="plumedpreheader">
<div class="headerInfo" id="value_details_data/ache-pws/plumed-unbiased.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div class="containerBadge">
<div class="headerBadge"><a href="plumed-unbiased.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-passing-green.svg" alt="tested onv2.10" /></a></div>
<div class="headerBadge"><a href="plumed-unbiased.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></div>
</div>
</div>
<pre class="plumedlisting">
<span class="plumedtooltip" style="color:green">UNITS<span class="right">This command sets the internal units for the code. <a href="https://www.plumed.org/doc-master/user-doc/html/UNITS" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">LENGTH<span class="right">the units of lengths<i></i></span></span>=nm <span class="plumedtooltip">TIME<span class="right">the units of time<i></i></span></span>=ps <span class="plumedtooltip">ENERGY<span class="right">the units of energy<i></i></span></span>=kcal/mol

<span style="display:none;" id="data/ache-pws/plumed-unbiased.dat">The UNITS action with label <b></b> calculates something</span><b name="data/ache-pws/plumed-unbiased.datpws" onclick='showPath("data/ache-pws/plumed-unbiased.dat","data/ache-pws/plumed-unbiased.datpws","data/ache-pws/plumed-unbiased.datpws","brown")'>pws</b>: <span class="plumedtooltip" style="color:green">PATHMSD<span class="right">This Colvar calculates path collective variables. <a href="https://www.plumed.org/doc-master/user-doc/html/PATHMSD" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">REFERENCE<span class="right">the pdb is needed to provide the various milestones<i></i></span></span>=pws.pdb <span class="plumedtooltip">LAMBDA<span class="right">the lambda parameter is needed for smoothing, is in the units of plumed<i></i></span></span>=62

<span style="display:none;" id="data/ache-pws/plumed-unbiased.datpws">The PATHMSD action with label <b>pws</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">pws.sss</td><td>the position on the path</td></tr><tr><td width="5%">pws.zzz</td><td>the distance from the path</td></tr></table></span><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/PRINT" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=* <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=10 <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=colvar_pws <span class="plumedtooltip">FMT<span class="right"> the format that should be used to output real numbers<i></i></span></span>=%12.8f
</pre></div>

{% endraw %}
