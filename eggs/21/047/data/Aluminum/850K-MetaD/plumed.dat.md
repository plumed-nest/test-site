**Project ID:** [plumID:21.047]({{ '/' | absolute_url }}eggs/21/047/)  
**Source:** Aluminum/850K-MetaD/plumed.dat  
**Originally used with PLUMED version:** 2.8  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/Aluminum/850K-MetaD/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr><tr><td style="padding:1px"><img src="https://img.shields.io/badge/with-LOAD-yellow.svg" alt="tested on master" /></td></tr>
</table></div></div>
<pre style="width=97%;">
<div class="tooltip" style="color:green">RESTART<div class="right">Activate restart. <a href="https://www.plumed.org/doc-master/user-doc/html/_r_e_s_t_a_r_t.html" style="color:green">More details</a><i></i></div></div>
<br/><div class="tooltip" style="color:green">LOAD<div class="right">Loads a library, possibly defining new actions. <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">FILE<div class="right">file to be loaded<i></i></div></div>=../../PairEntropy.cpp
<br/><div class="tooltip" style="color:green">PAIRENTROPY<div class="right">This action is not part of PLUMED and was included by using a LOAD command <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></div></div> ...
 LABEL=<b name="data/Aluminum/850K-MetaD/plumed.dats2" onclick='showPath("data/Aluminum/850K-MetaD/plumed.dat","data/Aluminum/850K-MetaD/plumed.dats2")'>s2</b>
 ATOMS=1-256
 MAXR=0.7
 SIGMA=0.0125
... PAIRENTROPY
<br/><div class="tooltip" style="color:green">ENERGY<div class="right">Calculate the total potential energy of the simulation box. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_n_e_r_g_y.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/Aluminum/850K-MetaD/plumed.datene" onclick='showPath("data/Aluminum/850K-MetaD/plumed.dat","data/Aluminum/850K-MetaD/plumed.datene")'>ene</b>
<br/><div class="tooltip" style="color:green">VOLUME<div class="right">Calculate the volume of the simulation box. <a href="https://www.plumed.org/doc-master/user-doc/html/_v_o_l_u_m_e.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/Aluminum/850K-MetaD/plumed.datvol" onclick='showPath("data/Aluminum/850K-MetaD/plumed.dat","data/Aluminum/850K-MetaD/plumed.datvol")'>vol</b>
<br/><span style="display:none;" id="data/Aluminum/850K-MetaD/plumed.datvol">The VOLUME action with label <b>vol</b> calculates a scalar quantity</span><div class="tooltip" style="color:green">COMBINE<div class="right">Calculate a polynomial combination of a set of other variables. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_m_b_i_n_e.html" style="color:green">More details</a><i></i></div></div> ...
 <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/Aluminum/850K-MetaD/plumed.datene">ene</b>,<b name="data/Aluminum/850K-MetaD/plumed.datvol">vol</b>
 <div class="tooltip">POWERS<div class="right"> the powers to which you are raising each of the arguments in your function<i></i></div></div>=1,1
 <div class="tooltip">COEFFICIENTS<div class="right"> the coefficients of the arguments in your function<i></i></div></div>=1.,0.060221409
 <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO
 <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/Aluminum/850K-MetaD/plumed.datenthalpy" onclick='showPath("data/Aluminum/850K-MetaD/plumed.dat","data/Aluminum/850K-MetaD/plumed.datenthalpy")'>enthalpy</b>
... COMBINE
<br/><span style="display:none;" id="data/Aluminum/850K-MetaD/plumed.datenthalpy">The COMBINE action with label <b>enthalpy</b> calculates a scalar quantity</span><div class="tooltip" style="color:green">COMBINE<div class="right">Calculate a polynomial combination of a set of other variables. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_m_b_i_n_e.html" style="color:green">More details</a><i></i></div></div> ...
 <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/Aluminum/850K-MetaD/plumed.datenthalpy">enthalpy</b>
 <div class="tooltip">POWERS<div class="right"> the powers to which you are raising each of the arguments in your function<i></i></div></div>=1
 <div class="tooltip">COEFFICIENTS<div class="right"> the coefficients of the arguments in your function<i></i></div></div>=0.00390625
 <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO
 <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/Aluminum/850K-MetaD/plumed.datenthalpyPerAtom" onclick='showPath("data/Aluminum/850K-MetaD/plumed.dat","data/Aluminum/850K-MetaD/plumed.datenthalpyPerAtom")'>enthalpyPerAtom</b>
... COMBINE
<br/><span style="display:none;" id="data/Aluminum/850K-MetaD/plumed.datenthalpyPerAtom">The COMBINE action with label <b>enthalpyPerAtom</b> calculates a scalar quantity</span><div class="tooltip" style="color:green">METAD<div class="right">Used to performed metadynamics on one or more collective variables. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_e_t_a_d.html" style="color:green">More details</a><i></i></div></div> ...
 <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/Aluminum/850K-MetaD/plumed.datmetad" onclick='showPath("data/Aluminum/850K-MetaD/plumed.dat","data/Aluminum/850K-MetaD/plumed.datmetad")'>metad</b>
 <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/Aluminum/850K-MetaD/plumed.datenthalpyPerAtom">enthalpyPerAtom</b>,<b name="data/Aluminum/850K-MetaD/plumed.dats2">s2</b>
 <div class="tooltip">SIGMA<div class="right">the widths of the Gaussian hills<i></i></div></div>=0.3,0.1
 <div class="tooltip">HEIGHT<div class="right">the heights of the Gaussian hills<i></i></div></div>=7.5
 <div class="tooltip">BIASFACTOR<div class="right">use well tempered metadynamics and use this bias factor<i></i></div></div>=30
 <div class="tooltip">TEMP<div class="right">the system temperature - this is only needed if you are doing well-tempered metadynamics<i></i></div></div>=850.0
 <div class="tooltip">PACE<div class="right">the frequency for hill addition<i></i></div></div>=500
 <div class="tooltip">GRID_MIN<div class="right">the lower bounds for the grid<i></i></div></div>=-330,-13
 <div class="tooltip">GRID_MAX<div class="right">the upper bounds for the grid<i></i></div></div>=-290,-1
 <div class="tooltip">GRID_BIN<div class="right">the number of bins for the grid<i></i></div></div>=500,500
 <div class="tooltip">CALC_RCT<div class="right"> calculate the c(t) reweighting factor and use that to obtain the normalized bias [rbias=bias-rct]<i></i></div></div>
... METAD
<br/><span style="display:none;" id="data/Aluminum/850K-MetaD/plumed.datmetad">The METAD action with label <b>metad</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">metad.bias</td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">metad.rbias</td><td>the instantaneous value of the bias normalized using the c(t) reweighting factor [rbias=bias-rct]</td></tr><tr><td width="5%">metad.rct</td><td>the reweighting factor $c(t)$</td></tr></table></span><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=500  <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div> <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=COLVAR
</pre>
{% endraw %}
