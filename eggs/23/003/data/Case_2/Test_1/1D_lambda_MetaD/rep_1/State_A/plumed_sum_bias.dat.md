**Project ID:** [plumID:23.003]({{ '/' | absolute_url }}eggs/23/003/)  
**Source:** Case_2/Test_1/1D_lambda_MetaD/rep_1/State_A/plumed_sum_bias.dat  
**Originally used with PLUMED version:** 2.8  
**Stable:** [zipped raw stdout](plumed_sum_bias.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_sum_bias.dat.plumed.stderr.txt.zip) - [stderr](plumed_sum_bias.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed_sum_bias.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_sum_bias.dat.plumed_master.stderr.txt.zip) - [stderr](plumed_sum_bias.dat.plumed_master.stderr)  

{% raw %}
<div class="plumedInputContainer">
<div class="plumedpreheader">
<div class="headerInfo" id="value_details_data/Case_2/Test_1/1D_lambda_MetaD/rep_1/State_A/plumed_sum_bias.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div class="containerBadge">
<div class="headerBadge"><a href="plumed_sum_bias.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-passing-green.svg" alt="tested onv2.10" /></a></div>
<div class="headerBadge"><a href="plumed_sum_bias.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></div>
</div>
</div>
<pre class="plumedlisting">
<b name="data/Case_2/Test_1/1D_lambda_MetaD/rep_1/State_A/plumed_sum_bias.datlambda" onclick='showPath("data/Case_2/Test_1/1D_lambda_MetaD/rep_1/State_A/plumed_sum_bias.dat","data/Case_2/Test_1/1D_lambda_MetaD/rep_1/State_A/plumed_sum_bias.datlambda","data/Case_2/Test_1/1D_lambda_MetaD/rep_1/State_A/plumed_sum_bias.datlambda","brown")'>lambda</b>: <span class="plumedtooltip" style="color:green">READ<span class="right">Read quantities from a colvar file. <a href="https://www.plumed.org/doc-master/user-doc/html/READ" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">FILE<span class="right">the name of the file from which to read these quantities<i></i></span></span>=COLVAR_fake <span class="plumedtooltip">VALUES<span class="right">the values to read from the file<i></i></span></span>=lambda <span class="plumedtooltip">IGNORE_TIME<span class="right"> ignore the time in the colvar file<i></i></span></span> <span class="plumedtooltip">IGNORE_FORCES<span class="right"> use this flag if the forces added by any bias can be safely ignored<i></i></span></span>
<br/><span style="display:none;" id="data/Case_2/Test_1/1D_lambda_MetaD/rep_1/State_A/plumed_sum_bias.datlambda">The READ action with label <b>lambda</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">lambda..#!custom</td><td>the names of the output components for this action depend on the actions input file see the example inputs below for details</td></tr></table></span><span class="plumedtooltip" style="color:green">METAD<span class="right">Used to performed metadynamics on one or more collective variables. <a href="https://www.plumed.org/doc-master/user-doc/html/METAD" style="color:green">More details</a><i></i></span></span> ...
<span class="plumedtooltip">ARG<span class="right">the labels of the scalars on which the bias will act<i></i></span></span>=<b name="data/Case_2/Test_1/1D_lambda_MetaD/rep_1/State_A/plumed_sum_bias.datlambda">lambda</b> 
<span class="plumedtooltip">SIGMA<span class="right">the widths of the Gaussian hills<i></i></span></span>=0.01     
<span class="plumedtooltip">HEIGHT<span class="right">the heights of the Gaussian hills<i></i></span></span>=0
<span class="plumedtooltip">PACE<span class="right">the frequency for hill addition<i></i></span></span>=5000000        
<span class="plumedtooltip">GRID_MIN<span class="right">the lower bounds for the grid<i></i></span></span>=0   
<span class="plumedtooltip">GRID_MAX<span class="right">the upper bounds for the grid<i></i></span></span>=19   
<span class="plumedtooltip">GRID_BIN<span class="right">the number of bins for the grid<i></i></span></span>=19
<span class="plumedtooltip">TEMP<span class="right">the system temperature - this is only needed if you are doing well-tempered metadynamics<i></i></span></span>=298
<span class="plumedtooltip">BIASFACTOR<span class="right">use well tempered metadynamics and use this bias factor<i></i></span></span>=60
<span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/Case_2/Test_1/1D_lambda_MetaD/rep_1/State_A/plumed_sum_bias.datmetad" onclick='showPath("data/Case_2/Test_1/1D_lambda_MetaD/rep_1/State_A/plumed_sum_bias.dat","data/Case_2/Test_1/1D_lambda_MetaD/rep_1/State_A/plumed_sum_bias.datmetad","data/Case_2/Test_1/1D_lambda_MetaD/rep_1/State_A/plumed_sum_bias.datmetad","brown")'>metad</b>    
<span class="plumedtooltip">FILE<span class="right"> a file in which the list of added hills is stored<i></i></span></span>=HILLS_1D_modified_fake
<span class="plumedtooltip">RESTART<span class="right">allows per-action setting of restart (YES/NO/AUTO)<i></i></span></span>=YES
... METAD
<br/><span style="display:none;" id="data/Case_2/Test_1/1D_lambda_MetaD/rep_1/State_A/plumed_sum_bias.datmetad">The METAD action with label <b>metad</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">metad.bias</td><td>the instantaneous value of the bias potential</td></tr></table></span><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/PRINT" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=1 <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=<b name="data/Case_2/Test_1/1D_lambda_MetaD/rep_1/State_A/plumed_sum_bias.datlambda">lambda</b>,<b name="data/Case_2/Test_1/1D_lambda_MetaD/rep_1/State_A/plumed_sum_bias.datmetad">metad.bias</b> <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=COLVAR_SUM_BIAS
</pre></div>

{% endraw %}
