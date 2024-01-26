**Project ID:** [plumID:23.003]({{ '/' | absolute_url }}eggs/23/003/)  
**Source:** Case_1/Test_1/1D_lambda_MetaD/rep_1/plumed.dat  
**Originally used with PLUMED version:** 2.8  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/Case_1/Test_1/1D_lambda_MetaD/rep_1/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<b name="data/Case_1/Test_1/1D_lambda_MetaD/rep_1/plumed.datlambda" onclick='showPath("data/Case_1/Test_1/1D_lambda_MetaD/rep_1/plumed.dat","data/Case_1/Test_1/1D_lambda_MetaD/rep_1/plumed.datlambda")'>lambda</b>: <div class="tooltip" style="color:green">EXTRACV<div class="right">Allow PLUMED to use collective variables computed in the MD engine. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_x_t_r_a_c_v.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">NAME<div class="right">name of the CV as computed by the MD engine<i></i></div></div>=<b name="data/Case_1/Test_1/1D_lambda_MetaD/rep_1/plumed.datlambda">lambda</b>
  
<div class="tooltip" style="color:green">METAD<div class="right">Used to performed metadynamics on one or more collective variables. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_e_t_a_d.html" style="color:green">More details</a><i></i></div></div> ...
<div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/Case_1/Test_1/1D_lambda_MetaD/rep_1/plumed.datlambda">lambda</b>
<div class="tooltip">SIGMA<div class="right">the widths of the Gaussian hills<i></i></div></div>=0.01     
<div class="tooltip">HEIGHT<div class="right">the heights of the Gaussian hills<i></i></div></div>=1.2388545199729883   
<div class="tooltip">PACE<div class="right">the frequency for hill addition<i></i></div></div>=10       
<div class="tooltip">GRID_MIN<div class="right">the lower bounds for the grid<i></i></div></div>=0    
<div class="tooltip">GRID_MAX<div class="right">the upper bounds for the grid<i></i></div></div>=5    
<div class="tooltip">GRID_BIN<div class="right">the number of bins for the grid<i></i></div></div>=5    
<div class="tooltip">TEMP<div class="right">the system temperature - this is only needed if you are doing well-tempered metadynamics<i></i></div></div>=298     
<div class="tooltip">BIASFACTOR<div class="right">use well tempered metadynamics and use this bias factor<i></i></div></div>=50   
<div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/Case_1/Test_1/1D_lambda_MetaD/rep_1/plumed.datmetad" onclick='showPath("data/Case_1/Test_1/1D_lambda_MetaD/rep_1/plumed.dat","data/Case_1/Test_1/1D_lambda_MetaD/rep_1/plumed.datmetad")'>metad</b>   
<div class="tooltip">FILE<div class="right"> a file in which the list of added hills is stored<i></i></div></div>=HILLS_LAMBDA
... METAD
<br/><span style="display:none;" id="data/Case_1/Test_1/1D_lambda_MetaD/rep_1/plumed.datmetad">The METAD action with label <b>metad</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">metad.bias</td><td>the instantaneous value of the bias potential</td></tr></table></span><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=10 <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/Case_1/Test_1/1D_lambda_MetaD/rep_1/plumed.datlambda">lambda</b>,<b name="data/Case_1/Test_1/1D_lambda_MetaD/rep_1/plumed.datmetad">metad.bias</b> <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=COLVAR
</pre>
{% endraw %}
