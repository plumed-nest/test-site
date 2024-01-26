**Project ID:** [plumID:20.022]({{ '/' | absolute_url }}eggs/20/022/)  
**Source:** water/plumed.dat  
**Originally used with PLUMED version:** 2.8  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/water/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr><tr><td style="padding:1px"><img src="https://img.shields.io/badge/with-LOAD-yellow.svg" alt="tested on master" /></td></tr>
</table></div></div>
<pre style="width=97%;">
<div class="tooltip" style="color:blue"># vim:ft=plumed<div class="right">Enables syntax highlighting for PLUMED files in vim. See <a href="https://www.plumed.org/doc-master/user-doc/html/_vim_syntax.html">here for more details. </a><i></i></div></div>
<div class="tooltip" style="color:green">LOAD<div class="right">Loads a library, possibly defining new actions. <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">FILE<div class="right">file to be loaded<i></i></div></div>=LennardJones.cpp
<br/><span style="color:blue">#+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++#</span>
<span style="color:blue">#                                                                       #</span>
<span style="color:blue">#  This input generates a simulation that samples all the intermediate  #</span>
<span style="color:blue">#  states needed for performing thermodynamic integration               #</span>
<span style="color:blue">#                                                                       #</span>
<span style="color:blue">#+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++#</span>
<br/><b name="data/water/plumed.dateneWAT" onclick='showPath("data/water/plumed.dat","data/water/plumed.dateneWAT")'>eneWAT</b>: <div class="tooltip" style="color:green">ENERGY<div class="right">Calculate the total potential energy of the simulation box. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_n_e_r_g_y.html" style="color:green">More details</a><i></i></div></div>
<div class="tooltip" style="color:green">LENNARDJONES<div class="right">This action is not part of PLUMED and was included by using a LOAD command <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></div></div> ...
 LABEL=<b name="data/water/plumed.dateneLJ" onclick='showPath("data/water/plumed.dat","data/water/plumed.dateneLJ")'>eneLJ</b>
 GROUPA=1-1152:3
 SIGMA=0.31536
 EPSILON=0.64852
 RCUT=0.85
 NLIST
 NL_CUTOFF=1.0
 NL_STRIDE=10
... LENNARDJONES
<b name="data/water/plumed.datDeltaU" onclick='showPath("data/water/plumed.dat","data/water/plumed.datDeltaU")'>DeltaU</b>: <div class="tooltip" style="color:green">CUSTOM<div class="right">Calculate a combination of variables using a custom expression. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_u_s_t_o_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/water/plumed.dateneLJ">eneLJ</b>,<b name="data/water/plumed.dateneWAT">eneWAT</b> <div class="tooltip">FUNC<div class="right">the function you wish to evaluate<i></i></div></div>=x-y <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO
<br/><span style="display:none;" id="data/water/plumed.datDeltaU">The CUSTOM action with label <b>DeltaU</b> calculates a scalar quantity</span><b name="data/water/plumed.datecv" onclick='showPath("data/water/plumed.dat","data/water/plumed.datecv")'>ecv</b>: <div class="tooltip" style="color:green">ECV_LINEAR<div class="right">Linear expansion, according to a parameter lambda. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_c_v__l_i_n_e_a_r.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label of the Hamiltonian difference<i></i></div></div>=<b name="data/water/plumed.datDeltaU">DeltaU</b> <div class="tooltip">TEMP<div class="right"> temperature<i></i></div></div>=443
<span style="display:none;" id="data/water/plumed.datecv">The ECV_LINEAR action with label <b>ecv</b> calculates a scalar quantity</span><b name="data/water/plumed.datopes" onclick='showPath("data/water/plumed.dat","data/water/plumed.datopes")'>opes</b>: <div class="tooltip" style="color:green">OPES_EXPANDED<div class="right">On-the-fly probability enhanced sampling with expanded ensembles for the target distribution. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s__e_x_p_a_n_d_e_d.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label of the ECVs that define the expansion<i></i></div></div>=<b name="data/water/plumed.datecv">ecv</b> <div class="tooltip">PACE<div class="right">how often the bias is updated<i></i></div></div>=100
<br/><span style="display:none;" id="data/water/plumed.datopes">The OPES_EXPANDED action with label <b>opes</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">opes.bias</td><td>the instantaneous value of the bias potential</td></tr></table></span><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/water/plumed.dateneWAT">eneWAT</b>,<b name="data/water/plumed.dateneLJ">eneLJ</b>,<b name="data/water/plumed.datDeltaU">DeltaU</b>,<b name="data/water/plumed.datopes">opes</b> <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=100 <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=COLVAR
<br/><div class="tooltip" style="color:green">ENDPLUMED<div class="right">Terminate plumed input. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html" style="color:green">More details</a><i></i></div></div><span style="color:blue">
</span></pre>
{% endraw %}
