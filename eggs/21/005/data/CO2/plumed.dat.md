**Project ID:** [plumID:21.005]({{ '/' | absolute_url }}eggs/21/005/)  
**Source:** CO2/plumed.dat  
**Originally used with PLUMED version:** 2.7-mod  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/CO2/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-failed-red.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-failed-red.svg" alt="tested onmaster" /></a></td></tr><tr><td style="padding:1px"><img src="https://img.shields.io/badge/with-LOAD-yellow.svg" alt="tested on master" /></td></tr>
</table></div></div>
<pre style="width=97%;">
<div class="tooltip" style="color:blue"># vim:ft=plumed<div class="right">Enables syntax highlighting for PLUMED files in vim. See <a href="https://www.plumed.org/doc-master/user-doc/html/_vim_syntax.html">here for more details. </a><i></i></div></div>
<div class="tooltip" style="color:green">LOAD<div class="right">Loads a library, possibly defining new actions. <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">FILE<div class="right">file to be loaded<i></i></div></div>=../codes/StructureFactor_descriptor.test.cpp
<span style="color:blue" class="comment">#RESTART</span>
<br/><span style="display:none;" id="data/CO2/plumed.dat">The LOAD action with label <b></b> calculates something</span><div class="tooltip" style="color:green">GROUP<div class="right">Define a group of atoms so that a particular list of atoms can be referenced with a single label in definitions of CVs or virtual atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_g_r_o_u_p.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the numerical indexes for the set of atoms in the group<i></i></div></div>=1-324:3 <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/CO2/plumed.datC" onclick='showPath("data/CO2/plumed.dat","data/CO2/plumed.datC","data/CO2/plumed.datC","brown")'>C</b>
<span style="display:none;" id="data/CO2/plumed.datC">The GROUP action with label <b>C</b> calculates something</span><div class="tooltip" style="color:green">GROUP<div class="right">Define a group of atoms so that a particular list of atoms can be referenced with a single label in definitions of CVs or virtual atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_g_r_o_u_p.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the numerical indexes for the set of atoms in the group<i></i></div></div>=2-324:3,3-324:3 <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/CO2/plumed.datO" onclick='showPath("data/CO2/plumed.dat","data/CO2/plumed.datO","data/CO2/plumed.datO","brown")'>O</b>
<br/><span style="display:none;" id="data/CO2/plumed.datO">The GROUP action with label <b>O</b> calculates something</span><b name="data/CO2/plumed.datso" onclick='showPath("data/CO2/plumed.dat","data/CO2/plumed.datso","data/CO2/plumed.datso","brown")'>so</b>: <div class="tooltip" style="color:green">STRUCTURE_FACTOR_DESCRIPTOR_TEST<div class="right">This action is not part of PLUMED and was included by using a LOAD command <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></div></div> ACTIVE_SHELLS=27,45,54,117,126,144 ATOMS=<b name="data/CO2/plumed.datO">O</b> 
<br/><b name="data/CO2/plumed.datauto1" onclick='showPath("data/CO2/plumed.dat","data/CO2/plumed.datauto1","data/CO2/plumed.datauto1","brown")'>auto1</b>: <div class="tooltip" style="color:green">PYTORCH_MODEL<div class="right">Load a PyTorch model compiled with TorchScript. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_y_t_o_r_c_h__m_o_d_e_l.html" style="color:green">More details</a><i></i></div></div> MODEL=co2_333_sfO_tc1.pt <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=so.Sk3_-3_-3,so.Sk3_-3_3,so.Sk3_3_-3,so.Sk3_3_3,so.Sk0_3_-6,so.Sk0_3_6,so.Sk0_6_-3,so.Sk0_6_3,so.Sk3_-6_0,so.Sk3_0_-6,so.Sk3_0_6,so.Sk3_6_0,so.Sk6_-3_0,so.Sk6_0_-3,so.Sk6_0_3,so.Sk6_3_0,so.Sk3_-6_-3,so.Sk3_-6_3,so.Sk3_-3_-6,so.Sk3_-3_6,so.Sk3_3_-6,so.Sk3_3_6,so.Sk3_6_-3,so.Sk3_6_3,so.Sk6_-3_-3,so.Sk6_-3_3,so.Sk6_3_-3,so.Sk6_3_3,so.Sk0_6_-9,so.Sk0_6_9,so.Sk0_9_-6,so.Sk0_9_6,so.Sk6_-9_0,so.Sk6_0_-9,so.Sk6_0_9,so.Sk6_9_0,so.Sk9_-6_0,so.Sk9_0_-6,so.Sk9_0_6,so.Sk9_6_0,so.Sk3_-9_-6,so.Sk3_-9_6,so.Sk3_-6_-9,so.Sk3_-6_9,so.Sk3_6_-9,so.Sk3_6_9,so.Sk3_9_-6,so.Sk3_9_6,so.Sk6_-9_-3,so.Sk6_-9_3,so.Sk6_-3_-9,so.Sk6_-3_9,so.Sk6_3_-9,so.Sk6_3_9,so.Sk6_9_-3,so.Sk6_9_3,so.Sk9_-6_-3,so.Sk9_-6_3,so.Sk9_-3_-6,so.Sk9_-3_6,so.Sk9_3_-6,so.Sk9_3_6,so.Sk9_6_-3,so.Sk9_6_3,so.Sk0_0_12,so.Sk0_12_0,so.Sk12_0_0
<span style="display:none;" id="data/CO2/plumed.datauto1">The PYTORCH_MODEL action with label <b>auto1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">auto1.node</td><td>Model outputs</td></tr></table></span><b name="data/CO2/plumed.datNNcube1" onclick='showPath("data/CO2/plumed.dat","data/CO2/plumed.datNNcube1","data/CO2/plumed.datNNcube1","brown")'>NNcube1</b>: <div class="tooltip" style="color:green">MATHEVAL<div class="right">An alias to the CUSTOM function that can also be used to calaculate combinations of variables using a custom expression. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input to this function<i></i></div></div>=<b name="data/CO2/plumed.datauto1">auto1.node-0</b> <div class="tooltip">FUNC<div class="right">the function you wish to evaluate<i></i></div></div>=x+x^3 <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO
<br/><span style="display:none;" id="data/CO2/plumed.datNNcube1">The MATHEVAL action with label <b>NNcube1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">NNcube1.value</td><td>an arbitrary function</td></tr></table></span><div class="tooltip" style="color:green">OPES_METAD<div class="right">On-the-fly probability enhanced sampling with metadynamics-like target distribution. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s__m_e_t_a_d.html" style="color:green">More details</a><i></i></div></div> ...
  <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/CO2/plumed.datopes" onclick='showPath("data/CO2/plumed.dat","data/CO2/plumed.datopes","data/CO2/plumed.datopes","brown")'>opes</b>
  <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/CO2/plumed.datNNcube1">NNcube1</b>
  <div class="tooltip">PACE<div class="right">the frequency for kernel deposition<i></i></div></div>=500
  <div class="tooltip">BARRIER<div class="right">the free energy barrier to be overcome<i></i></div></div>=200
  <div class="tooltip">FILE<div class="right"> a file in which the list of all deposited kernels is stored<i></i></div></div>=Kernels.data
  <div class="tooltip">STATE_RFILE<div class="right">read from this file the compressed kernels and all the info needed to RESTART the simulation<i></i></div></div>=compressed_KernelsR.data
  <div class="tooltip">STATE_WFILE<div class="right">write to this file the compressed kernels and all the info needed to RESTART the simulation<i></i></div></div>=compressed_KernelsW.data
  <div class="tooltip">STATE_WSTRIDE<div class="right">number of MD steps between writing the STATE_WFILE<i></i></div></div>=10000 
  <div class="tooltip">NLIST<div class="right"> use neighbor list for kernels summation, faster but experimental<i></i></div></div>
...

<br/><span style="display:none;" id="data/CO2/plumed.datopes">The OPES_METAD action with label <b>opes</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">opes.bias</td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">opes.rct</td><td>estimate of c(t)</td></tr><tr><td width="5%">opes.zed</td><td>estimate of Z_n</td></tr><tr><td width="5%">opes.neff</td><td>effective sample size</td></tr><tr><td width="5%">opes.nker</td><td>total number of compressed kernels used to represent the bias</td></tr><tr><td width="5%">opes.nlker</td><td>number of kernels in the neighbor list</td></tr><tr><td width="5%">opes.nlsteps</td><td>number of steps from last neighbor list update</td></tr></table></span><b name="data/CO2/plumed.datuwall" onclick='showPath("data/CO2/plumed.dat","data/CO2/plumed.datuwall","data/CO2/plumed.datuwall","brown")'>uwall</b>: <div class="tooltip" style="color:green">UPPER_WALLS<div class="right">Defines a wall for the value of one or more collective variables, <a href="https://www.plumed.org/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the arguments on which the bias is acting<i></i></div></div>=<b name="data/CO2/plumed.datNNcube1">NNcube1</b> <div class="tooltip">AT<div class="right">the positions of the wall<i></i></div></div>=2.9 <div class="tooltip">KAPPA<div class="right">the force constant for the wall<i></i></div></div>=10000
<span style="display:none;" id="data/CO2/plumed.datuwall">The UPPER_WALLS action with label <b>uwall</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">uwall.bias</td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">uwall.force2</td><td>the instantaneous value of the squared force due to this bias potential</td></tr></table></span><b name="data/CO2/plumed.datlwall" onclick='showPath("data/CO2/plumed.dat","data/CO2/plumed.datlwall","data/CO2/plumed.datlwall","brown")'>lwall</b>: <div class="tooltip" style="color:green">LOWER_WALLS<div class="right">Defines a wall for the value of one or more collective variables, <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the arguments on which the bias is acting<i></i></div></div>=<b name="data/CO2/plumed.datNNcube1">NNcube1</b> <div class="tooltip">AT<div class="right">the positions of the wall<i></i></div></div>=-2.9 <div class="tooltip">KAPPA<div class="right">the force constant for the wall<i></i></div></div>=10000
<br/><span style="display:none;" id="data/CO2/plumed.datlwall">The LOWER_WALLS action with label <b>lwall</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">lwall.bias</td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">lwall.force2</td><td>the instantaneous value of the squared force due to this bias potential</td></tr></table></span><div class="tooltip" style="color:green">FLUSH<div class="right">This command instructs plumed to flush all the open files with a user specified frequency. <a href="https://www.plumed.org/doc-master/user-doc/html/_f_l_u_s_h.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">STRIDE<div class="right">the frequency with which all the open files should be flushed<i></i></div></div>=500
<div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">FMT<div class="right">the format that should be used to output real numbers<i></i></div></div>=%g <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=500 <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=COLVAR-comps <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=so.Sk3_-3_-3,so.Sk3_-3_3,so.Sk3_3_-3,so.Sk3_3_3,so.Sk0_3_-6,so.Sk0_3_6,so.Sk0_6_-3,so.Sk0_6_3,so.Sk3_-6_0,so.Sk3_0_-6,so.Sk3_0_6,so.Sk3_6_0,so.Sk6_-3_0,so.Sk6_0_-3,so.Sk6_0_3,so.Sk6_3_0,so.Sk3_-6_-3,so.Sk3_-6_3,so.Sk3_-3_-6,so.Sk3_-3_6,so.Sk3_3_-6,so.Sk3_3_6,so.Sk3_6_-3,so.Sk3_6_3,so.Sk6_-3_-3,so.Sk6_-3_3,so.Sk6_3_-3,so.Sk6_3_3,so.Sk0_6_-9,so.Sk0_6_9,so.Sk0_9_-6,so.Sk0_9_6,so.Sk6_-9_0,so.Sk6_0_-9,so.Sk6_0_9,so.Sk6_9_0,so.Sk9_-6_0,so.Sk9_0_-6,so.Sk9_0_6,so.Sk9_6_0,so.Sk3_-9_-6,so.Sk3_-9_6,so.Sk3_-6_-9,so.Sk3_-6_9,so.Sk3_6_-9,so.Sk3_6_9,so.Sk3_9_-6,so.Sk3_9_6,so.Sk6_-9_-3,so.Sk6_-9_3,so.Sk6_-3_-9,so.Sk6_-3_9,so.Sk6_3_-9,so.Sk6_3_9,so.Sk6_9_-3,so.Sk6_9_3,so.Sk9_-6_-3,so.Sk9_-6_3,so.Sk9_-3_-6,so.Sk9_-3_6,so.Sk9_3_-6,so.Sk9_3_6,so.Sk9_6_-3,so.Sk9_6_3,so.Sk0_0_12,so.Sk0_12_0,so.Sk12_0_0
<div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">FMT<div class="right">the format that should be used to output real numbers<i></i></div></div>=%g <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=500 <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=COLVAR <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/CO2/plumed.datNNcube1">NNcube1</b>,<b name="data/CO2/plumed.datopes">opes.*</b>,<b name="data/CO2/plumed.datuwall">uwall.*</b>,<b name="data/CO2/plumed.datlwall">lwall</b>
</pre>
{% endraw %}