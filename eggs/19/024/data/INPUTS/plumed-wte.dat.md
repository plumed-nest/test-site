**Project ID:** [plumID:19.024]({{ '/' | absolute_url }}eggs/19/024/)  
**Source:** INPUTS/plumed-wte.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [zipped raw stdout](plumed-wte.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed-wte.dat.plumed.stderr.txt.zip) - [stderr](plumed-wte.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed-wte.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed-wte.dat.plumed_master.stderr.txt.zip) - [stderr](plumed-wte.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/INPUTS/plumed-wte.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed-wte.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed-wte.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue"># CV definition</span>
<b name="data/INPUTS/plumed-wte.datene" onclick='showPath("data/INPUTS/plumed-wte.dat","data/INPUTS/plumed-wte.datene")'>ene</b>: <div class="tooltip" style="color:green">ENERGY<div class="right">Calculate the total potential energy of the simulation box. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_n_e_r_g_y.html" style="color:green">More details</a><i></i></div></div>
<br/><span style="color:blue"># MetaD parameters</span>
<div class="tooltip" style="color:green">METAD<div class="right">Used to performed metadynamics on one or more collective variables. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_e_t_a_d.html" style="color:green">More details</a><i></i></div></div> ...
  <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/INPUTS/plumed-wte.datene">ene</b> <div class="tooltip">SIGMA<div class="right">the widths of the Gaussian hills<i></i></div></div>=500 <div class="tooltip">HEIGHT<div class="right">the heights of the Gaussian hills<i></i></div></div>=2.0 <div class="tooltip">PACE<div class="right">the frequency for hill addition<i></i></div></div>=125
  <div class="tooltip">TEMP<div class="right">the system temperature - this is only needed if you are doing well-tempered metadynamics<i></i></div></div>=300 <div class="tooltip">BIASFACTOR<div class="right">use well tempered metadynamics and use this bias factor<i></i></div></div>=24 <div class="tooltip">FILE<div class="right"> a file in which the list of added hills is stored<i></i></div></div>=HILLS
  <div class="tooltip">GRID_MIN<div class="right">the lower bounds for the grid<i></i></div></div>=-175000 <div class="tooltip">GRID_MAX<div class="right">the upper bounds for the grid<i></i></div></div>=-75000 <div class="tooltip">GRID_BIN<div class="right">the number of bins for the grid<i></i></div></div>=500 
  <div class="tooltip">GRID_WSTRIDE<div class="right">write the grid to a file every N steps<i></i></div></div>=500000 <div class="tooltip">GRID_WFILE<div class="right">the file on which to write the grid<i></i></div></div>=BIAS
... METAD
</pre>
{% endraw %}
