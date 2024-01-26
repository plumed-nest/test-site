**Project ID:** [plumID:22.001]({{ '/' | absolute_url }}eggs/22/001/)  
**Source:** lammps/CaCO3/chebyshev/plumed.dat  
**Originally used with PLUMED version:** 2.8  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/lammps/CaCO3/chebyshev/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue">#SETTINGS NREPLICAS=2</span>
<div class="tooltip" style="color:blue"># vim:ft=plumed<div class="right">Enables syntax highlighting for PLUMED files in vim. See <a href="https://www.plumed.org/doc-master/user-doc/html/_vim_syntax.html">here for more details. </a><i></i></div></div>
<div class="tooltip" style="color:green">UNITS<div class="right">This command sets the internal units for the code. <a href="https://www.plumed.org/doc-master/user-doc/html/_u_n_i_t_s.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">LENGTH<div class="right">the units of lengths<i></i></div></div>=A <div class="tooltip">ENERGY<div class="right">the units of energy<i></i></div></div>=eV
<br/><span style="color:blue"># CVs</span>
<b name="data/lammps/CaCO3/chebyshev/plumed.datdist" onclick='showPath("data/lammps/CaCO3/chebyshev/plumed.dat","data/lammps/CaCO3/chebyshev/plumed.datdist")'>dist</b>:  <div class="tooltip" style="color:green">DISTANCE<div class="right">Calculate the distance between a pair of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=7345,7346
<br/><span style="display:none;" id="data/lammps/CaCO3/chebyshev/plumed.datdist">The DISTANCE action with label <b>dist</b> calculates a scalar quantity</span><div class="tooltip" style="color:green">COORDINATION<div class="right">Calculate coordination numbers. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html" style="color:green">More details</a><i></i></div></div> ...
  <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/lammps/CaCO3/chebyshev/plumed.datcoord" onclick='showPath("data/lammps/CaCO3/chebyshev/plumed.dat","data/lammps/CaCO3/chebyshev/plumed.datcoord")'>coord</b>
  <div class="tooltip">GROUPA<div class="right">First list of atoms<i></i></div></div>=7345
  <div class="tooltip">GROUPB<div class="right">Second list of atoms (if empty, N*(N-1)/2 pairs in GROUPA are counted)<i></i></div></div>=2-7343:3
  <div class="tooltip">SWITCH<div class="right">This keyword is used if you want to employ an alternative to the continuous switching function defined above<i></i></div></div>={RATIONAL R_0=1.0 D_0=2.1 NN=4 MM=8}
  <div class="tooltip">NLIST<div class="right"> Use a neighbor list to speed up the calculation<i></i></div></div>
  <div class="tooltip">NL_CUTOFF<div class="right">The cutoff for the neighbor list<i></i></div></div>=10
  <div class="tooltip">NL_STRIDE<div class="right">The frequency with which we are updating the atoms in the neighbor list<i></i></div></div>=10
... COORDINATION
<br/><span style="color:blue"># Target distribution</span>
<span style="display:none;" id="data/lammps/CaCO3/chebyshev/plumed.datcoord">The COORDINATION action with label <b>coord</b> calculates a scalar quantity</span><b name="data/lammps/CaCO3/chebyshev/plumed.dattd_wt" onclick='showPath("data/lammps/CaCO3/chebyshev/plumed.dat","data/lammps/CaCO3/chebyshev/plumed.dattd_wt")'>td_wt</b>: <div class="tooltip" style="color:green">TD_WELLTEMPERED<div class="right">Well-tempered target distribution (dynamic). <a href="https://www.plumed.org/doc-master/user-doc/html/_t_d__w_e_l_l_t_e_m_p_e_r_e_d.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">BIASFACTOR<div class="right">The bias factor used for the well-tempered distribution<i></i></div></div>=5

<br/><span style="color:blue"># Basisset</span>
<div class="tooltip" style="color:green">BF_CHEBYSHEV<div class="right">Chebyshev polynomial basis functions. <a href="https://www.plumed.org/doc-master/user-doc/html/_b_f__c_h_e_b_y_s_h_e_v.html" style="color:green">More details</a><i></i></div></div> ...
  <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/lammps/CaCO3/chebyshev/plumed.datbfdist" onclick='showPath("data/lammps/CaCO3/chebyshev/plumed.dat","data/lammps/CaCO3/chebyshev/plumed.datbfdist")'>bfdist</b>
  <div class="tooltip">ORDER<div class="right">The order of the basis function expansion<i></i></div></div>=59
  <div class="tooltip">MINIMUM<div class="right">The minimum of the interval on which the basis functions are defined<i></i></div></div>=2
  <div class="tooltip">MAXIMUM<div class="right">The maximum of the interval on which the basis functions are defined<i></i></div></div>=12
... BF_CHEBYSHEV
<br/><div class="tooltip" style="color:green">BF_CHEBYSHEV<div class="right">Chebyshev polynomial basis functions. <a href="https://www.plumed.org/doc-master/user-doc/html/_b_f__c_h_e_b_y_s_h_e_v.html" style="color:green">More details</a><i></i></div></div> ...
  <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/lammps/CaCO3/chebyshev/plumed.datbfcoord" onclick='showPath("data/lammps/CaCO3/chebyshev/plumed.dat","data/lammps/CaCO3/chebyshev/plumed.datbfcoord")'>bfcoord</b>
  <div class="tooltip">ORDER<div class="right">The order of the basis function expansion<i></i></div></div>=29
  <div class="tooltip">MINIMUM<div class="right">The minimum of the interval on which the basis functions are defined<i></i></div></div>=5
  <div class="tooltip">MAXIMUM<div class="right">The maximum of the interval on which the basis functions are defined<i></i></div></div>=9
... BF_CHEBYSHEV

<br/><div class="tooltip" style="color:green">VES_LINEAR_EXPANSION<div class="right">Linear basis set expansion bias. <a href="https://www.plumed.org/doc-master/user-doc/html/_v_e_s__l_i_n_e_a_r__e_x_p_a_n_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> ...
  <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/lammps/CaCO3/chebyshev/plumed.datb1" onclick='showPath("data/lammps/CaCO3/chebyshev/plumed.dat","data/lammps/CaCO3/chebyshev/plumed.datb1")'>b1</b>
  <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/lammps/CaCO3/chebyshev/plumed.datdist">dist</b>,<b name="data/lammps/CaCO3/chebyshev/plumed.datcoord">coord</b>
  <div class="tooltip">BASIS_FUNCTIONS<div class="right">the label of the one dimensional basis functions that should be used<i></i></div></div>=<b name="data/lammps/CaCO3/chebyshev/plumed.datbfdist">bfdist</b>,<b name="data/lammps/CaCO3/chebyshev/plumed.datbfcoord">bfcoord</b>
  <div class="tooltip">TEMP<div class="right">the system temperature - this is needed if the MD code does not pass the temperature to PLUMED<i></i></div></div>=300.0
  <div class="tooltip">GRID_BINS<div class="right">the number of bins used for the grid<i></i></div></div>=300,300
  <div class="tooltip">TARGET_DISTRIBUTION<div class="right">the label of the target distribution to be used<i></i></div></div>=<b name="data/lammps/CaCO3/chebyshev/plumed.dattd_wt">td_wt</b>
... VES_LINEAR_EXPANSION
<br/><span style="display:none;" id="data/lammps/CaCO3/chebyshev/plumed.datb1">The VES_LINEAR_EXPANSION action with label <b>b1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">b1.bias</td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">b1.force2</td><td>the instantaneous value of the squared force due to this bias potential</td></tr></table></span><div class="tooltip" style="color:green">OPT_AVERAGED_SGD<div class="right">Averaged stochastic gradient decent with fixed step size. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_p_t__a_v_e_r_a_g_e_d__s_g_d.html" style="color:green">More details</a><i></i></div></div> ...
  <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/lammps/CaCO3/chebyshev/plumed.dato1" onclick='showPath("data/lammps/CaCO3/chebyshev/plumed.dat","data/lammps/CaCO3/chebyshev/plumed.dato1")'>o1</b>
  <div class="tooltip">BIAS<div class="right">the label of the VES bias to be optimized<i></i></div></div>=<b name="data/lammps/CaCO3/chebyshev/plumed.datb1">b1</b>
  <div class="tooltip">STRIDE<div class="right">the frequency of updating the coefficients given in the number of MD steps<i></i></div></div>=10
  <div class="tooltip">STEPSIZE<div class="right">the step size used for the optimization<i></i></div></div>=0.0005
  <div class="tooltip">FES_OUTPUT<div class="right">how often the FES(s) should be written out to file<i></i></div></div>=100
  <div class="tooltip">BIAS_OUTPUT<div class="right">how often the bias(es) should be written out to file<i></i></div></div>=100
  <div class="tooltip">COEFFS_OUTPUT<div class="right"> how often the coefficients should be written to file<i></i></div></div>=10
  <div class="tooltip">TARGETDIST_STRIDE<div class="right">stride for updating a target distribution that is iteratively updated during the optimization<i></i></div></div>=100
  <div class="tooltip">TARGETDIST_OUTPUT<div class="right">how often the dynamic target distribution(s) should be written out to file<i></i></div></div>=100
  <div class="tooltip">MULTIPLE_WALKERS<div class="right"> if optimization is to be performed using multiple walkers connected via MPI<i></i></div></div>
... OPT_AVERAGED_SGD
<br/><span style="display:none;" id="data/lammps/CaCO3/chebyshev/plumed.dato1">The OPT_AVERAGED_SGD action with label <b>o1</b> calculates a scalar quantity</span><div class="tooltip" style="color:green">UPPER_WALLS<div class="right">Defines a wall for the value of one or more collective variables, <a href="https://www.plumed.org/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html" style="color:green">More details</a><i></i></div></div> ...
  <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/lammps/CaCO3/chebyshev/plumed.datdist">dist</b>
  <div class="tooltip">AT<div class="right">the positions of the wall<i></i></div></div>=11
  <div class="tooltip">KAPPA<div class="right">the force constant for the wall<i></i></div></div>=12.0
  <div class="tooltip">EXP<div class="right"> the powers for the walls<i></i></div></div>=2
  <div class="tooltip">EPS<div class="right"> the values for s_i in the expression for a wall<i></i></div></div>=1
  <div class="tooltip">OFFSET<div class="right"> the offset for the start of the wall<i></i></div></div>=0
  <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/lammps/CaCO3/chebyshev/plumed.datwall" onclick='showPath("data/lammps/CaCO3/chebyshev/plumed.dat","data/lammps/CaCO3/chebyshev/plumed.datwall")'>wall</b>
... UPPER_WALLS
<br/><span style="display:none;" id="data/lammps/CaCO3/chebyshev/plumed.datwall">The UPPER_WALLS action with label <b>wall</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">wall.bias</td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">wall.force2</td><td>the instantaneous value of the squared force due to this bias potential</td></tr></table></span><div class="tooltip" style="color:green">FLUSH<div class="right">This command instructs plumed to flush all the open files with a user specified frequency. <a href="https://www.plumed.org/doc-master/user-doc/html/_f_l_u_s_h.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">STRIDE<div class="right">the frequency with which all the open files should be flushed<i></i></div></div>=10
<div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div> <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=10 <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=COLVAR
</pre>
{% endraw %}
