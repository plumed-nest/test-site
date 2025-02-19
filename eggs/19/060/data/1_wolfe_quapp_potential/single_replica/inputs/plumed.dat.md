**Project ID:** [plumID:19.060]({{ '/' | absolute_url }}eggs/19/060/)  
**Source:** 1_wolfe_quapp_potential/single_replica/inputs/plumed.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/1_wolfe_quapp_potential/single_replica/inputs/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-failed-red.svg" alt="tested onv2.10" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-failed-red.svg" alt="tested onmaster" /></a></td></tr><tr><td style="padding:1px"><img src="https://img.shields.io/badge/with-LOAD-yellow.svg" alt="tested on master" /></td></tr>
</table></div></div>
<pre style="width=97%;">
<span class="plumedtooltip" style="color:blue"># vim:ft=plumed<span class="right">Enables syntax highlighting for PLUMED files in vim. See <a href="https://www.plumed.org/doc-master/user-doc/html/_vim_syntax.html">here for more details. </a><i></i></span></span>
<span class="plumedtooltip" style="color:green">UNITS<span class="right">This command sets the internal units for the code. <a href="https://www.plumed.org/doc-master/user-doc/html/_u_n_i_t_s.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">NATURAL<span class="right"> use natural units<i></i></span></span>
<br/><span style="display:none;" id="data/1_wolfe_quapp_potential/single_replica/inputs/plumed.dat">The UNITS action with label <b></b> calculates something</span><span class="plumedtooltip" style="color:green">LOAD<span class="right">Loads a library, possibly defining new actions. <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">FILE<span class="right">file to be loaded<i></i></span></span>=<b name="data/1_wolfe_quapp_potential/single_replica/inputs/plumed.dat">../../../0_code/NeuralNetworkVes.cpp</b>

<b name="data/1_wolfe_quapp_potential/single_replica/inputs/plumed.datp" onclick='showPath("data/1_wolfe_quapp_potential/single_replica/inputs/plumed.dat","data/1_wolfe_quapp_potential/single_replica/inputs/plumed.datp","data/1_wolfe_quapp_potential/single_replica/inputs/plumed.datp","brown")'>p</b>: <span class="plumedtooltip" style="color:green">POSITION<span class="right">Calculate the components of the position of an atom. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_o_s_i_t_i_o_n.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOM<span class="right">the atom number<i></i></span></span>=1
<span style="display:none;" id="data/1_wolfe_quapp_potential/single_replica/inputs/plumed.datp">The POSITION action with label <b>p</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">p.x</td><td>the x-component of the atom position</td></tr><tr><td width="5%">p.y</td><td>the y-component of the atom position</td></tr><tr><td width="5%">p.z</td><td>the z-component of the atom position</td></tr></table></span><b name="data/1_wolfe_quapp_potential/single_replica/inputs/plumed.datene" onclick='showPath("data/1_wolfe_quapp_potential/single_replica/inputs/plumed.dat","data/1_wolfe_quapp_potential/single_replica/inputs/plumed.datene","data/1_wolfe_quapp_potential/single_replica/inputs/plumed.datene","brown")'>ene</b>: <span class="plumedtooltip" style="color:green">ENERGY<span class="right">Calculate the total potential energy of the simulation box. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_n_e_r_g_y.html" style="color:green">More details</a><i></i></span></span>
<br/><span style="color:blue" class="comment"># nn bias</span>
<span style="display:none;" id="data/1_wolfe_quapp_potential/single_replica/inputs/plumed.datene">The ENERGY action with label <b>ene</b> calculates something</span><span class="plumedtooltip" style="color:green">NN_VES<span class="right">This action is not part of PLUMED and was included by using a LOAD command <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></span></span> ...
LABEL=<b name="data/1_wolfe_quapp_potential/single_replica/inputs/plumed.datnn" onclick='showPath("data/1_wolfe_quapp_potential/single_replica/inputs/plumed.dat","data/1_wolfe_quapp_potential/single_replica/inputs/plumed.datnn","data/1_wolfe_quapp_potential/single_replica/inputs/plumed.datnn","brown")'>nn</b>
ARG=<b name="data/1_wolfe_quapp_potential/single_replica/inputs/plumed.datp">p.x</b>
NODES=48,24,12 
OPTIM=ADAM
ACTIVATION=RELU
GRID_MIN=-3. 
GRID_MAX=3.
GRID_BIN=50 
TEMP=1.
AVE_STRIDE=500 
PRINT_STRIDE=1000 
TARGET_STRIDE=1
GAMMA=10
LRATE=0.001
TAU_KL=50000
DECAY=5000
ADAPTIVE_DECAY=0.5
... NN_VES
<br/><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=500 <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=* <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=COLVAR <span class="plumedtooltip">FMT<span class="right">the format that should be used to output real numbers<i></i></span></span>=%10.8f
</pre>
{% endraw %}
