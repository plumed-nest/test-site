**Project ID:** [plumID:19.068]({{ '/' | absolute_url }}eggs/19/068/)  
**Source:** model/opes-model/plumed.dat  
**Originally used with PLUMED version:** 2.7  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div class="plumedInputContainer">
<div class="plumedpreheader">
<div class="headerInfo" id="value_details_data/model/opes-model/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div class="containerBadge">
<div class="headerBadge"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-passing-green.svg" alt="tested onv2.10" /></a></div>
<div class="headerBadge"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></div>
</div>
</div>
<pre class="plumedlisting">
<span class="plumedtooltip" style="color:blue"># vim:ft=plumed<span class="right">Enables syntax highlighting for PLUMED files in vim. See <a href="https://www.plumed.org/doc-master/user-doc/html/vim">here for more details. </a><i></i></span></span>
<span class="plumedtooltip" style="color:green">UNITS<span class="right">This command sets the internal units for the code. <a href="https://www.plumed.org/doc-master/user-doc/html/UNITS" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">NATURAL<span class="right"> use natural units<i></i></span></span>
<br/><span style="display:none;" id="data/model/opes-model/plumed.dat">The UNITS action with label <b></b> calculates something</span><b name="data/model/opes-model/plumed.datp" onclick='showPath("data/model/opes-model/plumed.dat","data/model/opes-model/plumed.datp","data/model/opes-model/plumed.datp","brown")'>p</b>: <span class="plumedtooltip" style="color:green">POSITION<span class="right">Calculate the components of the position of an atom or atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/POSITION" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOM<span class="right">the atom number<i></i></span></span>=1

<span style="display:none;" id="data/model/opes-model/plumed.datp">The POSITION action with label <b>p</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">p.x</td><td>the x-component of the atom position</td></tr><tr><td width="5%">p.y</td><td>the y-component of the atom position</td></tr><tr><td width="5%">p.z</td><td>the z-component of the atom position</td></tr></table></span><b name="data/model/opes-model/plumed.datopes" onclick='showPath("data/model/opes-model/plumed.dat","data/model/opes-model/plumed.datopes","data/model/opes-model/plumed.datopes","brown")'>opes</b>: <span class="plumedtooltip" style="color:green">OPES_METAD<span class="right">On-the-fly probability enhanced sampling with metadynamics-like target distribution. <a href="https://www.plumed.org/doc-master/user-doc/html/OPES_METAD" style="color:green">More details</a><i></i></span></span> ...
  <span class="plumedtooltip">ARG<span class="right">the labels of the scalars on which the bias will act<i></i></span></span>=<b name="data/model/opes-model/plumed.datp">p.x</b>
  <span class="plumedtooltip">FILE<span class="right"> a file in which the list of all deposited kernels is stored<i></i></span></span>=Kernels.data
  <span class="plumedtooltip">PACE<span class="right">the frequency for kernel deposition<i></i></span></span>=500
  <span class="plumedtooltip">SIGMA<span class="right"> the initial widths of the kernels<i></i></span></span>=0.185815
  <span class="plumedtooltip">BARRIER<span class="right">the free energy barrier to be overcome<i></i></span></span>=10
...
<br/><span style="display:none;" id="data/model/opes-model/plumed.datopes">The OPES_METAD action with label <b>opes</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">opes.bias</td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">opes.rct</td><td>estimate of c(t)</td></tr><tr><td width="5%">opes.zed</td><td>estimate of Z_n</td></tr><tr><td width="5%">opes.neff</td><td>effective sample size</td></tr><tr><td width="5%">opes.nker</td><td>total number of compressed kernels used to represent the bias</td></tr></table></span><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/PRINT" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">FMT<span class="right"> the format that should be used to output real numbers<i></i></span></span>=%g <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=500 <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=Colvar.data <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=<b name="data/model/opes-model/plumed.datp">p.x</b>,<b name="data/model/opes-model/plumed.datp">p.y</b>,<b name="data/model/opes-model/plumed.datopes">opes.*</b>

<span class="plumedtooltip" style="color:green">ENDPLUMED<span class="right">Terminate plumed input. <a href="https://www.plumed.org/doc-master/user-doc/html/ENDPLUMED" style="color:green">More details</a><i></i></span></span><span style="color:blue" class="comment">
</span></pre></div>

{% endraw %}
