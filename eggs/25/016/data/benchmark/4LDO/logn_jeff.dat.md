**Project ID:** [plumID:25.016]({{ '/' | absolute_url }}eggs/25/016/)  
**Source:** ./benchmark/4LDO/logn_jeff.dat  
**Originally used with PLUMED version:** 2.11  
**Stable:** [zipped raw stdout](logn_jeff.dat.plumed.stdout.txt.zip) - [zipped raw stderr](logn_jeff.dat.plumed.stderr.txt.zip) - [stderr](logn_jeff.dat.plumed.stderr)  
**Master:** [zipped raw stdout](logn_jeff.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](logn_jeff.dat.plumed_master.stderr.txt.zip) - [stderr](logn_jeff.dat.plumed_master.stderr)  

{% raw %}
<div class="plumedInputContainer">
<div class="plumedpreheader">
<div class="headerInfo" id="value_details_data/./benchmark/4LDO/logn_jeff.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div class="containerBadge">
<div class="headerBadge"><a href="logn_jeff.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-failed-red.svg" alt="tested onv2.10" /></a></div>
<div class="headerBadge"><a href="logn_jeff.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></div>
</div>
</div>
<pre class="plumedlisting">
<span style="color:blue" class="comment">#generate plumed action file</span>
<span style="color:blue" class="comment">####</span>
<span style="color:blue" class="comment"># read index file in GROMACS format</span>
<b name="data/./benchmark/4LDO/logn_jeff.datbatoms" onclick='showPath("data/./benchmark/4LDO/logn_jeff.dat","data/./benchmark/4LDO/logn_jeff.datbatoms","data/./benchmark/4LDO/logn_jeff.datbatoms","brown")'>batoms</b>: <span class="plumedtooltip" style="color:green">GROUP<span class="right">Define a group of atoms so that a particular list of atoms can be referenced with a single label in definitions of CVs or virtual atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/GROUP" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">NDX_FILE<span class="right">the name of index file (gromacs syntax)<i></i></span></span>=index.ndx <span class="plumedtooltip">NDX_GROUP<span class="right">the name of the group to be imported (gromacs syntax) - first group found is used by default<i></i></span></span>=batoms

<span style="color:blue" class="comment"># define action</span>
<span style="display:none;" id="data/./benchmark/4LDO/logn_jeff.datbatoms">The GROUP action with label <b>batoms</b> calculates something</span><b name="data/./benchmark/4LDO/logn_jeff.datbaies" onclick='showPath("data/./benchmark/4LDO/logn_jeff.dat","data/./benchmark/4LDO/logn_jeff.datbaies","data/./benchmark/4LDO/logn_jeff.datbaies","brown")'>baies</b>:   <span class="plumedtooltip" style="color:green">BAIES<span class="right">Bayesian refinement of AF models. <a href="https://www.plumed.org/doc-master/user-doc/html/BAIES" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS<span class="right">atoms used in the calculation of bAIes energy<i></i></span></span>=<b name="data/./benchmark/4LDO/logn_jeff.datbatoms">batoms</b> <span class="plumedtooltip">DATA_FILE<span class="right">file with AF2 fit parameters<i></i></span></span>=logn.out <span class="plumedtooltip">PRIOR<span class="right">type of prior to use (NONE, JEFFREYS, CAUCHY<i></i></span></span>=JEFFREYS <span class="plumedtooltip">TEMP<span class="right">temperature in kBt units<i></i></span></span>=2.478541306

<span style="display:none;" id="data/./benchmark/4LDO/logn_jeff.datbaies">The BAIES action with label <b>baies</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">baies.ene</td><td>Bayesian bAIes energy</td></tr></table></span><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/PRINT" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=<b name="data/./benchmark/4LDO/logn_jeff.datbaies">baies.ene</b> <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=COLVAR <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=500

<span style="display:none;" id="data/./benchmark/4LDO/logn_jeff.dat">The PRINT action with label <b></b> calculates something</span><b name="data/./benchmark/4LDO/logn_jeff.datbbias" onclick='showPath("data/./benchmark/4LDO/logn_jeff.dat","data/./benchmark/4LDO/logn_jeff.datbbias","data/./benchmark/4LDO/logn_jeff.datbbias","brown")'>bbias</b>: <span class="plumedtooltip" style="color:green">BIASVALUE<span class="right">Takes the value of one variable and use it as a bias <a href="https://www.plumed.org/doc-master/user-doc/html/BIASVALUE" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the labels of the scalar/vector arguments whose values will be used as a bias on the system<i></i></span></span>=<b name="data/./benchmark/4LDO/logn_jeff.datbaies">baies.ene</b> <span class="plumedtooltip">STRIDE<span class="right">the frequency with which the forces due to the bias should be calculated<i></i></span></span>=4
<span style="color:blue" class="comment">####</span>
<span style="display:none;" id="data/./benchmark/4LDO/logn_jeff.datbbias">The BIASVALUE action with label <b>bbias</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">bbias.bias</td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">bbias._bias</td><td>one or multiple instances of this quantity can be referenced elsewhere in the input file</td></tr></table></span></pre></div>

{% endraw %}
