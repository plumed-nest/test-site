**Project ID:** [plumID:19.071]({{ '/' | absolute_url }}eggs/19/071/)  
**Source:** MFI_paper_scripts/reweighting/plumed_FB.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [zipped raw stdout](plumed_FB.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_FB.dat.plumed.stderr.txt.zip) - [stderr](plumed_FB.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed_FB.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_FB.dat.plumed_master.stderr.txt.zip) - [stderr](plumed_FB.dat.plumed_master.stderr)  

{% raw %}
<div class="plumedInputContainer">
<div class="plumedpreheader">
<div class="headerInfo" id="value_details_data/MFI_paper_scripts/reweighting/plumed_FB.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div class="containerBadge">
<div class="headerBadge"><a href="plumed_FB.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-passing-green.svg" alt="tested onv2.10" /></a></div>
<div class="headerBadge"><a href="plumed_FB.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></div>
</div>
</div>
<pre class="plumedlisting">
<b name="data/MFI_paper_scripts/reweighting/plumed_FB.datp" onclick='showPath("data/MFI_paper_scripts/reweighting/plumed_FB.dat","data/MFI_paper_scripts/reweighting/plumed_FB.datp","data/MFI_paper_scripts/reweighting/plumed_FB.datp","brown")'>p</b>: <span class="plumedtooltip" style="color:green">READ<span class="right">Read quantities from a colvar file. <a href="https://www.plumed.org/doc-master/user-doc/html/READ" style="color:green">More details</a><i></i></span></span>  <span class="plumedtooltip">FILE<span class="right">the name of the file from which to read these quantities<i></i></span></span>=./position  <span class="plumedtooltip">VALUES<span class="right">the values to read from the file<i></i></span></span>=p.x <span class="plumedtooltip">IGNORE_FORCES<span class="right"> use this flag if the forces added by any bias can be safely ignored<i></i></span></span> <span class="plumedtooltip">IGNORE_TIME<span class="right"> ignore the time in the colvar file<i></i></span></span>
<br/><span style="display:none;" id="data/MFI_paper_scripts/reweighting/plumed_FB.datp">The READ action with label <b>p</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">p..#!custom</td><td>the names of the output components for this action depend on the actions input file see the example inputs below for details</td></tr></table></span><span class="plumedtooltip" style="color:green">METAD<span class="right">Used to performed metadynamics on one or more collective variables. <a href="https://www.plumed.org/doc-master/user-doc/html/METAD" style="color:green">More details</a><i></i></span></span> ... 
<span class="plumedtooltip">ARG<span class="right">the labels of the scalars on which the bias will act<i></i></span></span>=<b name="data/MFI_paper_scripts/reweighting/plumed_FB.datp">p.x</b>
<span class="plumedtooltip">SIGMA<span class="right">the widths of the Gaussian hills<i></i></span></span>=0.05 
<span class="plumedtooltip">HEIGHT<span class="right">the heights of the Gaussian hills<i></i></span></span>=0.1 
<span class="plumedtooltip">PACE<span class="right">the frequency for hill addition<i></i></span></span>=500 
<span class="plumedtooltip">BIASFACTOR<span class="right">use well tempered metadynamics and use this bias factor<i></i></span></span>=5 
<span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/MFI_paper_scripts/reweighting/plumed_FB.datmetad" onclick='showPath("data/MFI_paper_scripts/reweighting/plumed_FB.dat","data/MFI_paper_scripts/reweighting/plumed_FB.datmetad","data/MFI_paper_scripts/reweighting/plumed_FB.datmetad","brown")'>metad</b> 
<span class="plumedtooltip">TEMP<span class="right">the system temperature - this is only needed if you are doing well-tempered metadynamics<i></i></span></span>=120
<span class="plumedtooltip">GRID_MIN<span class="right">the lower bounds for the grid<i></i></span></span>=-2.7
<span class="plumedtooltip">GRID_MAX<span class="right">the upper bounds for the grid<i></i></span></span>=2.7
<span class="plumedtooltip">GRID_BIN<span class="right">the number of bins for the grid<i></i></span></span>=500
<span class="plumedtooltip">GRID_WSTRIDE<span class="right">write the grid to a file every N steps<i></i></span></span>=100000
<span class="plumedtooltip">GRID_WFILE<span class="right">the file on which to write the grid<i></i></span></span>=grid.dat
... METAD
<span style="display:none;" id="data/MFI_paper_scripts/reweighting/plumed_FB.datmetad">The METAD action with label <b>metad</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">metad.bias</td><td>the instantaneous value of the bias potential</td></tr></table></span></pre></div>

{% endraw %}
