**Project ID:** [plumID:20.022]({{ '/' | absolute_url }}eggs/20/022/)  
**Source:** chignolin/plumed.dat  
**Originally used with PLUMED version:** 2.8  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div class="plumedInputContainer">
<div class="plumedpreheader">
<div class="headerInfo" id="value_details_data/chignolin/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div class="containerBadge">
<div class="headerBadge"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-passing-green.svg" alt="tested onv2.10" /></a></div>
<div class="headerBadge"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></div>
</div>
</div>
<pre class="plumedlisting">
<span class="plumedtooltip" style="color:blue"># vim:ft=plumed<span class="right">Enables syntax highlighting for PLUMED files in vim. See <a href="https://www.plumed.org/doc-master/user-doc/html/vim">here for more details. </a><i></i></span></span>
<br/><span style="color:blue" class="comment">#++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++#</span>
<span style="color:blue" class="comment">#                                                                  #</span>
<span style="color:blue" class="comment">#  This input generates a multithermal-multibaric simulation that  #</span>
<span style="color:blue" class="comment">#  samples a whole range of temperatures and pressures, using a    #</span>
<span style="color:blue" class="comment">#  chosen fixed number of replicas (multiple walkers)              #</span>
<span style="color:blue" class="comment">#                                                                  #</span>
<span style="color:blue" class="comment">#++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++#</span>
<br/><span style="color:blue" class="comment">#RESTART</span>
<span class="plumedtooltip" style="color:green">MOLINFO<span class="right">This command is used to provide information on the molecules that are present in your system. <a href="https://www.plumed.org/doc-master/user-doc/html/MOLINFO" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">STRUCTURE<span class="right">a file in pdb format containing a reference structure<i></i></span></span>=input-chignolin.pdb
<span style="display:none;" id="data/chignolin/plumed.dat">The MOLINFO action with label <b></b> calculates something</span><span class="plumedtooltip" style="color:green">WHOLEMOLECULES<span class="right">This action is used to rebuild molecules that can become split by the periodic boundary conditions. <a href="https://www.plumed.org/doc-master/user-doc/html/WHOLEMOLECULES" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which molecules are reassembled<i></i></span></span>=1 <span class="plumedtooltip">ENTITY0<span class="right">the atoms that make up a molecule that you wish to align<i></i></span></span>=1-166

<b name="data/chignolin/plumed.datene" onclick='showPath("data/chignolin/plumed.dat","data/chignolin/plumed.datene","data/chignolin/plumed.datene","brown")'>ene</b>: <span class="plumedtooltip" style="color:green">ENERGY<span class="right">Calculate the total potential energy of the simulation box. <a href="https://www.plumed.org/doc-master/user-doc/html/ENERGY" style="color:green">More details</a><i></i></span></span>
<span style="display:none;" id="data/chignolin/plumed.datene">The ENERGY action with label <b>ene</b> calculates something</span><b name="data/chignolin/plumed.datvol" onclick='showPath("data/chignolin/plumed.dat","data/chignolin/plumed.datvol","data/chignolin/plumed.datvol","brown")'>vol</b>: <span class="plumedtooltip" style="color:green">VOLUME<span class="right">Calculate the volume the simulation box. <a href="https://www.plumed.org/doc-master/user-doc/html/VOLUME" style="color:green">More details</a><i></i></span></span>
<span style="display:none;" id="data/chignolin/plumed.datvol">The VOLUME action with label <b>vol</b> calculates the volume of simulation box</span><b name="data/chignolin/plumed.datpdb_rmsd" onclick='showPath("data/chignolin/plumed.dat","data/chignolin/plumed.datpdb_rmsd","data/chignolin/plumed.datpdb_rmsd","brown")'>pdb_rmsd</b>: <span class="plumedtooltip" style="color:green">RMSD<span class="right">Calculate the RMSD with respect to a reference structure. <a href="https://www.plumed.org/doc-master/user-doc/html/RMSD" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">REFERENCE<span class="right">a file in pdb format containing the reference structure and the atoms involved in the CV<i></i></span></span>=input-chignolin.pdb <span class="plumedtooltip">TYPE<span class="right"> the manner in which RMSD alignment is performed<i></i></span></span>=OPTIMAL

<span style="display:none;" id="data/chignolin/plumed.datpdb_rmsd">The RMSD action with label <b>pdb_rmsd</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">pdb_rmsd.value</td><td>the RMSD distance between the instaneous structure and the reference structure/s that were input</td></tr></table></span><b name="data/chignolin/plumed.datecv" onclick='showPath("data/chignolin/plumed.dat","data/chignolin/plumed.datecv","data/chignolin/plumed.datecv","brown")'>ecv</b>: <span class="plumedtooltip" style="color:green">ECV_MULTITHERMAL_MULTIBARIC<span class="right">Expand a simulation to sample multiple temperatures and pressures. <a href="https://www.plumed.org/doc-master/user-doc/html/ECV_MULTITHERMAL_MULTIBARIC" style="color:green">More details</a><i></i></span></span> ...
  <span class="plumedtooltip">ARG<span class="right">the labels of the potential energy and of the volume of the system<i></i></span></span>=<b name="data/chignolin/plumed.datene">ene</b>,<b name="data/chignolin/plumed.datvol">vol</b>
<span style="color:blue" class="comment"># TEMP=500</span>
  <span class="plumedtooltip">TEMP_MIN<span class="right">the minimum of the temperature range<i></i></span></span>=270
  <span class="plumedtooltip">TEMP_MAX<span class="right">the maximum of the temperature range<i></i></span></span>=800
  <span class="plumedtooltip">PRESSURE<span class="right">pressure<i></i></span></span>=0.06022140857*2000 <span style="color:blue" class="comment">#2 kbar</span>
  <span class="plumedtooltip">PRESSURE_MIN<span class="right">the minimum of the pressure range<i></i></span></span>=0.06022140857  <span style="color:blue" class="comment">#1 bar</span>
  <span class="plumedtooltip">PRESSURE_MAX<span class="right">the maximum of the pressure range<i></i></span></span>=0.06022140857*4000 <span style="color:blue" class="comment">#4 kbar</span>
  <span class="plumedtooltip">CUT_CORNER<span class="right">avoid region of high temperature and low pressure<i></i></span></span>=500,0.06022140857,800,0.06022140857*1000
...
<span style="display:none;" id="data/chignolin/plumed.datecv">The ECV_MULTITHERMAL_MULTIBARIC action with label <b>ecv</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ecv..#!custom</td><td>the names of the output components for this action depend on the actions input file see the example inputs below for details</td></tr></table></span><b name="data/chignolin/plumed.datopes" onclick='showPath("data/chignolin/plumed.dat","data/chignolin/plumed.datopes","data/chignolin/plumed.datopes","brown")'>opes</b>: <span class="plumedtooltip" style="color:green">OPES_EXPANDED<span class="right">On-the-fly probability enhanced sampling with expanded ensembles for the target distribution. <a href="https://www.plumed.org/doc-master/user-doc/html/OPES_EXPANDED" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the label of the ECVs that define the expansion<i></i></span></span>=<b name="data/chignolin/plumed.datecv">ecv.*</b> <span class="plumedtooltip">FILE<span class="right"> a file with the estimate of the relative Delta F for each component of the target and of the global c(t)<i></i></span></span>=DeltaFs.data <span class="plumedtooltip">PACE<span class="right">how often the bias is updated<i></i></span></span>=500 <span class="plumedtooltip">WALKERS_MPI<span class="right"> switch on MPI version of multiple walkers<i></i></span></span>
<br/><span style="color:blue" class="comment">#e2e: DISTANCE ATOMS=5,147 #first and last CA</span>
<span style="color:blue" class="comment">#gyr: GYRATION ATOMS=5,26,47,67,73,88,102,109,123,147</span>
<br/><span style="display:none;" id="data/chignolin/plumed.datopes">The OPES_EXPANDED action with label <b>opes</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">opes.bias</td><td>the instantaneous value of the bias potential</td></tr></table></span><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/PRINT" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">FMT<span class="right"> the format that should be used to output real numbers<i></i></span></span>=%g <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=500 <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=Colvar.data <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=<b name="data/chignolin/plumed.datene">ene</b>,<b name="data/chignolin/plumed.datvol">vol</b>,<b name="data/chignolin/plumed.datpdb_rmsd">pdb_rmsd</b>,<b name="data/chignolin/plumed.datopes">opes.*</b>

<span class="plumedtooltip" style="color:green">ENDPLUMED<span class="right">Terminate plumed input. <a href="https://www.plumed.org/doc-master/user-doc/html/ENDPLUMED" style="color:green">More details</a><i></i></span></span><span style="color:blue" class="comment">

temp=500 K
pres=2000 bar

input obtained from unbiased simultation, only rep 6,8,9 start from folded
</span></pre></div>

{% endraw %}
