**Project ID:** [plumID:21.006]({{ '/' | absolute_url }}eggs/21/006/)  
**Source:** ala2-well_tempered-phi/plumed.dat  
**Originally used with PLUMED version:** 2.8  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div class="plumedInputContainer">
<div class="plumedpreheader">
<div class="headerInfo" id="value_details_data/ala2-well_tempered-phi/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div class="containerBadge">
<div class="headerBadge"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-passing-green.svg" alt="tested onv2.10" /></a></div>
<div class="headerBadge"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></div>
</div>
</div>
<pre class="plumedlisting">
<span class="plumedtooltip" style="color:blue"># vim:ft=plumed<span class="right">Enables syntax highlighting for PLUMED files in vim. See <a href="https://www.plumed.org/doc-master/user-doc/html/vim">here for more details. </a><i></i></span></span>
<br/><span style="color:blue" class="comment">#+++++++++++++++++++++++++++++++++++++++++++++++++++#</span>
<span style="color:blue" class="comment">#                                                   #</span>
<span style="color:blue" class="comment">#  This input generates a well-tempered simulation  #</span>
<span style="color:blue" class="comment">#  that samples along the phi collective variable   #</span>
<span style="color:blue" class="comment">#                                                   #</span>
<span style="color:blue" class="comment">#+++++++++++++++++++++++++++++++++++++++++++++++++++#</span>
<br/><b name="data/ala2-well_tempered-phi/plumed.datphi" onclick='showPath("data/ala2-well_tempered-phi/plumed.dat","data/ala2-well_tempered-phi/plumed.datphi","data/ala2-well_tempered-phi/plumed.datphi","brown")'>phi</b>: <span class="plumedtooltip" style="color:green">TORSION<span class="right">Calculate one or multiple torsional angles. <a href="https://www.plumed.org/doc-master/user-doc/html/TORSION" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=5,7,9,15
<span style="display:none;" id="data/ala2-well_tempered-phi/plumed.datphi">The TORSION action with label <b>phi</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">phi.value</td><td>the TORSION involving these atoms</td></tr></table></span><b name="data/ala2-well_tempered-phi/plumed.datpsi" onclick='showPath("data/ala2-well_tempered-phi/plumed.dat","data/ala2-well_tempered-phi/plumed.datpsi","data/ala2-well_tempered-phi/plumed.datpsi","brown")'>psi</b>: <span class="plumedtooltip" style="color:green">TORSION<span class="right">Calculate one or multiple torsional angles. <a href="https://www.plumed.org/doc-master/user-doc/html/TORSION" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=7,9,15,17
<span style="display:none;" id="data/ala2-well_tempered-phi/plumed.datpsi">The TORSION action with label <b>psi</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">psi.value</td><td>the TORSION involving these atoms</td></tr></table></span><b name="data/ala2-well_tempered-phi/plumed.datene" onclick='showPath("data/ala2-well_tempered-phi/plumed.dat","data/ala2-well_tempered-phi/plumed.datene","data/ala2-well_tempered-phi/plumed.datene","brown")'>ene</b>: <span class="plumedtooltip" style="color:green">ENERGY<span class="right">Calculate the total potential energy of the simulation box. <a href="https://www.plumed.org/doc-master/user-doc/html/ENERGY" style="color:green">More details</a><i></i></span></span>
<br/><span style="display:none;" id="data/ala2-well_tempered-phi/plumed.datene">The ENERGY action with label <b>ene</b> calculates something</span><b name="data/ala2-well_tempered-phi/plumed.datopes" onclick='showPath("data/ala2-well_tempered-phi/plumed.dat","data/ala2-well_tempered-phi/plumed.datopes","data/ala2-well_tempered-phi/plumed.datopes","brown")'>opes</b>: <span class="plumedtooltip" style="color:green">OPES_METAD<span class="right">On-the-fly probability enhanced sampling with metadynamics-like target distribution. <a href="https://www.plumed.org/doc-master/user-doc/html/OPES_METAD" style="color:green">More details</a><i></i></span></span> ...
  <span class="plumedtooltip">ARG<span class="right">the labels of the scalars on which the bias will act<i></i></span></span>=<b name="data/ala2-well_tempered-phi/plumed.datphi">phi</b>
  <span class="plumedtooltip">FILE<span class="right"> a file in which the list of all deposited kernels is stored<i></i></span></span>=Kernels.data
  <span class="plumedtooltip">PACE<span class="right">the frequency for kernel deposition<i></i></span></span>=500
  <span class="plumedtooltip">BARRIER<span class="right">the free energy barrier to be overcome<i></i></span></span>=50
  <span class="plumedtooltip">SIGMA<span class="right"> the initial widths of the kernels<i></i></span></span>=0.15
  <span class="plumedtooltip">STATE_WFILE<span class="right">write to this file the compressed kernels and all the info needed to RESTART the simulation<i></i></span></span>=State.data
  <span class="plumedtooltip">NLIST<span class="right"> use neighbor list for kernels summation, faster but experimental<i></i></span></span>
...
<br/><span style="display:none;" id="data/ala2-well_tempered-phi/plumed.datopes">The OPES_METAD action with label <b>opes</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">opes.bias</td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">opes.rct</td><td>estimate of c(t)</td></tr><tr><td width="5%">opes.zed</td><td>estimate of Z_n</td></tr><tr><td width="5%">opes.neff</td><td>effective sample size</td></tr><tr><td width="5%">opes.nker</td><td>total number of compressed kernels used to represent the bias</td></tr><tr><td width="5%">opes.nlker</td><td>number of kernels in the neighbor list</td></tr><tr><td width="5%">opes.nlsteps</td><td>number of steps from last neighbor list update</td></tr></table></span><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/PRINT" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">FMT<span class="right"> the format that should be used to output real numbers<i></i></span></span>=%g <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=500 <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=Colvar.data <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=<b name="data/ala2-well_tempered-phi/plumed.datphi">phi</b>,<b name="data/ala2-well_tempered-phi/plumed.datpsi">psi</b>,<b name="data/ala2-well_tempered-phi/plumed.datene">ene</b>,<b name="data/ala2-well_tempered-phi/plumed.datopes">opes.bias</b>,<b name="data/ala2-well_tempered-phi/plumed.datopes">opes.rct</b>,<b name="data/ala2-well_tempered-phi/plumed.datopes">opes.zed</b>,<b name="data/ala2-well_tempered-phi/plumed.datopes">opes.nker</b>

<span style="display:none;" id="data/ala2-well_tempered-phi/plumed.dat">The PRINT action with label <b></b> calculates something</span><span class="plumedtooltip" style="color:green">ENDPLUMED<span class="right">Terminate plumed input. <a href="https://www.plumed.org/doc-master/user-doc/html/ENDPLUMED" style="color:green">More details</a><i></i></span></span><span style="color:blue" class="comment">

If no SIGMA is provided, it will be automatically guessed.
The option NLIST activates a neighbor list that speeds up the computation.

The main advantage of using OPES_METAD over a multiumbrella OPES_EXPANDED is that it is much easier to handle multiple collective variables.
</span></pre></div>

{% endraw %}
