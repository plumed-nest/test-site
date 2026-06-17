**Project ID:** [plumID:22.003]({{ '/' | absolute_url }}eggs/22/003/)  
**Source:** ala2/opes/plumed.dat  
**Originally used with PLUMED version:** 2.8  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div class="plumedInputContainer">
<div class="plumedpreheader">
<div class="headerInfo" id="value_details_data/ala2/opes/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div class="containerBadge">
<div class="headerBadge"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-passing-green.svg" alt="tested onv2.10" /></a></div>
<div class="headerBadge"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></div>
</div>
</div>
<pre class="plumedlisting">
<span class="plumedtooltip" style="color:blue"># vim:ft=plumed<span class="right">Enables syntax highlighting for PLUMED files in vim. See <a href="https://www.plumed.org/doc-master/user-doc/html/vim">here for more details. </a><i></i></span></span>
<br/><b name="data/ala2/opes/plumed.datphi" onclick='showPath("data/ala2/opes/plumed.dat","data/ala2/opes/plumed.datphi","data/ala2/opes/plumed.datphi","brown")'>phi</b>: <span class="plumedtooltip" style="color:green">TORSION<span class="right">Calculate one or multiple torsional angles. <a href="https://www.plumed.org/doc-master/user-doc/html/TORSION" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=5,7,9,15
<span style="display:none;" id="data/ala2/opes/plumed.datphi">The TORSION action with label <b>phi</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">phi.value</td><td>the TORSION involving these atoms</td></tr></table></span><b name="data/ala2/opes/plumed.datpsi" onclick='showPath("data/ala2/opes/plumed.dat","data/ala2/opes/plumed.datpsi","data/ala2/opes/plumed.datpsi","brown")'>psi</b>: <span class="plumedtooltip" style="color:green">TORSION<span class="right">Calculate one or multiple torsional angles. <a href="https://www.plumed.org/doc-master/user-doc/html/TORSION" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=7,9,15,17

<span style="display:none;" id="data/ala2/opes/plumed.datpsi">The TORSION action with label <b>psi</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">psi.value</td><td>the TORSION involving these atoms</td></tr></table></span><b name="data/ala2/opes/plumed.datopes" onclick='showPath("data/ala2/opes/plumed.dat","data/ala2/opes/plumed.datopes","data/ala2/opes/plumed.datopes","brown")'>opes</b>: <span class="plumedtooltip" style="color:green">OPES_METAD<span class="right">On-the-fly probability enhanced sampling with metadynamics-like target distribution. <a href="https://www.plumed.org/doc-master/user-doc/html/OPES_METAD" style="color:green">More details</a><i></i></span></span> ...
  <span class="plumedtooltip">ARG<span class="right">the labels of the scalars on which the bias will act<i></i></span></span>=<b name="data/ala2/opes/plumed.datphi">phi</b>,<b name="data/ala2/opes/plumed.datpsi">psi</b>
  <span class="plumedtooltip">PACE<span class="right">the frequency for kernel deposition<i></i></span></span>=500
  <span class="plumedtooltip">BARRIER<span class="right">the free energy barrier to be overcome<i></i></span></span>=30
  <span class="plumedtooltip">NLIST<span class="right"> use neighbor list for kernels summation, faster but experimental<i></i></span></span>
  <span class="plumedtooltip">STATE_WFILE<span class="right">write to this file the compressed kernels and all the info needed to RESTART the simulation<i></i></span></span>=STATE
  <span class="plumedtooltip">STATE_WSTRIDE<span class="right">number of MD steps between writing the STATE_WFILE<i></i></span></span>=500*100
  <span class="plumedtooltip">STORE_STATES<span class="right"> append to STATE_WFILE instead of ovewriting it each time<i></i></span></span>
...
<br/><span style="display:none;" id="data/ala2/opes/plumed.datopes">The OPES_METAD action with label <b>opes</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">opes.bias</td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">opes.rct</td><td>estimate of c(t)</td></tr><tr><td width="5%">opes.zed</td><td>estimate of Z_n</td></tr><tr><td width="5%">opes.neff</td><td>effective sample size</td></tr><tr><td width="5%">opes.nker</td><td>total number of compressed kernels used to represent the bias</td></tr><tr><td width="5%">opes.nlker</td><td>number of kernels in the neighbor list</td></tr><tr><td width="5%">opes.nlsteps</td><td>number of steps from last neighbor list update</td></tr></table></span><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/PRINT" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">FMT<span class="right"> the format that should be used to output real numbers<i></i></span></span>=%g <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=500 <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=COLVAR <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=<b name="data/ala2/opes/plumed.datphi">phi</b>,<b name="data/ala2/opes/plumed.datpsi">psi</b>,<b name="data/ala2/opes/plumed.datopes">opes.*</b>

<span style="display:none;" id="data/ala2/opes/plumed.dat">The PRINT action with label <b></b> calculates something</span><span class="plumedtooltip" style="color:green">ENDPLUMED<span class="right">Terminate plumed input. <a href="https://www.plumed.org/doc-master/user-doc/html/ENDPLUMED" style="color:green">More details</a><i></i></span></span><span style="color:blue" class="comment">

run with:
../queue_gromacs.sh
</span></pre></div>

{% endraw %}
