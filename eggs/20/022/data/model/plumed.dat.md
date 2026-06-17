**Project ID:** [plumID:20.022]({{ '/' | absolute_url }}eggs/20/022/)  
**Source:** model/plumed.dat  
**Originally used with PLUMED version:** 2.8  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div class="plumedInputContainer">
<div class="plumedpreheader">
<div class="headerInfo" id="value_details_data/model/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div class="containerBadge">
<div class="headerBadge"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-passing-green.svg" alt="tested onv2.10" /></a></div>
<div class="headerBadge"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></div>
</div>
</div>
<pre class="plumedlisting">
<span class="plumedtooltip" style="color:blue"># vim:ft=plumed<span class="right">Enables syntax highlighting for PLUMED files in vim. See <a href="https://www.plumed.org/doc-master/user-doc/html/vim">here for more details. </a><i></i></span></span>
<br/><span style="color:blue" class="comment">#+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++#</span>
<span style="color:blue" class="comment">#                                                           #</span>
<span style="color:blue" class="comment">#  This input generates a simulation that samples the same  #</span>
<span style="color:blue" class="comment">#  distribution as 28 umbrella-sampling windows             #</span>
<span style="color:blue" class="comment">#                                                           #</span>
<span style="color:blue" class="comment">#+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++#</span>
<br/><span class="plumedtooltip" style="color:green">UNITS<span class="right">This command sets the internal units for the code. <a href="https://www.plumed.org/doc-master/user-doc/html/UNITS" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">NATURAL<span class="right"> use natural units<i></i></span></span>
<br/><span style="display:none;" id="data/model/plumed.dat">The UNITS action with label <b></b> calculates something</span><b name="data/model/plumed.datp" onclick='showPath("data/model/plumed.dat","data/model/plumed.datp","data/model/plumed.datp","brown")'>p</b>: <span class="plumedtooltip" style="color:green">POSITION<span class="right">Calculate the components of the position of an atom or atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/POSITION" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOM<span class="right">the atom number<i></i></span></span>=1

<span style="display:none;" id="data/model/plumed.datp">The POSITION action with label <b>p</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">p.x</td><td>the x-component of the atom position</td></tr><tr><td width="5%">p.y</td><td>the y-component of the atom position</td></tr><tr><td width="5%">p.z</td><td>the z-component of the atom position</td></tr></table></span><b name="data/model/plumed.datecv" onclick='showPath("data/model/plumed.dat","data/model/plumed.datecv","data/model/plumed.datecv","brown")'>ecv</b>: <span class="plumedtooltip" style="color:green">ECV_UMBRELLAS_LINE<span class="right">Target a multiumbrella ensemble, by combining systems each with a parabolic bias potential at a different location. <a href="https://www.plumed.org/doc-master/user-doc/html/ECV_UMBRELLAS_LINE" style="color:green">More details</a><i></i></span></span> ...
  <span class="plumedtooltip">ARG<span class="right">the labels of the scalar values that are input to this action<i></i></span></span>=<b name="data/model/plumed.datp">p.x</b>
  <span class="plumedtooltip">CV_MIN<span class="right">the minimum of the CV range to be explored<i></i></span></span>=-2.5
  <span class="plumedtooltip">CV_MAX<span class="right">the maximum of the CV range to be explored<i></i></span></span>=2.5
  <span class="plumedtooltip">SIGMA<span class="right">sigma of the umbrella Gaussians<i></i></span></span>=0.185815
...
<span style="display:none;" id="data/model/plumed.datecv">The ECV_UMBRELLAS_LINE action with label <b>ecv</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ecv..#!custom</td><td>the names of the output components for this action depend on the actions input file see the example inputs below for details</td></tr></table></span><b name="data/model/plumed.datopes" onclick='showPath("data/model/plumed.dat","data/model/plumed.datopes","data/model/plumed.datopes","brown")'>opes</b>: <span class="plumedtooltip" style="color:green">OPES_EXPANDED<span class="right">On-the-fly probability enhanced sampling with expanded ensembles for the target distribution. <a href="https://www.plumed.org/doc-master/user-doc/html/OPES_EXPANDED" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the label of the ECVs that define the expansion<i></i></span></span>=<b name="data/model/plumed.datecv">ecv.*</b> <span class="plumedtooltip">FILE<span class="right"> a file with the estimate of the relative Delta F for each component of the target and of the global c(t)<i></i></span></span>=DeltaFs.data <span class="plumedtooltip">PACE<span class="right">how often the bias is updated<i></i></span></span>=500

<span style="display:none;" id="data/model/plumed.datopes">The OPES_EXPANDED action with label <b>opes</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">opes.bias</td><td>the instantaneous value of the bias potential</td></tr></table></span><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/PRINT" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">FMT<span class="right"> the format that should be used to output real numbers<i></i></span></span>=%g <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=500 <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=Colvar.data <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=<b name="data/model/plumed.datp">p.x</b>,<b name="data/model/plumed.datp">p.y</b>,<b name="data/model/plumed.datopes">opes.*</b>

<span class="plumedtooltip" style="color:green">ENDPLUMED<span class="right">Terminate plumed input. <a href="https://www.plumed.org/doc-master/user-doc/html/ENDPLUMED" style="color:green">More details</a><i></i></span></span><span style="color:blue" class="comment">

will produce 10 independent run, use instead WALKERS_MPI to make multiple walkers share bias

to print the running FES with GNUPLOT:
p &#x27;&lt;awk &#x27;&#x27;END{for(i=3;i&lt;=NF;i++)print -2.5+(i-3)*5/(NF-3),$i}&#x27;&#x27; DeltaFs.0.data&#x27;w lp
</span></pre></div>

{% endraw %}
