**Project ID:** [plumID:19.081]({{ '/' | absolute_url }}eggs/19/081/)  
**Source:** Na/01_Distributions/Solid/plumed.dat  
**Originally used with PLUMED version:** 2.6-dev  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/Na/01_Distributions/Solid/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-failed-red.svg" alt="tested onv2.10" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-failed-red.svg" alt="tested onmaster" /></a></td></tr><tr><td style="padding:1px"><img src="https://img.shields.io/badge/with-LOAD-yellow.svg" alt="tested on master" /></td></tr>
</table></div></div>
<pre style="width=97%;">
<span class="plumedtooltip" style="color:blue"># vim:ft=plumed<span class="right">Enables syntax highlighting for PLUMED files in vim. See <a href="https://www.plumed.org/doc-master/user-doc/html/_vim_syntax.html">here for more details. </a><i></i></span></span>
<br/><span class="plumedtooltip" style="color:green">RESTART<span class="right">Activate restart. <a href="https://www.plumed.org/doc-master/user-doc/html/_r_e_s_t_a_r_t.html" style="color:green">More details</a><i></i></span></span>
<br/><span style="display:none;" id="data/Na/01_Distributions/Solid/plumed.dat">The RESTART action with label <b></b> calculates something</span><span class="plumedtooltip" style="color:green">LOAD<span class="right">Loads a library, possibly defining new actions. <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">FILE<span class="right">file to be loaded<i></i></span></span>=<b name="data/Na/01_Distributions/Solid/plumed.dat">../../../RefCV.cpp</b>

<b name="data/Na/01_Distributions/Solid/plumed.datenergy" onclick='showPath("data/Na/01_Distributions/Solid/plumed.dat","data/Na/01_Distributions/Solid/plumed.datenergy","data/Na/01_Distributions/Solid/plumed.datenergy","brown")'>energy</b>: <span class="plumedtooltip" style="color:green">ENERGY<span class="right">Calculate the total potential energy of the simulation box. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_n_e_r_g_y.html" style="color:green">More details</a><i></i></span></span>
<br/><span style="display:none;" id="data/Na/01_Distributions/Solid/plumed.datenergy">The ENERGY action with label <b>energy</b> calculates something</span><b name="data/Na/01_Distributions/Solid/plumed.datvol" onclick='showPath("data/Na/01_Distributions/Solid/plumed.dat","data/Na/01_Distributions/Solid/plumed.datvol","data/Na/01_Distributions/Solid/plumed.datvol","brown")'>vol</b>: <span class="plumedtooltip" style="color:green">VOLUME<span class="right">Calculate the volume of the simulation box. <a href="https://www.plumed.org/doc-master/user-doc/html/_v_o_l_u_m_e.html" style="color:green">More details</a><i></i></span></span>
<br/><span style="display:none;" id="data/Na/01_Distributions/Solid/plumed.datvol">The VOLUME action with label <b>vol</b> calculates the volume of simulation box</span><span class="plumedtooltip" style="color:green">REFCV<span class="right">This action is not part of PLUMED and was included by using a LOAD command <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></span></span> ...
 SPECIES=1-250
 SIGMA=0.065
 LATTICE_CONSTANTS=0.432
 CRYSTAL_STRUCTURE=BCC
 LABEL=<b name="data/Na/01_Distributions/Solid/plumed.datrefcv" onclick='showPath("data/Na/01_Distributions/Solid/plumed.dat","data/Na/01_Distributions/Solid/plumed.datrefcv","data/Na/01_Distributions/Solid/plumed.datrefcv","brown")'>refcv</b>
 MORE_THAN={RATIONAL R_0=0.5 NN=12 MM=24}
 MEAN
... REFCV
<br/><span class="plumedtooltip" style="color:green">HISTOGRAM<span class="right">Accumulate the average probability density along a few CVs from a trajectory. <a href="https://www.plumed.org/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html" style="color:green">More details</a><i></i></span></span> ...
  <span class="plumedtooltip">DATA<span class="right">an alternative to the ARG keyword<i></i></span></span>=refcv
  <span class="plumedtooltip">GRID_MIN<span class="right"> the lower bounds for the grid<i></i></span></span>=-1.5
  <span class="plumedtooltip">GRID_MAX<span class="right"> the upper bounds for the grid<i></i></span></span>=1.5
  <span class="plumedtooltip">GRID_BIN<span class="right">the number of bins for the grid<i></i></span></span>=1000
  <span class="plumedtooltip">BANDWIDTH<span class="right">the bandwidths for kernel density esimtation<i></i></span></span>=0.05
  <span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/Na/01_Distributions/Solid/plumed.dathh" onclick='showPath("data/Na/01_Distributions/Solid/plumed.dat","data/Na/01_Distributions/Solid/plumed.dathh","data/Na/01_Distributions/Solid/plumed.dathh","brown")'>hh</b>
  <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which to store data for averaging<i></i></span></span>=10
... HISTOGRAM
<br/><span style="display:none;" id="data/Na/01_Distributions/Solid/plumed.dathh">The HISTOGRAM action with label <b>hh</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">hh.value</td><td>the estimate of the histogram as a function of the argument that was obtained</td></tr></table></span><span class="plumedtooltip" style="color:green">DUMPGRID<span class="right">Output the function on the grid to a file with the PLUMED grid format. <a href="https://www.plumed.org/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">GRID<span class="right">the grid you would like to print (can also use ARG for specifying what is being printed)<i></i></span></span>=<b name="data/Na/01_Distributions/Solid/plumed.dathh">hh</b> <span class="plumedtooltip">FILE<span class="right"> the file on which to write the grid<i></i></span></span>=histo <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the grid should be output to the file<i></i></span></span>=5000

<span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=* <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=COLVAR <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=500
</pre>
{% endraw %}
