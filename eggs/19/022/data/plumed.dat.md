**Project ID:** [plumID:19.022]({{ '/' | absolute_url }}eggs/19/022/)  
**Source:** plumed.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div class="plumedInputContainer">
<div class="plumedpreheader">
<div class="headerInfo" id="value_details_data/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div class="containerBadge">
<div class="headerBadge"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-passing-green.svg" alt="tested onv2.10" /></a></div>
<div class="headerBadge"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></div>
</div>
</div>
<pre class="plumedlisting">
<b name="data/plumed.datphi" onclick='showPath("data/plumed.dat","data/plumed.datphi","data/plumed.datphi","brown")'>phi</b>: <span class="plumedtooltip" style="color:green">TORSION<span class="right">Calculate one or multiple torsional angles. <a href="https://www.plumed.org/doc-master/user-doc/html/TORSION" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=5,7,9,15
<span style="display:none;" id="data/plumed.datphi">The TORSION action with label <b>phi</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">phi.value</td><td>the TORSION involving these atoms</td></tr></table></span><b name="data/plumed.datpsi" onclick='showPath("data/plumed.dat","data/plumed.datpsi","data/plumed.datpsi","brown")'>psi</b>: <span class="plumedtooltip" style="color:green">TORSION<span class="right">Calculate one or multiple torsional angles. <a href="https://www.plumed.org/doc-master/user-doc/html/TORSION" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=7,9,15,17

<span style="display:none;" id="data/plumed.datpsi">The TORSION action with label <b>psi</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">psi.value</td><td>the TORSION involving these atoms</td></tr></table></span><span class="plumedtooltip" style="color:green">DRR<span class="right">Used to performed extended-system adaptive biasing force (eABF) <a href="https://www.plumed.org/doc-master/user-doc/html/DRR" style="color:green">More details</a><i></i></span></span> ...
<span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/plumed.datalad" onclick='showPath("data/plumed.dat","data/plumed.datalad","data/plumed.datalad","brown")'>alad</b>
<span class="plumedtooltip">ARG<span class="right">the labels of the scalars on which the bias will act<i></i></span></span>=<b name="data/plumed.datphi">phi</b>,<b name="data/plumed.datpsi">psi</b>
<span class="plumedtooltip">FULLSAMPLES<span class="right"> number of samples in a bin prior to application of the ABF<i></i></span></span>=500
<span class="plumedtooltip">GRID_MIN<span class="right">the lower bounds for the grid (GRID_BIN or GRID_SPACING should be specified)<i></i></span></span>=-pi,-pi
<span class="plumedtooltip">GRID_MAX<span class="right">the upper bounds for the grid (GRID_BIN or GRID_SPACING should be specified)<i></i></span></span>=pi,pi
<span class="plumedtooltip">GRID_BIN<span class="right">the number of bins for the grid<i></i></span></span>=180,180
<span class="plumedtooltip">FRICTION<span class="right"> add a friction to the variable, similar to extended Langevin Damping in Colvars<i></i></span></span>=2.0,2.0
<span class="plumedtooltip">TAU<span class="right"> specifies relaxation time on each of variables are, similar to extended Time Constant in Colvars<i></i></span></span>=0.2,0.2
<span class="plumedtooltip">OUTPUTFREQ<span class="right">write results to a file every N steps<i></i></span></span>=50000
<span class="plumedtooltip">HISTORYFREQ<span class="right">save history to a file every N steps<i></i></span></span>=500000
... DRR
<br/><span style="display:none;" id="data/plumed.datalad">The DRR action with label <b>alad</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">alad.bias</td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">alad._fict</td><td>one or multiple instances of this quantity can be referenced elsewhere in the input file</td></tr><tr><td width="5%">alad._vfict</td><td>one or multiple instances of this quantity can be referenced elsewhere in the input file</td></tr><tr><td width="5%">alad._biasforce</td><td>The bias force from eABF/DRR of the fictitious particle</td></tr><tr><td width="5%">alad._springforce</td><td>Spring force between real CVs and extended CVs</td></tr><tr><td width="5%">alad._fictNoPBC</td><td>the positions of fictitious particles (without PBC)</td></tr></table></span><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/PRINT" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=10 <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=<b name="data/plumed.datphi">phi</b>,<b name="data/plumed.datpsi">psi</b>,<b name="data/plumed.datalad">alad.phi_fict</b>,<b name="data/plumed.datalad">alad.psi_fict</b>,<b name="data/plumed.datalad">alad.phi_biasforce</b>,<b name="data/plumed.datalad">alad.psi_biasforce</b> <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=COLVAR
</pre></div>

{% endraw %}
