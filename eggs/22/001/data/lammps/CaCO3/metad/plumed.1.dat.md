**Project ID:** [plumID:22.001]({{ '/' | absolute_url }}eggs/22/001/)  
**Source:** lammps/CaCO3/metad/plumed.1.dat  
**Originally used with PLUMED version:** 2.8  
**Stable:** [zipped raw stdout](plumed.1.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.1.dat.plumed.stderr.txt.zip) - [stderr](plumed.1.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.1.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.1.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.1.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/lammps/CaCO3/metad/plumed.1.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.1.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.1.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue">#SETTINGS NREPLICAS=2</span>
<div class="tooltip" style="color:blue"># vim:ft=plumed<div class="right">Enables syntax highlighting for PLUMED files in vim. See <a href="https://www.plumed.org/doc-master/user-doc/html/_vim_syntax.html">here for more details. </a><i></i></div></div>
<span id="data/lammps/CaCO3/metad/plumed.1.datplumed-common.dat_short"><div class="tooltip" style="color:green">INCLUDE<div class="right">Includes an external input file, similar to #include in C preprocessor. <a href="https://www.plumed.org/doc-master/user-doc/html/_i_n_c_l_u_d_e.html">More details</a>. Show <a href='javascript:;' onclick='toggleDisplay("data/lammps/CaCO3/metad/plumed.1.datplumed-common.dat");'>included file</a><i></i></div></div> <div class="tooltip">FILE<div class="right">file to be included<i></i></div></div>=<a href='javascript:;' onclick='toggleDisplay("data/lammps/CaCO3/metad/plumed.1.datplumed-common.dat");'>plumed-common.dat</a>
</span><span id="data/lammps/CaCO3/metad/plumed.1.datplumed-common.dat_long" style="display:none;"><span style="color:blue"># The command:
</span><span style="color:red" onclick='toggleDisplay("data/lammps/CaCO3/metad/plumed.1.datplumed-common.dat")'># INCLUDE FILE=plumed-common.dat
</span><span style="color:blue"># ensures PLUMED loads the contents of the file called plumed-common.dat</span>
<span style="color:blue"># The contents of this file are shown below (click the red comment to hide them).</span>
<div class="tooltip" style="color:blue"># vim:ft=plumed<div class="right">Enables syntax highlighting for PLUMED files in vim. See <a href="https://www.plumed.org/doc-master/user-doc/html/_vim_syntax.html">here for more details. </a><i></i></div></div>
<div class="tooltip" style="color:green">UNITS<div class="right">This command sets the internal units for the code. <a href="https://www.plumed.org/doc-master/user-doc/html/_u_n_i_t_s.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">LENGTH<div class="right">the units of lengths<i></i></div></div>=A <div class="tooltip">ENERGY<div class="right">the units of energy<i></i></div></div>=eV <div class="tooltip">TIME<div class="right">the units of time<i></i></div></div>=ps
<br/><span style="color:blue"># CVs</span>
<b name="data/lammps/CaCO3/metad/plumed.1.datdist" onclick='showPath("data/lammps/CaCO3/metad/plumed.1.dat","data/lammps/CaCO3/metad/plumed.1.datdist")'>dist</b>:  <div class="tooltip" style="color:green">DISTANCE<div class="right">Calculate the distance between a pair of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=7345,7346
<br/><span style="display:none;" id="data/lammps/CaCO3/metad/plumed.1.datdist">The DISTANCE action with label <b>dist</b> calculates a scalar quantity</span><div class="tooltip" style="color:green">COORDINATION<div class="right">Calculate coordination numbers. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html" style="color:green">More details</a><i></i></div></div> ...
  <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/lammps/CaCO3/metad/plumed.1.datcoord" onclick='showPath("data/lammps/CaCO3/metad/plumed.1.dat","data/lammps/CaCO3/metad/plumed.1.datcoord")'>coord</b>
  <div class="tooltip">GROUPA<div class="right">First list of atoms<i></i></div></div>=7345
  <div class="tooltip">GROUPB<div class="right">Second list of atoms (if empty, N*(N-1)/2 pairs in GROUPA are counted)<i></i></div></div>=2-7343:3
  <div class="tooltip">SWITCH<div class="right">This keyword is used if you want to employ an alternative to the continuous switching function defined above<i></i></div></div>={RATIONAL R_0=1.0 D_0=2.1 NN=4 MM=8}
  <div class="tooltip">NLIST<div class="right"> Use a neighbor list to speed up the calculation<i></i></div></div>
  <div class="tooltip">NL_CUTOFF<div class="right">The cutoff for the neighbor list<i></i></div></div>=10
  <div class="tooltip">NL_STRIDE<div class="right">The frequency with which we are updating the atoms in the neighbor list<i></i></div></div>=10
... COORDINATION

<br/><span style="color:blue"># metad with multiple walkers</span>
<span style="display:none;" id="data/lammps/CaCO3/metad/plumed.1.datcoord">The COORDINATION action with label <b>coord</b> calculates a scalar quantity</span><div class="tooltip" style="color:green">METAD<div class="right">Used to performed metadynamics on one or more collective variables. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_e_t_a_d.html" style="color:green">More details</a><i></i></div></div> ...
  <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/lammps/CaCO3/metad/plumed.1.datmetad" onclick='showPath("data/lammps/CaCO3/metad/plumed.1.dat","data/lammps/CaCO3/metad/plumed.1.datmetad")'>metad</b>
  <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/lammps/CaCO3/metad/plumed.1.datdist">dist</b>,<b name="data/lammps/CaCO3/metad/plumed.1.datcoord">coord</b>
  <div class="tooltip">SIGMA<div class="right">the widths of the Gaussian hills<i></i></div></div>=0.2,0.1
  <div class="tooltip">HEIGHT<div class="right">the heights of the Gaussian hills<i></i></div></div>=0.025852
  <div class="tooltip">BIASFACTOR<div class="right">use well tempered metadynamics and use this bias factor<i></i></div></div>=5
  <div class="tooltip">TEMP<div class="right">the system temperature - this is only needed if you are doing well-tempered metadynamics<i></i></div></div>=300
  <div class="tooltip">PACE<div class="right">the frequency for hill addition<i></i></div></div>=1000
  <div class="tooltip">GRID_MIN<div class="right">the lower bounds for the grid<i></i></div></div>=2,3
  <div class="tooltip">GRID_MAX<div class="right">the upper bounds for the grid<i></i></div></div>=13,10
  <div class="tooltip">CALC_RCT<div class="right"> calculate the c(t) reweighting factor and use that to obtain the normalized bias [rbias=bias-rct]<i></i></div></div>
  <div class="tooltip">WALKERS_MPI<div class="right"> Switch on MPI version of multiple walkers - not compatible with WALKERS_* options other than WALKERS_DIR<i></i></div></div>
... METAD
<br/><span style="color:blue"># walls to stay close to associated state</span>
<span style="display:none;" id="data/lammps/CaCO3/metad/plumed.1.datmetad">The METAD action with label <b>metad</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">metad.bias</td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">metad.rbias</td><td>the instantaneous value of the bias normalized using the c(t) reweighting factor [rbias=bias-rct]</td></tr><tr><td width="5%">metad.rct</td><td>the reweighting factor $c(t)$</td></tr></table></span><div class="tooltip" style="color:green">UPPER_WALLS<div class="right">Defines a wall for the value of one or more collective variables, <a href="https://www.plumed.org/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html" style="color:green">More details</a><i></i></div></div> ...
  <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/lammps/CaCO3/metad/plumed.1.datdist">dist</b>
  <div class="tooltip">AT<div class="right">the positions of the wall<i></i></div></div>=12
  <div class="tooltip">KAPPA<div class="right">the force constant for the wall<i></i></div></div>=12.0
  <div class="tooltip">EXP<div class="right"> the powers for the walls<i></i></div></div>=2
  <div class="tooltip">EPS<div class="right"> the values for s_i in the expression for a wall<i></i></div></div>=1
  <div class="tooltip">OFFSET<div class="right"> the offset for the start of the wall<i></i></div></div>=0
  <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/lammps/CaCO3/metad/plumed.1.datwall" onclick='showPath("data/lammps/CaCO3/metad/plumed.1.dat","data/lammps/CaCO3/metad/plumed.1.datwall")'>wall</b>
... UPPER_WALLS
<span style="color:blue"># --- End of included input --- </span></span><br/><span style="display:none;" id="data/lammps/CaCO3/metad/plumed.1.datwall">The UPPER_WALLS action with label <b>wall</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">wall.bias</td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">wall.force2</td><td>the instantaneous value of the squared force due to this bias potential</td></tr></table></span><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div> <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=100 <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=COLVAR
</pre>
{% endraw %}
