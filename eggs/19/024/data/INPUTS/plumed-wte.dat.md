**Project ID:** [plumID:19.024]({{ '/' | absolute_url }}eggs/19/024/)  
**Source:** INPUTS/plumed-wte.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [zipped raw stdout](plumed-wte.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed-wte.dat.plumed.stderr.txt.zip) - [stderr](plumed-wte.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed-wte.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed-wte.dat.plumed_master.stderr.txt.zip) - [stderr](plumed-wte.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/INPUTS/plumed-wte.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed-wte.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-passing-green.svg" alt="tested onv2.10" /></a></td></tr><tr><td style="padding:1px"><a href="plumed-wte.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue" class="comment"># CV definition</span>
<b name="data/INPUTS/plumed-wte.datene" onclick='showPath("data/INPUTS/plumed-wte.dat","data/INPUTS/plumed-wte.datene","data/INPUTS/plumed-wte.datene","black")'>ene</b><span style="display:none;" id="data/INPUTS/plumed-wte.datene">The ENERGY action with label <b>ene</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ene</td><td width="5%"><font color="black">scalar</font></td><td>the internal energy</td></tr></table></span>: <span class="plumedtooltip" style="color:green">ENERGY<span class="right">Calculate the total potential energy of the simulation box. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_n_e_r_g_y.html" style="color:green">More details</a><i></i></span></span>
<br/><span style="color:blue" class="comment"># MetaD parameters</span>
<span class="plumedtooltip" style="color:green">METAD<span class="right">Used to performed metadynamics on one or more collective variables. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_e_t_a_d.html" style="color:green">More details</a><i></i></span></span> ...
  <span class="plumedtooltip">ARG<span class="right">the labels of the scalars on which the bias will act<i></i></span></span>=<b name="data/INPUTS/plumed-wte.datene">ene</b> <span class="plumedtooltip">SIGMA<span class="right">the widths of the Gaussian hills<i></i></span></span>=500 <span class="plumedtooltip">HEIGHT<span class="right">the heights of the Gaussian hills<i></i></span></span>=2.0 <span class="plumedtooltip">PACE<span class="right">the frequency for hill addition<i></i></span></span>=125
  <span class="plumedtooltip">TEMP<span class="right">the system temperature - this is only needed if you are doing well-tempered metadynamics<i></i></span></span>=300 <span class="plumedtooltip">BIASFACTOR<span class="right">use well tempered metadynamics and use this bias factor<i></i></span></span>=24 <span class="plumedtooltip">FILE<span class="right"> a file in which the list of added hills is stored<i></i></span></span>=HILLS
  <span class="plumedtooltip">GRID_MIN<span class="right">the lower bounds for the grid<i></i></span></span>=-175000 <span class="plumedtooltip">GRID_MAX<span class="right">the upper bounds for the grid<i></i></span></span>=-75000 <span class="plumedtooltip">GRID_BIN<span class="right">the number of bins for the grid<i></i></span></span>=500 
  <span class="plumedtooltip">GRID_WSTRIDE<span class="right">write the grid to a file every N steps<i></i></span></span>=500000 <span class="plumedtooltip">GRID_WFILE<span class="right">the file on which to write the grid<i></i></span></span>=BIAS
... METAD
</pre>
{% endraw %}
