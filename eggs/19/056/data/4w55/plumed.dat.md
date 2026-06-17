**Project ID:** [plumID:19.056]({{ '/' | absolute_url }}eggs/19/056/)  
**Source:** 4w55/plumed.dat  
**Originally used with PLUMED version:** 2.6-dev  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div class="plumedInputContainer">
<div class="plumedpreheader">
<div class="headerInfo" id="value_details_data/4w55/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div class="containerBadge">
<div class="headerBadge"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-passing-green.svg" alt="tested onv2.10" /></a></div>
<div class="headerBadge"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></div>
</div>
</div>
<pre class="plumedlisting">
<span class="plumedtooltip" style="color:green">UNITS<span class="right">This command sets the internal units for the code. <a href="https://www.plumed.org/doc-master/user-doc/html/UNITS" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">LENGTH<span class="right">the units of lengths<i></i></span></span>=A <span class="plumedtooltip">TIME<span class="right">the units of time<i></i></span></span>=ps <span class="plumedtooltip">ENERGY<span class="right">the units of energy<i></i></span></span>=kcal/mol

<span style="display:none;" id="data/4w55/plumed.dat">The UNITS action with label <b></b> calculates something</span><span class="plumedtooltip" style="color:green">MAZE_LOSS<span class="right">Define a coarse-grained loss function describing interactions in a <a href="https://www.plumed.org/doc-master/user-doc/html/MAZE_LOSS" style="color:green">More details</a><i></i></span></span> ...
  <span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/4w55/plumed.datl" onclick='showPath("data/4w55/plumed.dat","data/4w55/plumed.datl","data/4w55/plumed.datl","brown")'>l</b>

  <span class="plumedtooltip">PARAMS<span class="right">Parameters for the loss function<i></i></span></span>=1,1,1
... MAZE_LOSS
<br/><span style="display:none;" id="data/4w55/plumed.datl">The MAZE_LOSS action with label <b>l</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">l.value</td><td>the value of the loss function</td></tr></table></span><span class="plumedtooltip" style="color:green">MAZE_SIMULATED_ANNEALING<span class="right">Calculates the biasing direction along which the ligand unbinds by minimizing <a href="https://www.plumed.org/doc-master/user-doc/html/MAZE_SIMULATED_ANNEALING" style="color:green">More details</a><i></i></span></span> ...
  <span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/4w55/plumed.datopt" onclick='showPath("data/4w55/plumed.dat","data/4w55/plumed.datopt","data/4w55/plumed.datopt","brown")'>opt</b>
  
  <span class="plumedtooltip">LOSS<span class="right">Loss function describing ligand-protein interactions required by every optimizer<i></i></span></span>=<b name="data/4w55/plumed.datl">l</b>
  
  <span class="plumedtooltip">N_ITER<span class="right">Number of optimization steps<i></i></span></span>=1000
  <span class="plumedtooltip">OPTIMIZER_STRIDE<span class="right">Optimizer stride<i></i></span></span>=250000 <span style="color:blue" class="comment"># 1 ns</span>

  <span class="plumedtooltip">PROBABILITY_DECREASER<span class="right">Temperature-like parameter that is decreased during optimization to modify the Metropolis-Hastings acceptance probability<i></i></span></span>=300
  <span class="plumedtooltip">COOLING<span class="right">Reduction factor for PROBABILITY_DECREASER, should be in (0, 1]<i></i></span></span>=0.95
  <span class="plumedtooltip">COOLING_SCHEME<span class="right">Cooling scheme: geometric<i></i></span></span>=geometric  
   
  <span class="plumedtooltip">LIGAND<span class="right">Indices of ligand atoms<i></i></span></span>=2635-2655
  <span class="plumedtooltip">PROTEIN<span class="right">Indices of protein atoms<i></i></span></span>=1-2634

  <span class="plumedtooltip">NLIST<span class="right"> Use a neighbor list of ligand-protein atom pairs to speed up the calculating of the distances<i></i></span></span>
  <span class="plumedtooltip">NL_CUTOFF<span class="right">Neighbor list cut-off for the distances of ligand-protein atom pairs<i></i></span></span>=7
  <span class="plumedtooltip">NL_STRIDE<span class="right">Update stride for the ligand-protein atom pairs in the neighbor list<i></i></span></span>=100
... MAZE_SIMULATED_ANNEALING
<br/><span style="display:none;" id="data/4w55/plumed.datopt">The MAZE_SIMULATED_ANNEALING action with label <b>opt</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">opt.x</td><td>Optimal biasing direction; x component</td></tr><tr><td width="5%">opt.y</td><td>Optimal biasing direction; y component</td></tr><tr><td width="5%">opt.z</td><td>Optimal biasing direction; z component</td></tr><tr><td width="5%">opt.loss</td><td>Loss function value defined by the provided pairing function</td></tr><tr><td width="5%">opt.sr</td><td>Sampling radius</td></tr></table></span><b name="data/4w55/plumed.datp" onclick='showPath("data/4w55/plumed.dat","data/4w55/plumed.datp","data/4w55/plumed.datp","brown")'>p</b>: <span class="plumedtooltip" style="color:green">POSITION<span class="right">Calculate the components of the position of an atom or atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/POSITION" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOM<span class="right">the atom number<i></i></span></span>=2640 <span class="plumedtooltip">NOPBC<span class="right"> ignore the periodic boundary conditions when calculating distances<i></i></span></span>
<br/><span style="display:none;" id="data/4w55/plumed.datp">The POSITION action with label <b>p</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">p.x</td><td>the x-component of the atom position</td></tr><tr><td width="5%">p.y</td><td>the y-component of the atom position</td></tr><tr><td width="5%">p.z</td><td>the z-component of the atom position</td></tr></table></span><span class="plumedtooltip" style="color:green">MAZE_OPTIMIZER_BIAS<span class="right">Biases the ligand along the direction calculated by the chosen MAZE_OPTIMIZER. <a href="https://www.plumed.org/doc-master/user-doc/html/MAZE_OPTIMIZER_BIAS" style="color:green">More details</a><i></i></span></span> ...
  <span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/4w55/plumed.datb" onclick='showPath("data/4w55/plumed.dat","data/4w55/plumed.datb","data/4w55/plumed.datb","brown")'>b</b>  

  <span class="plumedtooltip">ARG<span class="right">the labels of the scalars on which the bias will act<i></i></span></span>=<b name="data/4w55/plumed.datp">p.x</b>,<b name="data/4w55/plumed.datp">p.y</b>,<b name="data/4w55/plumed.datp">p.z</b>

  <span class="plumedtooltip">BIASING_RATE<span class="right">Biasing rate<i></i></span></span>=0.03
  <span class="plumedtooltip">ALPHA<span class="right">Rescaled force constant<i></i></span></span>=3.6
  <span class="plumedtooltip">OPTIMIZER<span class="right">Optimization technique to minimize the collective variable for ligand     unbinding: RANDOM_WALK,                STEERED_MD,                RANDOM_ACCELERATION_MD,                SIMULATED_ANNEALING,                MEMETIC_SAMPLING<i></i></span></span>=<b name="data/4w55/plumed.datopt">opt</b>
... MAZE_OPTIMIZER_BIAS
<br/><span style="display:none;" id="data/4w55/plumed.datb">The MAZE_OPTIMIZER_BIAS action with label <b>b</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">b.bias</td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">b.force2</td><td>Square of the biasing force</td></tr><tr><td width="5%">b.x</td><td>Optimal biasing direction: x component</td></tr><tr><td width="5%">b.y</td><td>Optimal biasing direction: y component</td></tr><tr><td width="5%">b.z</td><td>Optimal biasing direction: z component</td></tr><tr><td width="5%">b.tdist</td><td>Total distance traveled by biased atoms</td></tr></table></span><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/PRINT" style="color:green">More details</a><i></i></span></span> ...
  <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=<b name="data/4w55/plumed.datopt">opt.loss</b>,<b name="data/4w55/plumed.datopt">opt.sr</b>,<b name="data/4w55/plumed.datb">b.bias</b>,<b name="data/4w55/plumed.datb">b.force2</b>,<b name="data/4w55/plumed.datb">b.tdist</b>
  <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=500
  <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=colvar
  <span class="plumedtooltip">FMT<span class="right"> the format that should be used to output real numbers<i></i></span></span>=%15.8f 
... PRINT
</pre></div>

{% endraw %}
