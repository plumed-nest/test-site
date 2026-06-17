**Project ID:** [plumID:19.059]({{ '/' | absolute_url }}eggs/19/059/)  
**Source:** plumed.0.dat  
**Originally used with PLUMED version:** 2.2.3  
**Stable:** [zipped raw stdout](plumed.0.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.0.dat.plumed.stderr.txt.zip) - [stderr](plumed.0.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.0.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.0.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.0.dat.plumed_master.stderr)  

{% raw %}
<div class="plumedInputContainer">
<div class="plumedpreheader">
<div class="headerInfo" id="value_details_data/plumed.0.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div class="containerBadge">
<div class="headerBadge"><a href="plumed.0.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-passing-green.svg" alt="tested onv2.10" /></a></div>
<div class="headerBadge"><a href="plumed.0.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></div>
</div>
</div>
<pre class="plumedlisting">
<span style="color:blue" class="comment">#RESTART</span>
<span id="data/plumed.0.datplumed_be-common.dat_short"><span class="plumedtooltip" style="color:green">INCLUDE<span class="right">Includes an external input file, similar to #include in C preprocessor. <a href="https://www.plumed.org/doc-master/user-doc/html/INCLUDE">More details</a>. Show <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/plumed.0.datplumed_be-common.dat");'>included file</a><i></i></span></span> <span class="plumedtooltip">FILE<span class="right">file to be included<i></i></span></span>=<a class="toggler" href='javascript:;' onclick='toggleDisplay("data/plumed.0.datplumed_be-common.dat");'>plumed_be-common.dat</a>
</span><span id="data/plumed.0.datplumed_be-common.dat_long" style="display:none;"><span style="color:blue" class="comment"># The command:
</span><span class="toggler" style="color:red" onclick='toggleDisplay("data/plumed.0.datplumed_be-common.dat")'># INCLUDE FILE=plumed_be-common.dat
</span><span style="color:blue" class="comment"># ensures PLUMED loads the contents of the file called plumed_be-common.dat</span>
<span style="color:blue" class="comment"># The contents of this file are shown below (click the red comment to hide them).</span>
<span style="color:blue" class="comment">#RESTART</span>
<span style="color:blue" class="comment"># randomize the exchange (not between consecutive indeces, here just 2 replicas, so it is not relevant)</span>
<span style="display:none;" id="data/plumed.0.datplumed_be-common.dat">The INCLUDE action with label <b>plumed_be-common.dat</b> calculates something</span><span class="plumedtooltip" style="color:green">RANDOM_EXCHANGES<span class="right">Set random pattern for exchanges. <a href="https://www.plumed.org/doc-master/user-doc/html/RANDOM_EXCHANGES" style="color:green">More details</a><i></i></span></span>
<span style="color:blue" class="comment"># set up the two torsion collective variables </span>
<span style="color:blue" class="comment"># omega (use cv1 so it will be compatible with the METAGUI analysis plugin)</span>
<span style="display:none;" id="data/plumed.0.dat">The RANDOM_EXCHANGES action with label <b></b> calculates something</span><b name="data/plumed.0.datcv1" onclick='showPath("data/plumed.0.dat","data/plumed.0.datcv1","data/plumed.0.datcv1","brown")'>cv1</b>: <span class="plumedtooltip" style="color:green">TORSION<span class="right">Calculate one or multiple torsional angles. <a href="https://www.plumed.org/doc-master/user-doc/html/TORSION" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=19,40,42,45
<span style="color:blue" class="comment"># psi (use cv2 so it will be compatible with the METAGUI analysis plugin)</span>
<span style="display:none;" id="data/plumed.0.datcv1">The TORSION action with label <b>cv1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cv1.value</td><td>the TORSION involving these atoms</td></tr></table></span><b name="data/plumed.0.datcv2" onclick='showPath("data/plumed.0.dat","data/plumed.0.datcv2","data/plumed.0.datcv2","brown")'>cv2</b>: <span class="plumedtooltip" style="color:green">TORSION<span class="right">Calculate one or multiple torsional angles. <a href="https://www.plumed.org/doc-master/user-doc/html/TORSION" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=41,45,53,55

<span style="color:blue"># --- End of included input --- </span></span><br/><span style="color:blue" class="comment">#METAD activates metadynamics</span>
<span style="color:blue" class="comment">#ARG indicates variables to enhance (omega &amp; psi)</span>
<span style="color:blue" class="comment">#PACE indicates frequency of Gaussian deposition is 1000 time step (2ps)</span>
<span style="color:blue" class="comment">#HEIGHT indicates that height of the Gaussians is 0.2 kJ/mol</span>
<span style="color:blue" class="comment">#SIGMA indicates the width of the Gaussians on the biased cv, respectively</span>
<br/><span style="display:none;" id="data/plumed.0.datcv2">The TORSION action with label <b>cv2</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cv2.value</td><td>the TORSION involving these atoms</td></tr></table></span><b name="data/plumed.0.datbe" onclick='showPath("data/plumed.0.dat","data/plumed.0.datbe","data/plumed.0.datbe","brown")'>be</b>: <span class="plumedtooltip" style="color:green">METAD<span class="right">Used to performed metadynamics on one or more collective variables. <a href="https://www.plumed.org/doc-master/user-doc/html/METAD" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the labels of the scalars on which the bias will act<i></i></span></span>=<b name="data/plumed.0.datcv1">cv1</b> <span class="plumedtooltip">PACE<span class="right">the frequency for hill addition<i></i></span></span>=1000 <span class="plumedtooltip">HEIGHT<span class="right">the heights of the Gaussian hills<i></i></span></span>=0.2 <span class="plumedtooltip">SIGMA<span class="right">the widths of the Gaussian hills<i></i></span></span>=0.17

<span style="color:blue" class="comment">#print in other file the values of the CVS and the bias potential</span>
<span style="color:blue" class="comment">#STRIDE frequency of output</span>
<span style="color:blue" class="comment">#ARG things to print, omega, psi</span>
<span style="color:blue" class="comment">#FILE, name of the file to output; COLVAR</span>
<br/><span style="display:none;" id="data/plumed.0.datbe">The METAD action with label <b>be</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">be.bias</td><td>the instantaneous value of the bias potential</td></tr></table></span><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/PRINT" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=500 <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=<b name="data/plumed.0.datcv1">cv1</b>,<b name="data/plumed.0.datcv2">cv2</b> <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=COLVAR
</pre></div>

{% endraw %}
