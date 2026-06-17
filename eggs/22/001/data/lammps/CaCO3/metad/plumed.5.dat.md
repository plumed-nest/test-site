**Project ID:** [plumID:22.001]({{ '/' | absolute_url }}eggs/22/001/)  
**Source:** lammps/CaCO3/metad/plumed.5.dat  
**Originally used with PLUMED version:** 2.8  
**Stable:** [zipped raw stdout](plumed.5.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.5.dat.plumed.stderr.txt.zip) - [stderr](plumed.5.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.5.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.5.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.5.dat.plumed_master.stderr)  

{% raw %}
<div class="plumedInputContainer">
<div class="plumedpreheader">
<div class="headerInfo" id="value_details_data/lammps/CaCO3/metad/plumed.5.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div class="containerBadge">
<div class="headerBadge"><a href="plumed.5.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-passing-green.svg" alt="tested onv2.10" /></a></div>
<div class="headerBadge"><a href="plumed.5.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></div>
</div>
</div>
<pre class="plumedlisting">
<span style="color:blue" class="comment">#SETTINGS NREPLICAS=2</span>
<span class="plumedtooltip" style="color:blue"># vim:ft=plumed<span class="right">Enables syntax highlighting for PLUMED files in vim. See <a href="https://www.plumed.org/doc-master/user-doc/html/vim">here for more details. </a><i></i></span></span>
<span id="data/lammps/CaCO3/metad/plumed.5.datplumed-common.dat_short"><span class="plumedtooltip" style="color:green">INCLUDE<span class="right">Includes an external input file, similar to #include in C preprocessor. <a href="https://www.plumed.org/doc-master/user-doc/html/INCLUDE">More details</a>. Show <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/lammps/CaCO3/metad/plumed.5.datplumed-common.dat");'>included file</a><i></i></span></span> <span class="plumedtooltip">FILE<span class="right">file to be included<i></i></span></span>=<a class="toggler" href='javascript:;' onclick='toggleDisplay("data/lammps/CaCO3/metad/plumed.5.datplumed-common.dat");'>plumed-common.dat</a>
</span><span id="data/lammps/CaCO3/metad/plumed.5.datplumed-common.dat_long" style="display:none;"><span style="color:blue" class="comment"># The command:
</span><span class="toggler" style="color:red" onclick='toggleDisplay("data/lammps/CaCO3/metad/plumed.5.datplumed-common.dat")'># INCLUDE FILE=plumed-common.dat
</span><span style="color:blue" class="comment"># ensures PLUMED loads the contents of the file called plumed-common.dat</span>
<span style="color:blue" class="comment"># The contents of this file are shown below (click the red comment to hide them).</span>
<span class="plumedtooltip" style="color:blue"># vim:ft=plumed<span class="right">Enables syntax highlighting for PLUMED files in vim. See <a href="https://www.plumed.org/doc-master/user-doc/html/vim">here for more details. </a><i></i></span></span>
<span style="display:none;" id="data/lammps/CaCO3/metad/plumed.5.datplumed-common.dat">The INCLUDE action with label <b>plumed-common.dat</b> calculates something</span><span class="plumedtooltip" style="color:green">UNITS<span class="right">This command sets the internal units for the code. <a href="https://www.plumed.org/doc-master/user-doc/html/UNITS" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">LENGTH<span class="right">the units of lengths<i></i></span></span>=A <span class="plumedtooltip">ENERGY<span class="right">the units of energy<i></i></span></span>=eV <span class="plumedtooltip">TIME<span class="right">the units of time<i></i></span></span>=ps

<span style="color:blue" class="comment"># CVs</span>
<span style="display:none;" id="data/lammps/CaCO3/metad/plumed.5.dat">The UNITS action with label <b></b> calculates something</span><b name="data/lammps/CaCO3/metad/plumed.5.datdist" onclick='showPath("data/lammps/CaCO3/metad/plumed.5.dat","data/lammps/CaCO3/metad/plumed.5.datdist","data/lammps/CaCO3/metad/plumed.5.datdist","brown")'>dist</b>:  <span class="plumedtooltip" style="color:green">DISTANCE<span class="right">Calculate the distance/s between pairs of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/DISTANCE" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS<span class="right">the pair of atom that we are calculating the distance between<i></i></span></span>=7345,7346

<span style="display:none;" id="data/lammps/CaCO3/metad/plumed.5.datdist">The DISTANCE action with label <b>dist</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">dist.value</td><td>the DISTANCE between this pair of atoms</td></tr></table></span><span class="plumedtooltip" style="color:green">COORDINATION<span class="right">Calculate coordination numbers. <a href="https://www.plumed.org/doc-master/user-doc/html/COORDINATION" style="color:green">More details</a><i></i></span></span> ...
  <span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/lammps/CaCO3/metad/plumed.5.datcoord" onclick='showPath("data/lammps/CaCO3/metad/plumed.5.dat","data/lammps/CaCO3/metad/plumed.5.datcoord","data/lammps/CaCO3/metad/plumed.5.datcoord","brown")'>coord</b>
  <span class="plumedtooltip">GROUPA<span class="right">First list of atoms<i></i></span></span>=7345
  <span class="plumedtooltip">GROUPB<span class="right">Second list of atoms (if empty, N*(N-1)/2 pairs in GROUPA are counted)<i></i></span></span>=2-7343:3
  <span class="plumedtooltip">SWITCH<span class="right">This keyword is used if you want to employ an alternative to the continuous switching function defined above. Options for this keyword are explained in the documentation for <a href="https://www.plumed.org/doc-master/user-doc/html/LESS_THAN">LESS_THAN</a>.<i></i></span></span>={RATIONAL R_0=1.0 D_0=2.1 NN=4 MM=8}
  <span class="plumedtooltip">NLIST<span class="right"> Use a neighbor list to speed up the calculation<i></i></span></span>
  <span class="plumedtooltip">NL_CUTOFF<span class="right">The cutoff for the neighbor list<i></i></span></span>=10
  <span class="plumedtooltip">NL_STRIDE<span class="right">The frequency with which we are updating the atoms in the neighbor list<i></i></span></span>=10
... COORDINATION

<br/><span style="color:blue" class="comment"># metad with multiple walkers</span>
<span style="display:none;" id="data/lammps/CaCO3/metad/plumed.5.datcoord">The COORDINATION action with label <b>coord</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">coord.value</td><td>the value of the coordination</td></tr></table></span><span class="plumedtooltip" style="color:green">METAD<span class="right">Used to performed metadynamics on one or more collective variables. <a href="https://www.plumed.org/doc-master/user-doc/html/METAD" style="color:green">More details</a><i></i></span></span> ...
  <span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/lammps/CaCO3/metad/plumed.5.datmetad" onclick='showPath("data/lammps/CaCO3/metad/plumed.5.dat","data/lammps/CaCO3/metad/plumed.5.datmetad","data/lammps/CaCO3/metad/plumed.5.datmetad","brown")'>metad</b>
  <span class="plumedtooltip">ARG<span class="right">the labels of the scalars on which the bias will act<i></i></span></span>=<b name="data/lammps/CaCO3/metad/plumed.5.datdist">dist</b>,<b name="data/lammps/CaCO3/metad/plumed.5.datcoord">coord</b>
  <span class="plumedtooltip">SIGMA<span class="right">the widths of the Gaussian hills<i></i></span></span>=0.2,0.1
  <span class="plumedtooltip">HEIGHT<span class="right">the heights of the Gaussian hills<i></i></span></span>=0.025852
  <span class="plumedtooltip">BIASFACTOR<span class="right">use well tempered metadynamics and use this bias factor<i></i></span></span>=5
  <span class="plumedtooltip">TEMP<span class="right">the system temperature - this is only needed if you are doing well-tempered metadynamics<i></i></span></span>=300
  <span class="plumedtooltip">PACE<span class="right">the frequency for hill addition<i></i></span></span>=1000
  <span class="plumedtooltip">GRID_MIN<span class="right">the lower bounds for the grid<i></i></span></span>=2,3
  <span class="plumedtooltip">GRID_MAX<span class="right">the upper bounds for the grid<i></i></span></span>=13,10
  <span class="plumedtooltip">CALC_RCT<span class="right"> calculate the c(t) reweighting factor and use that to obtain the normalized bias [rbias=bias-rct]<i></i></span></span>
  <span class="plumedtooltip">WALKERS_MPI<span class="right"> Switch on MPI version of multiple walkers - not compatible with WALKERS_* options other than WALKERS_DIR<i></i></span></span>
... METAD
<br/><span style="color:blue" class="comment"># walls to stay close to associated state</span>
<span style="display:none;" id="data/lammps/CaCO3/metad/plumed.5.datmetad">The METAD action with label <b>metad</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">metad.bias</td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">metad.rbias</td><td>the instantaneous value of the bias normalized using the c(t) reweighting factor [rbias=bias-rct]</td></tr><tr><td width="5%">metad.rct</td><td>the reweighting factor c(t)</td></tr></table></span><span class="plumedtooltip" style="color:green">UPPER_WALLS<span class="right">Defines a wall for the value of one or more collective variables, <a href="https://www.plumed.org/doc-master/user-doc/html/UPPER_WALLS" style="color:green">More details</a><i></i></span></span> ...
  <span class="plumedtooltip">ARG<span class="right">the arguments on which the bias is acting<i></i></span></span>=<b name="data/lammps/CaCO3/metad/plumed.5.datdist">dist</b>
  <span class="plumedtooltip">AT<span class="right">the positions of the wall<i></i></span></span>=12
  <span class="plumedtooltip">KAPPA<span class="right">the force constant for the wall<i></i></span></span>=12.0
  <span class="plumedtooltip">EXP<span class="right"> the powers for the walls<i></i></span></span>=2
  <span class="plumedtooltip">EPS<span class="right"> the values for s_i in the expression for a wall<i></i></span></span>=1
  <span class="plumedtooltip">OFFSET<span class="right"> the offset for the start of the wall<i></i></span></span>=0.
  <span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/lammps/CaCO3/metad/plumed.5.datwall" onclick='showPath("data/lammps/CaCO3/metad/plumed.5.dat","data/lammps/CaCO3/metad/plumed.5.datwall","data/lammps/CaCO3/metad/plumed.5.datwall","brown")'>wall</b>
... UPPER_WALLS
<span style="color:blue"># --- End of included input --- </span></span><br/><span style="display:none;" id="data/lammps/CaCO3/metad/plumed.5.datwall">The UPPER_WALLS action with label <b>wall</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">wall.bias</td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">wall.force2</td><td>the instantaneous value of the squared force due to this bias potential</td></tr></table></span><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/PRINT" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=* <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=100 <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=COLVAR
</pre></div>

{% endraw %}
