**Project ID:** [plumID:20.022]({{ '/' | absolute_url }}eggs/20/022/)  
**Source:** water/plumed.dat  
**Originally used with PLUMED version:** 2.8  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div class="plumedInputContainer">
<div class="plumedpreheader">
<div class="headerInfo" id="value_details_data/water/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div class="containerBadge">
<div class="headerBadge"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-passing-green.svg" alt="tested onv2.10" /></a></div>
<div class="headerBadge"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></div>
<div class="headerBadge"><img src="https://img.shields.io/badge/with-LOAD-yellow.svg" alt="tested on master" /></div>
</div>
</div>
<pre class="plumedlisting">
<span class="plumedtooltip" style="color:blue"># vim:ft=plumed<span class="right">Enables syntax highlighting for PLUMED files in vim. See <a href="https://www.plumed.org/doc-master/user-doc/html/vim">here for more details. </a><i></i></span></span>
<span class="plumedtooltip" style="color:green">LOAD<span class="right">Loads a library, possibly defining new actions. <a href="https://www.plumed.org/doc-master/user-doc/html/LOAD" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">FILE<span class="right">file to be loaded<i></i></span></span>=LennardJones.cpp

<span style="color:blue" class="comment">#+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++#</span>
<span style="color:blue" class="comment">#                                                                       #</span>
<span style="color:blue" class="comment">#  This input generates a simulation that samples all the intermediate  #</span>
<span style="color:blue" class="comment">#  states needed for performing thermodynamic integration               #</span>
<span style="color:blue" class="comment">#                                                                       #</span>
<span style="color:blue" class="comment">#+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++#</span>
<br/><span style="display:none;" id="data/water/plumed.dat">The LOAD action with label <b></b> calculates something</span><b name="data/water/plumed.dateneWAT" onclick='showPath("data/water/plumed.dat","data/water/plumed.dateneWAT","data/water/plumed.dateneWAT","brown")'>eneWAT</b>: <span class="plumedtooltip" style="color:green">ENERGY<span class="right">Calculate the total potential energy of the simulation box. <a href="https://www.plumed.org/doc-master/user-doc/html/ENERGY" style="color:green">More details</a><i></i></span></span>
<span style="display:none;" id="data/water/plumed.dateneWAT">The ENERGY action with label <b>eneWAT</b> calculates something</span><span class="plumedtooltip" style="color:green">LENNARDJONES<span class="right">This action is not part of PLUMED and was included by using a LOAD command <a href="https://www.plumed.org/doc-master/user-doc/html/LOAD" style="color:green">More details</a><i></i></span></span> ...
 LABEL=<b name="data/water/plumed.dateneLJ" onclick='showPath("data/water/plumed.dat","data/water/plumed.dateneLJ","data/water/plumed.dateneLJ","brown")'>eneLJ</b>
 GROUPA=1-1152:3
 SIGMA=0.31536
 EPSILON=0.64852
 RCUT=0.85
 NLIST
 NL_CUTOFF=1.0
 NL_STRIDE=10
... LENNARDJONES
<b name="data/water/plumed.datDeltaU" onclick='showPath("data/water/plumed.dat","data/water/plumed.datDeltaU","data/water/plumed.datDeltaU","brown")'>DeltaU</b>: <span class="plumedtooltip" style="color:green">CUSTOM<span class="right">Calculate a combination of variables using a custom expression. <a href="https://www.plumed.org/doc-master/user-doc/html/CUSTOM" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the values input to this function<i></i></span></span>=eneLJ,<b name="data/water/plumed.dateneWAT">eneWAT</b> <span class="plumedtooltip">FUNC<span class="right">the function you wish to evaluate<i></i></span></span>=x-y <span class="plumedtooltip">PERIODIC<span class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></span></span>=NO

<span style="display:none;" id="data/water/plumed.datDeltaU">The CUSTOM action with label <b>DeltaU</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">DeltaU.value</td><td>an arbitrary function</td></tr></table></span><b name="data/water/plumed.datecv" onclick='showPath("data/water/plumed.dat","data/water/plumed.datecv","data/water/plumed.datecv","brown")'>ecv</b>: <span class="plumedtooltip" style="color:green">ECV_LINEAR<span class="right">Linear expansion, according to a parameter lambda. <a href="https://www.plumed.org/doc-master/user-doc/html/ECV_LINEAR" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the label of the Hamiltonian difference<i></i></span></span>=<b name="data/water/plumed.datDeltaU">DeltaU</b> <span class="plumedtooltip">TEMP<span class="right"> temperature<i></i></span></span>=443
<span style="display:none;" id="data/water/plumed.datecv">The ECV_LINEAR action with label <b>ecv</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ecv..#!custom</td><td>the names of the output components for this action depend on the actions input file see the example inputs below for details</td></tr></table></span><b name="data/water/plumed.datopes" onclick='showPath("data/water/plumed.dat","data/water/plumed.datopes","data/water/plumed.datopes","brown")'>opes</b>: <span class="plumedtooltip" style="color:green">OPES_EXPANDED<span class="right">On-the-fly probability enhanced sampling with expanded ensembles for the target distribution. <a href="https://www.plumed.org/doc-master/user-doc/html/OPES_EXPANDED" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the label of the ECVs that define the expansion<i></i></span></span>=<b name="data/water/plumed.datecv">ecv.*</b> <span class="plumedtooltip">PACE<span class="right">how often the bias is updated<i></i></span></span>=100

<span style="display:none;" id="data/water/plumed.datopes">The OPES_EXPANDED action with label <b>opes</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">opes.bias</td><td>the instantaneous value of the bias potential</td></tr></table></span><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/PRINT" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=<b name="data/water/plumed.dateneWAT">eneWAT</b>,eneLJ,<b name="data/water/plumed.datDeltaU">DeltaU</b>,<b name="data/water/plumed.datopes">opes.*</b> <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=100 <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=COLVAR

<span class="plumedtooltip" style="color:green">ENDPLUMED<span class="right">Terminate plumed input. <a href="https://www.plumed.org/doc-master/user-doc/html/ENDPLUMED" style="color:green">More details</a><i></i></span></span><span style="color:blue" class="comment">
</span></pre></div>

{% endraw %}
