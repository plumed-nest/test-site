**Project ID:** [plumID:19.044]({{ '/' | absolute_url }}eggs/19/044/)  
**Source:** MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.dat  
**Originally used with PLUMED version:** 2.4-dev  
**Stable:** [zipped raw stdout](plumed.start.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.start.dat.plumed.stderr.txt.zip) - [stderr](plumed.start.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.start.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.start.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.start.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.start.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.start.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<div class="tooltip" style="color:blue"># vim:ft=plumed<div class="right">Enables syntax highlighting for PLUMED files in vim. See <a href="https://www.plumed.org/doc-master/user-doc/html/_vim_syntax.html">here for more details. </a><i></i></div></div>
<br/><b name="data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.datenergy" onclick='showPath("data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.dat","data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.datenergy","data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.datenergy","black")'>energy</b><span style="display:none;" id="data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.datenergy">The ENERGY action with label <b>energy</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">energy</td><td width="5%"><font color="black">scalar</font></td><td>the value calculated by this action</td></tr></table></span>: <div class="tooltip" style="color:green">ENERGY<div class="right">Calculate the total potential energy of the simulation box. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_n_e_r_g_y.html" style="color:green">More details</a><i></i></div></div>
<br/><b name="data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.datvol" onclick='showPath("data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.dat","data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.datvol","data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.datvol","black")'>vol</b><span style="display:none;" id="data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.datvol">The VOLUME action with label <b>vol</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">vol</td><td width="5%"><font color="black">scalar</font></td><td>the volume of simulation box</td></tr></table></span>: <div class="tooltip" style="color:green">VOLUME<div class="right">Calculate the volume of the simulation box. <a href="https://www.plumed.org/doc-master/user-doc/html/_v_o_l_u_m_e.html" style="color:green">More details</a><i></i></div></div>
<br/><span style="color:blue" class="comment"># Construct a bias potential using VES</span>
<span style="color:blue" class="comment">#</span>
<span style="color:blue" class="comment"># Basis functions</span>
<br/><b name="data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.datbf1" onclick='showPath("data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.dat","data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.datbf1","data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.datbf1","brown")'>bf1</b>: <div class="tooltip" style="color:green">BF_LEGENDRE<div class="right">Legendre polynomials basis functions. <a href="https://www.plumed.org/doc-master/user-doc/html/_b_f__l_e_g_e_n_d_r_e.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ORDER<div class="right">The order of the basis function expansion<i></i></div></div>=10 <div class="tooltip">MINIMUM<div class="right">The minimum of the interval on which the basis functions are defined<i></i></div></div>=-14750 <div class="tooltip">MAXIMUM<div class="right">The maximum of the interval on which the basis functions are defined<i></i></div></div>=-12250
<span style="display:none;" id="data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.datbf1">The BF_LEGENDRE action with label <b>bf1</b> calculates something</span><b name="data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.datbf2" onclick='showPath("data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.dat","data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.datbf2","data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.datbf2","brown")'>bf2</b>: <div class="tooltip" style="color:green">BF_LEGENDRE<div class="right">Legendre polynomials basis functions. <a href="https://www.plumed.org/doc-master/user-doc/html/_b_f__l_e_g_e_n_d_r_e.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ORDER<div class="right">The order of the basis function expansion<i></i></div></div>=10 <div class="tooltip">MINIMUM<div class="right">The minimum of the interval on which the basis functions are defined<i></i></div></div>=6.5 <div class="tooltip">MAXIMUM<div class="right">The maximum of the interval on which the basis functions are defined<i></i></div></div>=8.25
<br/><span style="color:blue" class="comment"># Target distributions</span>
<span style="display:none;" id="data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.datbf2">The BF_LEGENDRE action with label <b>bf2</b> calculates something</span><div class="tooltip" style="color:green">TD_MULTITHERMAL_MULTIBARIC<div class="right">Multithermal-multibaric target distribution (dynamic). <a href="https://www.plumed.org/doc-master/user-doc/html/_t_d__m_u_l_t_i_t_h_e_r_m_a_l__m_u_l_t_i_b_a_r_i_c.html" style="color:green">More details</a><i></i></div></div> ...
 <div class="tooltip">MIN_TEMP<div class="right">Minimum energy<i></i></div></div>=260
 <div class="tooltip">MAX_TEMP<div class="right">Maximum energy<i></i></div></div>=350
 <div class="tooltip">MAX_PRESSURE<div class="right">Maximum pressure<i></i></div></div>=180.66422571 <span style="color:blue" class="comment"># 300 MPa</span>
 <div class="tooltip">MIN_PRESSURE<div class="right">Minimum pressure<i></i></div></div>=0.06022140857
 <div class="tooltip">PRESSURE<div class="right">Target pressure of the barostat used in the MD engine<i></i></div></div>=0.06022140857
 <div class="tooltip">STEPS_PRESSURE<div class="right"> Number of pressure steps<i></i></div></div>=20
 <div class="tooltip">STEPS_TEMP<div class="right"> Number of temperature steps<i></i></div></div>=20
 <div class="tooltip">SIGMA<div class="right">The standard deviation parameters of the Gaussian kernels used for smoothing the target distribution<i></i></div></div>=50.,0.05
 <div class="tooltip">THRESHOLD<div class="right"> Maximum exploration free energy in kT<i></i></div></div>=1
 <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.dattd_multi" onclick='showPath("data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.dat","data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.dattd_multi","data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.dattd_multi","brown")'>td_multi</b>
... TD_MULTITHERMAL_MULTIBARIC
<br/><span style="color:blue" class="comment"># Expansion</span>
<br/><span style="display:none;" id="data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.dattd_multi">The TD_MULTITHERMAL_MULTIBARIC action with label <b>td_multi</b> calculates something</span><div class="tooltip" style="color:green">VES_LINEAR_EXPANSION<div class="right">Linear basis set expansion bias. <a href="https://www.plumed.org/doc-master/user-doc/html/_v_e_s__l_i_n_e_a_r__e_x_p_a_n_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> ...
 <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.datenergy">energy</b>,<b name="data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.datvol">vol</b>
 <div class="tooltip">BASIS_FUNCTIONS<div class="right">the label of the one dimensional basis functions that should be used<i></i></div></div>=<b name="data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.datbf1">bf1</b>,<b name="data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.datbf2">bf2</b>
 <div class="tooltip">TEMP<div class="right">the system temperature - this is needed if the MD code does not pass the temperature to PLUMED<i></i></div></div>=300.0
 <div class="tooltip">GRID_BINS<div class="right">the number of bins used for the grid<i></i></div></div>=200,200
 <div class="tooltip">TARGET_DISTRIBUTION<div class="right">the label of the target distribution to be used<i></i></div></div>=<b name="data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.dattd_multi">td_multi</b>
 <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.datb1" onclick='showPath("data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.dat","data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.datb1","data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.datb1","black")'>b1</b><span style="display:none;" id="data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.datb1">The VES_LINEAR_EXPANSION action with label <b>b1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">b1.bias</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">b1.force2</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the squared force due to this bias potential.</td></tr></table></span>
... VES_LINEAR_EXPANSION
<br/><span style="color:blue" class="comment"># Optimization algorithm</span>
<br/><span id="data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.datdefo1_short"><div class="tooltip" style="color:green">OPT_AVERAGED_SGD<div class="right">Averaged stochastic gradient decent with fixed step size. This action has <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.datdefo1");'>hidden defaults</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_p_t__a_v_e_r_a_g_e_d__s_g_d.html">More details</a><i></i></div></div> ...
  <div class="tooltip">BIAS<div class="right">the label of the VES bias to be optimized<i></i></div></div>=<b name="data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.datb1">b1</b>
  <div class="tooltip">STRIDE<div class="right">the frequency of updating the coefficients given in the number of MD steps<i></i></div></div>=500
  <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.dato1" onclick='showPath("data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.dat","data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.dato1","data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.dato1","brown")'>o1</b>
  <div class="tooltip">STEPSIZE<div class="right">the step size used for the optimization<i></i></div></div>=10 <span style="color:blue" class="comment"># Later I found a stepsize of 1 seems to work better.</span>
  <div class="tooltip">FES_OUTPUT<div class="right">how often the FES(s) should be written out to file<i></i></div></div>=500
  <div class="tooltip">BIAS_OUTPUT<div class="right">how often the bias(es) should be written out to file<i></i></div></div>=500
  <div class="tooltip">TARGETDIST_OUTPUT<div class="right">how often the dynamic target distribution(s) should be written out to file<i></i></div></div>=500
  <div class="tooltip">COEFFS_OUTPUT<div class="right"> how often the coefficients should be written to file<i></i></div></div>=10
  <div class="tooltip">TARGETDIST_STRIDE<div class="right">stride for updating a target distribution that is iteratively updated during the optimization<i></i></div></div>=100
... OPT_AVERAGED_SGD
</span><span id="data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.datdefo1_long" style="display:none;"><span style="display:none;" id="data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.dato1">The OPT_AVERAGED_SGD action with label <b>o1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">o1.value</td><td>a scalar</td></tr></table></span><div class="tooltip" style="color:green">OPT_AVERAGED_SGD<div class="right">Averaged stochastic gradient decent with fixed step size. This action uses the <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.datdefo1");'>defaults shown here</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_p_t__a_v_e_r_a_g_e_d__s_g_d.html">More details</a><i></i></div></div> ...
  <div class="tooltip">BIAS<div class="right">the label of the VES bias to be optimized<i></i></div></div>=<b name="data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.datb1">b1</b>
  <div class="tooltip">STRIDE<div class="right">the frequency of updating the coefficients given in the number of MD steps<i></i></div></div>=500
  <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.dato1" onclick='showPath("data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.dat","data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.dato1","data/MultithermalMultibaricSimulations/MultithermalMultibaric/Input/plumed.start.dato1","brown")'>o1</b>
  <div class="tooltip">STEPSIZE<div class="right">the step size used for the optimization<i></i></div></div>=10 <span style="color:blue" class="comment"># Later I found a stepsize of 1 seems to work better.</span>
  <div class="tooltip">FES_OUTPUT<div class="right">how often the FES(s) should be written out to file<i></i></div></div>=500
  <div class="tooltip">BIAS_OUTPUT<div class="right">how often the bias(es) should be written out to file<i></i></div></div>=500
  <div class="tooltip">TARGETDIST_OUTPUT<div class="right">how often the dynamic target distribution(s) should be written out to file<i></i></div></div>=500
  <div class="tooltip">COEFFS_OUTPUT<div class="right"> how often the coefficients should be written to file<i></i></div></div>=10
  <div class="tooltip">TARGETDIST_STRIDE<div class="right">stride for updating a target distribution that is iteratively updated during the optimization<i></i></div></div>=100
 <div class="tooltip">COEFFS_FILE<div class="right"> the name of output file for the coefficients<i></i></div></div>=coeffs.data
... OPT_AVERAGED_SGD
</span><br/><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div> <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=COLVAR <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=500
</pre>
{% endraw %}