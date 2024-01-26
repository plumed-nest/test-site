**Project ID:** [plumID:19.056]({{ '/' | absolute_url }}eggs/19/056/)  
**Source:** 4w52/plumed.dat  
**Originally used with PLUMED version:** 2.6-dev  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/4w52/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<div class="tooltip" style="color:green">UNITS<div class="right">This command sets the internal units for the code. <a href="https://www.plumed.org/doc-master/user-doc/html/_u_n_i_t_s.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">LENGTH<div class="right">the units of lengths<i></i></div></div>=A <div class="tooltip">TIME<div class="right">the units of time<i></i></div></div>=ps <div class="tooltip">ENERGY<div class="right">the units of energy<i></i></div></div>=kcal/mol
<br/><div class="tooltip" style="color:green">MAZE_LOSS<div class="right">Define a coarse-grained loss function describing interactions in a <a href="https://www.plumed.org/doc-master/user-doc/html/_m_a_z_e__l_o_s_s.html" style="color:green">More details</a><i></i></div></div> ...
  <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/4w52/plumed.datl" onclick='showPath("data/4w52/plumed.dat","data/4w52/plumed.datl")'>l</b>

  <div class="tooltip">PARAMS<div class="right">Parameters for the loss function<i></i></div></div>=1,1,1
... MAZE_LOSS
<br/><span style="display:none;" id="data/4w52/plumed.datl">The MAZE_LOSS action with label <b>l</b> calculates a scalar quantity</span><div class="tooltip" style="color:green">MAZE_SIMULATED_ANNEALING<div class="right">Calculates the biasing direction along which the ligand unbinds by minimizing <a href="https://www.plumed.org/doc-master/user-doc/html/_m_a_z_e__s_i_m_u_l_a_t_e_d__a_n_n_e_a_l_i_n_g.html" style="color:green">More details</a><i></i></div></div> ...
  <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/4w52/plumed.datopt" onclick='showPath("data/4w52/plumed.dat","data/4w52/plumed.datopt")'>opt</b>
  
  <div class="tooltip">LOSS<div class="right">Loss function describing ligand-protein interactions required by every optimizer<i></i></div></div>=<b name="data/4w52/plumed.datl">l</b>
  
  <div class="tooltip">N_ITER<div class="right">Number of optimization steps<i></i></div></div>=1000
  <div class="tooltip">OPTIMIZER_STRIDE<div class="right">Optimizer stride<i></i></div></div>=250000 <span style="color:blue"># 1 ns</span>

  <div class="tooltip">PROBABILITY_DECREASER<div class="right">Temperature-like parameter that is decreased during optimization to modify the Metropolis-Hastings acceptance probability<i></i></div></div>=300
  <div class="tooltip">COOLING<div class="right">Reduction factor for PROBABILITY_DECREASER, should be in (0, 1]<i></i></div></div>=0.95
  <div class="tooltip">COOLING_SCHEME<div class="right">Cooling scheme: geometric<i></i></div></div>=geometric  
   
  <div class="tooltip">LIGAND<div class="right">Indices of ligand atoms<i></i></div></div>=2635-2646
  <div class="tooltip">PROTEIN<div class="right">Indices of protein atoms<i></i></div></div>=1-2634

  <div class="tooltip">NLIST<div class="right"> Use a neighbor list of ligand-protein atom pairs to speed up the calculating of the distances<i></i></div></div>
  <div class="tooltip">NL_CUTOFF<div class="right">Neighbor list cut-off for the distances of ligand-protein atom pairs<i></i></div></div>=7
  <div class="tooltip">NL_STRIDE<div class="right">Update stride for the ligand-protein atom pairs in the neighbor list<i></i></div></div>=100
... MAZE_SIMULATED_ANNEALING
<br/><span style="display:none;" id="data/4w52/plumed.datopt">The MAZE_SIMULATED_ANNEALING action with label <b>opt</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">opt.x</td><td>Optimal biasing direction; x component</td></tr><tr><td width="5%">opt.y</td><td>Optimal biasing direction; y component</td></tr><tr><td width="5%">opt.z</td><td>Optimal biasing direction; z component</td></tr><tr><td width="5%">opt.loss</td><td>Loss function value defined by the provided pairing function</td></tr><tr><td width="5%">opt.sr</td><td>Sampling radius</td></tr></table></span><b name="data/4w52/plumed.datp" onclick='showPath("data/4w52/plumed.dat","data/4w52/plumed.datp")'>p</b>: <div class="tooltip" style="color:green">POSITION<div class="right">Calculate the components of the position of an atom. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_o_s_i_t_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOM<div class="right">the atom number<i></i></div></div>=2640 <div class="tooltip">NOPBC<div class="right"> ignore the periodic boundary conditions when calculating distances<i></i></div></div>
<br/><span style="display:none;" id="data/4w52/plumed.datp">The POSITION action with label <b>p</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">p.x</td><td>the x-component of the atom position</td></tr><tr><td width="5%">p.y</td><td>the y-component of the atom position</td></tr><tr><td width="5%">p.z</td><td>the z-component of the atom position</td></tr></table></span><div class="tooltip" style="color:green">MAZE_OPTIMIZER_BIAS<div class="right">Biases the ligand along the direction calculated by the chosen ef MAZE_OPTIMIZER. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_a_z_e__o_p_t_i_m_i_z_e_r__b_i_a_s.html" style="color:green">More details</a><i></i></div></div> ...
  <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/4w52/plumed.datb" onclick='showPath("data/4w52/plumed.dat","data/4w52/plumed.datb")'>b</b>  

  <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/4w52/plumed.datp">p.x</b>,<b name="data/4w52/plumed.datp">p.y</b>,<b name="data/4w52/plumed.datp">p.z</b>

  <div class="tooltip">BIASING_RATE<div class="right">Biasing rate<i></i></div></div>=0.018
  <div class="tooltip">ALPHA<div class="right">Rescaled force constant<i></i></div></div>=3.6
  <div class="tooltip">OPTIMIZER<div class="right">Optimization technique to minimize the collective variable for ligand     unbinding: RANDOM_WALK,                STEERED_MD,                RANDOM_ACCELERATION_MD,                SIMULATED_ANNEALING,                MEMETIC_SAMPLING<i></i></div></div>=<b name="data/4w52/plumed.datopt">opt</b>
... MAZE_OPTIMIZER_BIAS
<br/><span style="display:none;" id="data/4w52/plumed.datb">The MAZE_OPTIMIZER_BIAS action with label <b>b</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">b.bias</td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">b.force2</td><td>Square of the biasing force</td></tr><tr><td width="5%">b.x</td><td>Optimal biasing direction: x component</td></tr><tr><td width="5%">b.y</td><td>Optimal biasing direction: y component</td></tr><tr><td width="5%">b.z</td><td>Optimal biasing direction: z component</td></tr><tr><td width="5%">b.tdist</td><td>Total distance traveled by biased atoms</td></tr></table></span><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> ...
  <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/4w52/plumed.datopt">opt.loss</b>,<b name="data/4w52/plumed.datopt">opt.sr</b>,<b name="data/4w52/plumed.datb">b.bias</b>,<b name="data/4w52/plumed.datb">b.force2</b>,<b name="data/4w52/plumed.datb">b.tdist</b>
  <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=500
  <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=colvar
  <div class="tooltip">FMT<div class="right">the format that should be used to output real numbers<i></i></div></div>=%15.8f 
... PRINT
</pre>
{% endraw %}
