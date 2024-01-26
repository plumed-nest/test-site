**Project ID:** [plumID:19.081]({{ '/' | absolute_url }}eggs/19/081/)  
**Source:** Na/01_Distributions/Liquid/plumed.dat  
**Originally used with PLUMED version:** 2.6-dev  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/Na/01_Distributions/Liquid/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr><tr><td style="padding:1px"><img src="https://img.shields.io/badge/with-LOAD-yellow.svg" alt="tested on master" /></td></tr>
</table></div></div>
<pre style="width=97%;">
<div class="tooltip" style="color:blue"># vim:ft=plumed<div class="right">Enables syntax highlighting for PLUMED files in vim. See <a href="https://www.plumed.org/doc-master/user-doc/html/_vim_syntax.html">here for more details. </a><i></i></div></div>
<br/><div class="tooltip" style="color:green">RESTART<div class="right">Activate restart. <a href="https://www.plumed.org/doc-master/user-doc/html/_r_e_s_t_a_r_t.html" style="color:green">More details</a><i></i></div></div>
<br/><div class="tooltip" style="color:green">LOAD<div class="right">Loads a library, possibly defining new actions. <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">FILE<div class="right">file to be loaded<i></i></div></div>=../../../RefCV.cpp
<br/><b name="data/Na/01_Distributions/Liquid/plumed.datenergy" onclick='showPath("data/Na/01_Distributions/Liquid/plumed.dat","data/Na/01_Distributions/Liquid/plumed.datenergy")'>energy</b>: <div class="tooltip" style="color:green">ENERGY<div class="right">Calculate the total potential energy of the simulation box. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_n_e_r_g_y.html" style="color:green">More details</a><i></i></div></div>
<br/><b name="data/Na/01_Distributions/Liquid/plumed.datvol" onclick='showPath("data/Na/01_Distributions/Liquid/plumed.dat","data/Na/01_Distributions/Liquid/plumed.datvol")'>vol</b>: <div class="tooltip" style="color:green">VOLUME<div class="right">Calculate the volume of the simulation box. <a href="https://www.plumed.org/doc-master/user-doc/html/_v_o_l_u_m_e.html" style="color:green">More details</a><i></i></div></div>
<br/><span style="display:none;" id="data/Na/01_Distributions/Liquid/plumed.datvol">The VOLUME action with label <b>vol</b> calculates a scalar quantity</span><div class="tooltip" style="color:green">REFCV<div class="right">This action is not part of PLUMED and was included by using a LOAD command <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></div></div> ...
 SPECIES=1-250
 SIGMA=0.065
 LATTICE_CONSTANTS=0.432
 CRYSTAL_STRUCTURE=BCC
 LABEL=<b name="data/Na/01_Distributions/Liquid/plumed.datrefcv" onclick='showPath("data/Na/01_Distributions/Liquid/plumed.dat","data/Na/01_Distributions/Liquid/plumed.datrefcv")'>refcv</b>
 MORE_THAN={RATIONAL R_0=0.5 NN=12 MM=24}
 MEAN
... REFCV
<br/><div class="tooltip" style="color:green">HISTOGRAM<div class="right">Accumulate the average probability density along a few CVs from a trajectory. <a href="https://www.plumed.org/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html" style="color:green">More details</a><i></i></div></div> ...
  <div class="tooltip">DATA<div class="right">input data from action with vessel and compute histogram<i></i></div></div>=<b name="data/Na/01_Distributions/Liquid/plumed.datrefcv">refcv</b>
  <div class="tooltip">GRID_MIN<div class="right">the lower bounds for the grid<i></i></div></div>=-1.5
  <div class="tooltip">GRID_MAX<div class="right">the upper bounds for the grid<i></i></div></div>=1.5
  <div class="tooltip">GRID_BIN<div class="right">the number of bins for the grid<i></i></div></div>=1000
  <div class="tooltip">BANDWIDTH<div class="right">the bandwidths for kernel density estimation<i></i></div></div>=0.05
  <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/Na/01_Distributions/Liquid/plumed.dathh" onclick='showPath("data/Na/01_Distributions/Liquid/plumed.dat","data/Na/01_Distributions/Liquid/plumed.dathh")'>hh</b>
  <div class="tooltip">STRIDE<div class="right"> the frequency with which the data should be collected and added to the quantity being averaged<i></i></div></div>=10
... HISTOGRAM
<br/><span style="display:none;" id="data/Na/01_Distributions/Liquid/plumed.dathh">The HISTOGRAM action with label <b>hh</b> calculates a scalar quantity</span><div class="tooltip" style="color:green">DUMPGRID<div class="right">Output the function on the grid to a file with the PLUMED grid format. <a href="https://www.plumed.org/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">GRID<div class="right">the action that creates the grid you would like to output<i></i></div></div>=<b name="data/Na/01_Distributions/Liquid/plumed.dathh">hh</b> <div class="tooltip">FILE<div class="right"> the file on which to write the grid<i></i></div></div>=histo <div class="tooltip">STRIDE<div class="right"> the frequency with which the grid should be output to the file<i></i></div></div>=5000
<br/><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div> <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=COLVAR <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=500
</pre>
{% endraw %}
