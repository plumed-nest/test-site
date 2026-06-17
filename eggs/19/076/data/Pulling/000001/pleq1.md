**Project ID:** [plumID:19.076]({{ '/' | absolute_url }}eggs/19/076/)  
**Source:** Pulling/000001/pleq1  
**Originally used with PLUMED version:** 2.1  
**Stable:** [zipped raw stdout](pleq1.plumed.stdout.txt.zip) - [zipped raw stderr](pleq1.plumed.stderr.txt.zip) - [stderr](pleq1.plumed.stderr)  
**Master:** [zipped raw stdout](pleq1.plumed_master.stdout.txt.zip) - [zipped raw stderr](pleq1.plumed_master.stderr.txt.zip) - [stderr](pleq1.plumed_master.stderr)  

{% raw %}
<div class="plumedInputContainer">
<div class="plumedpreheader">
<div class="headerInfo" id="value_details_data/Pulling/000001/pleq1"> Click on the labels of the actions for more information on what each action computes </div>
<div class="containerBadge">
<div class="headerBadge"><a href="pleq1.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-passing-green.svg" alt="tested onv2.10" /></a></div>
<div class="headerBadge"><a href="pleq1.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></div>
</div>
</div>
<pre class="plumedlisting">
<span style="color:blue" class="comment"># Adapt units to LAMMPS script (units real)</span>
<span class="plumedtooltip" style="color:green">UNITS<span class="right">This command sets the internal units for the code. <a href="https://www.plumed.org/doc-master/user-doc/html/UNITS" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">LENGTH<span class="right">the units of lengths<i></i></span></span>=A <span class="plumedtooltip">TIME<span class="right">the units of time<i></i></span></span>=fs <span class="plumedtooltip">ENERGY<span class="right">the units of energy<i></i></span></span>=kcal/mol

<span style="color:blue" class="comment"># Radius of Gyration</span>
<span style="display:none;" id="data/Pulling/000001/pleq1">The UNITS action with label <b></b> calculates something</span><b name="data/Pulling/000001/pleq1rg" onclick='showPath("data/Pulling/000001/pleq1","data/Pulling/000001/pleq1rg","data/Pulling/000001/pleq1rg","brown")'>rg</b>: <span class="plumedtooltip" style="color:green">GYRATION<span class="right">Calculate the radius of gyration, or other properties related to it. <a href="https://www.plumed.org/doc-master/user-doc/html/GYRATION" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">TYPE<span class="right"> The type of calculation relative to the Gyration Tensor you want to perform<i></i></span></span>=RADIUS <span class="plumedtooltip">ATOMS<span class="right">the group of atoms that you are calculating the Gyration Tensor for<i></i></span></span>=1-293


<span style="display:none;" id="data/Pulling/000001/pleq1rg">The GYRATION action with label <b>rg</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">rg.value</td><td>the radius that was computed from the weights</td></tr></table></span><b name="data/Pulling/000001/pleq1restr" onclick='showPath("data/Pulling/000001/pleq1","data/Pulling/000001/pleq1restr","data/Pulling/000001/pleq1restr","brown")'>restr</b>: ...
        <span class="plumedtooltip" style="color:green">MOVINGRESTRAINT<span class="right">Add a time-dependent, harmonic restraint on one or more variables. <a href="https://www.plumed.org/doc-master/user-doc/html/MOVINGRESTRAINT" style="color:green">More details</a><i></i></span></span>
        <span class="plumedtooltip">ARG<span class="right">the labels of the scalars on which the bias will act<i></i></span></span>=<b name="data/Pulling/000001/pleq1rg">rg</b>
        <span class="plumedtooltip">STEP0<span class="right">This keyword appears multiple times as STEPx with x=0,1,2,<i></i></span></span>=0 <span class="plumedtooltip">AT0<span class="right">ATx is equal to the position of the restraint at time STEPx<i></i></span></span>=31.5315 <span class="plumedtooltip">KAPPA0<span class="right">KAPPAx is equal to the value of the force constants at time STEPx<i></i></span></span>=10
        <span class="plumedtooltip">STEP1<span class="right">This keyword appears multiple times as STEPx with x=0,1,2,<i></i></span></span>=1 <span class="plumedtooltip">AT1<span class="right">ATx is equal to the position of the restraint at time STEPx<i></i></span></span>=31.5315 <span class="plumedtooltip">KAPPA1<span class="right">KAPPAx is equal to the value of the force constants at time STEPx<i></i></span></span>=10
...
<span style="color:blue" class="comment"># Print rg</span>
<span style="display:none;" id="data/Pulling/000001/pleq1restr">The MOVINGRESTRAINT action with label <b>restr</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">restr.bias</td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">restr.work</td><td>the total work performed changing this restraint</td></tr><tr><td width="5%">restr.force2</td><td>the instantaneous value of the squared force due to this bias potential</td></tr><tr><td width="5%">restr._cntr</td><td>one or multiple instances of this quantity can be referenced elsewhere in the input file</td></tr><tr><td width="5%">restr._work</td><td>one or multiple instances of this quantity can be referenced elsewhere in the input file</td></tr><tr><td width="5%">restr._kappa</td><td>one or multiple instances of this quantity can be referenced elsewhere in the input file</td></tr></table></span><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/PRINT" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=<b name="data/Pulling/000001/pleq1rg">rg</b>,<b name="data/Pulling/000001/pleq1restr">restr.rg_cntr</b>,<b name="data/Pulling/000001/pleq1restr">restr.rg_work</b> <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=workeq1 <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=100000

<span style="color:blue" class="comment"># End of Program</span>
<span class="plumedtooltip" style="color:green">ENDPLUMED<span class="right">Terminate plumed input. <a href="https://www.plumed.org/doc-master/user-doc/html/ENDPLUMED" style="color:green">More details</a><i></i></span></span><span style="color:blue" class="comment">
</span></pre></div>

{% endraw %}
