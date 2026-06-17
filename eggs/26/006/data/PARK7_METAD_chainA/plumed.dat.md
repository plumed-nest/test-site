**Project ID:** [plumID:26.006]({{ '/' | absolute_url }}eggs/26/006/)  
**Source:** PARK7_METAD_chainA/plumed.dat  
**Originally used with PLUMED version:** 2.9  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div class="plumedInputContainer">
<div class="plumedpreheader">
<div class="headerInfo" id="value_details_data/PARK7_METAD_chainA/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div class="containerBadge">
<div class="headerBadge"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-passing-green.svg" alt="tested onv2.10" /></a></div>
<div class="headerBadge"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></div>
</div>
</div>
<pre class="plumedlisting">
<span style="color:blue" class="comment"># protein info</span>
<span class="plumedtooltip" style="color:green">MOLINFO<span class="right">This command is used to provide information on the molecules that are present in your system. <a href="https://www.plumed.org/doc-master/user-doc/html/MOLINFO" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">STRUCTURE<span class="right">a file in pdb format containing a reference structure<i></i></span></span>=processed_chainA.pdb <span class="plumedtooltip">MOLTYPE<span class="right"> what kind of molecule is contained in the pdb file - usually not needed since protein/RNA/DNA are compatible<i></i></span></span>=protein

<span style="color:blue" class="comment"># whole molecule for all the backbone atoms</span>
<span style="display:none;" id="data/PARK7_METAD_chainA/plumed.dat">The MOLINFO action with label <b></b> calculates something</span><span class="plumedtooltip" style="color:green">WHOLEMOLECULES<span class="right">This action is used to rebuild molecules that can become split by the periodic boundary conditions. <a href="https://www.plumed.org/doc-master/user-doc/html/WHOLEMOLECULES" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ENTITY0<span class="right">the atoms that make up a molecule that you wish to align<i></i></span></span>=1-2839

<span style="color:blue" class="comment"># dihedral angles</span>
<span style="color:blue" class="comment"># P2719 ZETA</span>
<b name="data/PARK7_METAD_chainA/plumed.datzeta" onclick='showPath("data/PARK7_METAD_chainA/plumed.dat","data/PARK7_METAD_chainA/plumed.datzeta","data/PARK7_METAD_chainA/plumed.datzeta","brown")'>zeta</b>: <span class="plumedtooltip" style="color:green">TORSION<span class="right">Calculate one or multiple torsional angles. <a href="https://www.plumed.org/doc-master/user-doc/html/TORSION" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=976,980,982,985
<span style="color:blue" class="comment"># P2719 PSI</span>
<span style="display:none;" id="data/PARK7_METAD_chainA/plumed.datzeta">The TORSION action with label <b>zeta</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">zeta.value</td><td>the TORSION involving these atoms</td></tr></table></span><b name="data/PARK7_METAD_chainA/plumed.datpsi" onclick='showPath("data/PARK7_METAD_chainA/plumed.dat","data/PARK7_METAD_chainA/plumed.datpsi","data/PARK7_METAD_chainA/plumed.datpsi","brown")'>psi</b>: <span class="plumedtooltip" style="color:green">TORSION<span class="right">Calculate one or multiple torsional angles. <a href="https://www.plumed.org/doc-master/user-doc/html/TORSION" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=981,985,993,995

<span style="color:blue" class="comment"># METAD</span>
<span style="display:none;" id="data/PARK7_METAD_chainA/plumed.datpsi">The TORSION action with label <b>psi</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">psi.value</td><td>the TORSION involving these atoms</td></tr></table></span><span class="plumedtooltip" style="color:green">METAD<span class="right">Used to performed metadynamics on one or more collective variables. <a href="https://www.plumed.org/doc-master/user-doc/html/METAD" style="color:green">More details</a><i></i></span></span> ...
<span class="plumedtooltip">ARG<span class="right">the labels of the scalars on which the bias will act<i></i></span></span>=<b name="data/PARK7_METAD_chainA/plumed.datzeta">zeta</b>,<b name="data/PARK7_METAD_chainA/plumed.datpsi">psi</b>
<span class="plumedtooltip">PACE<span class="right">the frequency for hill addition<i></i></span></span>=500
<span class="plumedtooltip">HEIGHT<span class="right">the heights of the Gaussian hills<i></i></span></span>=0.8
<span class="plumedtooltip">BIASFACTOR<span class="right">use well tempered metadynamics and use this bias factor<i></i></span></span>=10 
<span class="plumedtooltip">SIGMA<span class="right">the widths of the Gaussian hills<i></i></span></span>=0.07,0.07
<span class="plumedtooltip">GRID_MIN<span class="right">the lower bounds for the grid<i></i></span></span>=-pi,-pi
<span class="plumedtooltip">GRID_MAX<span class="right">the upper bounds for the grid<i></i></span></span>=pi,pi
<span class="plumedtooltip">FILE<span class="right"> a file in which the list of added hills is stored<i></i></span></span>=HILLS_PRO
<span class="plumedtooltip">TEMP<span class="right">the system temperature - this is only needed if you are doing well-tempered metadynamics<i></i></span></span>=298
<span class="plumedtooltip">CALC_RCT<span class="right"> calculate the c(t) reweighting factor and use that to obtain the normalized bias [rbias=bias-rct]<i></i></span></span>
<span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/PARK7_METAD_chainA/plumed.datmetad" onclick='showPath("data/PARK7_METAD_chainA/plumed.dat","data/PARK7_METAD_chainA/plumed.datmetad","data/PARK7_METAD_chainA/plumed.datmetad","brown")'>metad</b>
... METAD
<br/><span style="color:blue" class="comment"># Print out information</span>
<span style="display:none;" id="data/PARK7_METAD_chainA/plumed.datmetad">The METAD action with label <b>metad</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">metad.bias</td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">metad.rbias</td><td>the instantaneous value of the bias normalized using the c(t) reweighting factor [rbias=bias-rct]</td></tr><tr><td width="5%">metad.rct</td><td>the reweighting factor c(t)</td></tr></table></span><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/PRINT" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=<b name="data/PARK7_METAD_chainA/plumed.datzeta">zeta</b>,<b name="data/PARK7_METAD_chainA/plumed.datpsi">psi</b>,<b name="data/PARK7_METAD_chainA/plumed.datmetad">metad.rbias</b>,<b name="data/PARK7_METAD_chainA/plumed.datmetad">metad.rct</b>,<b name="data/PARK7_METAD_chainA/plumed.datmetad">metad.bias</b> <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=2500 <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=COLVAR
</pre></div>

{% endraw %}
