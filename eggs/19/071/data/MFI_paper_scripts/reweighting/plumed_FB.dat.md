**Project ID:** [plumID:19.071]({{ '/' | absolute_url }}eggs/19/071/)  
**Source:** MFI_paper_scripts/reweighting/plumed_FB.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [zipped raw stdout](plumed_FB.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_FB.dat.plumed.stderr.txt.zip) - [stderr](plumed_FB.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed_FB.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_FB.dat.plumed_master.stderr.txt.zip) - [stderr](plumed_FB.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/MFI_paper_scripts/reweighting/plumed_FB.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed_FB.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed_FB.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span id="data/MFI_paper_scripts/reweighting/plumed_FB.datdefp_short"><b name="data/MFI_paper_scripts/reweighting/plumed_FB.datp" onclick='showPath("data/MFI_paper_scripts/reweighting/plumed_FB.dat","data/MFI_paper_scripts/reweighting/plumed_FB.datp","data/MFI_paper_scripts/reweighting/plumed_FB.datp","black")'>p</b><span style="display:none;" id="data/MFI_paper_scripts/reweighting/plumed_FB.datp">The READ action with label <b>p</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">p.x</td><td width="5%"><font color="black">scalar</font></td><td>values from the column labelled p.x in the file named ./position</td></tr></table></span>: <div class="tooltip" style="color:green">READ<div class="right">Read quantities from a colvar file. This action has <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/MFI_paper_scripts/reweighting/plumed_FB.datdefp");'>hidden defaults</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_r_e_a_d.html">More details</a><i></i></div></div>  <div class="tooltip">FILE<div class="right">the name of the file from which to read these quantities<i></i></div></div>=./position  <div class="tooltip">VALUES<div class="right">the values to read from the file<i></i></div></div>=<b name="data/MFI_paper_scripts/reweighting/plumed_FB.datp">p.x</b> <div class="tooltip">IGNORE_FORCES<div class="right"> use this flag if the forces added by any bias can be safely ignored<i></i></div></div> <div class="tooltip">IGNORE_TIME<div class="right"> ignore the time in the colvar file<i></i></div></div>
</span><span id="data/MFI_paper_scripts/reweighting/plumed_FB.datdefp_long" style="display:none;"><b name="data/MFI_paper_scripts/reweighting/plumed_FB.datp" onclick='showPath("data/MFI_paper_scripts/reweighting/plumed_FB.dat","data/MFI_paper_scripts/reweighting/plumed_FB.datp","data/MFI_paper_scripts/reweighting/plumed_FB.datp","black")'>p</b>: <div class="tooltip" style="color:green">READ<div class="right">Read quantities from a colvar file. This action uses the <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/MFI_paper_scripts/reweighting/plumed_FB.datdefp");'>defaults shown here</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_r_e_a_d.html">More details</a><i></i></div></div>  <div class="tooltip">FILE<div class="right">the name of the file from which to read these quantities<i></i></div></div>=./position  <div class="tooltip">VALUES<div class="right">the values to read from the file<i></i></div></div>=<b name="data/MFI_paper_scripts/reweighting/plumed_FB.datp">p.x</b> <div class="tooltip">IGNORE_FORCES<div class="right"> use this flag if the forces added by any bias can be safely ignored<i></i></div></div> <div class="tooltip">IGNORE_TIME<div class="right"> ignore the time in the colvar file<i></i></div></div>  <div class="tooltip">STRIDE<div class="right"> the frequency with which the file should be read<i></i></div></div>=1 <div class="tooltip">EVERY<div class="right"> only read every nth line of the colvar file<i></i></div></div>=1
</span><br/><span id="data/MFI_paper_scripts/reweighting/plumed_FB.datdefmetad_short"><div class="tooltip" style="color:green">METAD<div class="right">Used to performed metadynamics on one or more collective variables. This action has <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/MFI_paper_scripts/reweighting/plumed_FB.datdefmetad");'>hidden defaults</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_e_t_a_d.html">More details</a><i></i></div></div> ... 
<div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/MFI_paper_scripts/reweighting/plumed_FB.datp">p.x</b>
<div class="tooltip">SIGMA<div class="right">the widths of the Gaussian hills<i></i></div></div>=0.05 
<div class="tooltip">HEIGHT<div class="right">the heights of the Gaussian hills<i></i></div></div>=0.1 
<div class="tooltip">PACE<div class="right">the frequency for hill addition<i></i></div></div>=500 
<div class="tooltip">BIASFACTOR<div class="right">use well tempered metadynamics and use this bias factor<i></i></div></div>=5 
<div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/MFI_paper_scripts/reweighting/plumed_FB.datmetad" onclick='showPath("data/MFI_paper_scripts/reweighting/plumed_FB.dat","data/MFI_paper_scripts/reweighting/plumed_FB.datmetad","data/MFI_paper_scripts/reweighting/plumed_FB.datmetad","black")'>metad</b><span style="display:none;" id="data/MFI_paper_scripts/reweighting/plumed_FB.datmetad">The METAD action with label <b>metad</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">metad.bias</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the bias potential</td></tr></table></span> 
<div class="tooltip">TEMP<div class="right">the system temperature - this is only needed if you are doing well-tempered metadynamics<i></i></div></div>=120
<div class="tooltip">GRID_MIN<div class="right">the lower bounds for the grid<i></i></div></div>=-2.7
<div class="tooltip">GRID_MAX<div class="right">the upper bounds for the grid<i></i></div></div>=2.7
<div class="tooltip">GRID_BIN<div class="right">the number of bins for the grid<i></i></div></div>=500
<div class="tooltip">GRID_WSTRIDE<div class="right">write the grid to a file every N steps<i></i></div></div>=100000
<div class="tooltip">GRID_WFILE<div class="right">the file on which to write the grid<i></i></div></div>=grid.dat
... METAD
</span><span id="data/MFI_paper_scripts/reweighting/plumed_FB.datdefmetad_long" style="display:none;"><div class="tooltip" style="color:green">METAD<div class="right">Used to performed metadynamics on one or more collective variables. This action uses the <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/MFI_paper_scripts/reweighting/plumed_FB.datdefmetad");'>defaults shown here</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_e_t_a_d.html">More details</a><i></i></div></div> ... 
<div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/MFI_paper_scripts/reweighting/plumed_FB.datp">p.x</b>
<div class="tooltip">SIGMA<div class="right">the widths of the Gaussian hills<i></i></div></div>=0.05 
<div class="tooltip">HEIGHT<div class="right">the heights of the Gaussian hills<i></i></div></div>=0.1 
<div class="tooltip">PACE<div class="right">the frequency for hill addition<i></i></div></div>=500 
<div class="tooltip">BIASFACTOR<div class="right">use well tempered metadynamics and use this bias factor<i></i></div></div>=5 
<div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/MFI_paper_scripts/reweighting/plumed_FB.datmetad" onclick='showPath("data/MFI_paper_scripts/reweighting/plumed_FB.dat","data/MFI_paper_scripts/reweighting/plumed_FB.datmetad","data/MFI_paper_scripts/reweighting/plumed_FB.datmetad","black")'>metad</b> 
<div class="tooltip">TEMP<div class="right">the system temperature - this is only needed if you are doing well-tempered metadynamics<i></i></div></div>=120
<div class="tooltip">GRID_MIN<div class="right">the lower bounds for the grid<i></i></div></div>=-2.7
<div class="tooltip">GRID_MAX<div class="right">the upper bounds for the grid<i></i></div></div>=2.7
<div class="tooltip">GRID_BIN<div class="right">the number of bins for the grid<i></i></div></div>=500
<div class="tooltip">GRID_WSTRIDE<div class="right">write the grid to a file every N steps<i></i></div></div>=100000
<div class="tooltip">GRID_WFILE<div class="right">the file on which to write the grid<i></i></div></div>=grid.dat
 <div class="tooltip">FILE<div class="right"> a file in which the list of added hills is stored<i></i></div></div>=HILLS
... METAD
</span></pre>
{% endraw %}