**Project ID:** [plumID:24.001]({{ '/' | absolute_url }}eggs/24/001/)  
**Source:** amylase/opes_flooding_qmmm/plumed.dat  
**Originally used with PLUMED version:** 2.9  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/amylase/opes_flooding_qmmm/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<div class="tooltip" style="color:green">UNITS<div class="right">This command sets the internal units for the code. <a href="https://www.plumed.org/doc-master/user-doc/html/_u_n_i_t_s.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">LENGTH<div class="right">the units of lengths<i></i></div></div>=A
<br/><span style="display:none;" id="data/amylase/opes_flooding_qmmm/plumed.dat">The UNITS action with label <b></b> calculates something</span><b name="data/amylase/opes_flooding_qmmm/plumed.datd_nuc" onclick='showPath("data/amylase/opes_flooding_qmmm/plumed.dat","data/amylase/opes_flooding_qmmm/plumed.datd_nuc","data/amylase/opes_flooding_qmmm/plumed.datd_nuc","black")'>d_nuc</b><span style="display:none;" id="data/amylase/opes_flooding_qmmm/plumed.datd_nuc">The DISTANCE action with label <b>d_nuc</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d_nuc</td><td width="5%"><font color="black">scalar</font></td><td>the DISTANCE between this pair of atoms</td></tr></table></span>: <div class="tooltip" style="color:green">DISTANCE<div class="right">Calculate the distance between a pair of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=3026,7700
<b name="data/amylase/opes_flooding_qmmm/plumed.datd_gly" onclick='showPath("data/amylase/opes_flooding_qmmm/plumed.dat","data/amylase/opes_flooding_qmmm/plumed.datd_gly","data/amylase/opes_flooding_qmmm/plumed.datd_gly","black")'>d_gly</b><span style="display:none;" id="data/amylase/opes_flooding_qmmm/plumed.datd_gly">The DISTANCE action with label <b>d_gly</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d_gly</td><td width="5%"><font color="black">scalar</font></td><td>the DISTANCE between this pair of atoms</td></tr></table></span>: <div class="tooltip" style="color:green">DISTANCE<div class="right">Calculate the distance between a pair of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=7700,7699
<b name="data/amylase/opes_flooding_qmmm/plumed.datd_acid" onclick='showPath("data/amylase/opes_flooding_qmmm/plumed.dat","data/amylase/opes_flooding_qmmm/plumed.datd_acid","data/amylase/opes_flooding_qmmm/plumed.datd_acid","black")'>d_acid</b><span style="display:none;" id="data/amylase/opes_flooding_qmmm/plumed.datd_acid">The DISTANCE action with label <b>d_acid</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d_acid</td><td width="5%"><font color="black">scalar</font></td><td>the DISTANCE between this pair of atoms</td></tr></table></span>: <div class="tooltip" style="color:green">DISTANCE<div class="right">Calculate the distance between a pair of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=7699,3607

<br/><span style="color:blue" class="comment">###### Walls #####################</span>
<div class="tooltip" style="color:green">UPPER_WALLS<div class="right">Defines a wall for the value of one or more collective variables, <a href="https://www.plumed.org/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the arguments on which the bias is acting<i></i></div></div>=<b name="data/amylase/opes_flooding_qmmm/plumed.datd_nuc">d_nuc</b> <div class="tooltip">AT<div class="right">the positions of the wall<i></i></div></div>=+4.0 <div class="tooltip">KAPPA<div class="right">the force constant for the wall<i></i></div></div>=500.0 <div class="tooltip">EXP<div class="right"> the powers for the walls<i></i></div></div>=2 <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/amylase/opes_flooding_qmmm/plumed.datuwall_d_nuc" onclick='showPath("data/amylase/opes_flooding_qmmm/plumed.dat","data/amylase/opes_flooding_qmmm/plumed.datuwall_d_nuc","data/amylase/opes_flooding_qmmm/plumed.datuwall_d_nuc","black")'>uwall_d_nuc</b><span style="display:none;" id="data/amylase/opes_flooding_qmmm/plumed.datuwall_d_nuc">The UPPER_WALLS action with label <b>uwall_d_nuc</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">uwall_d_nuc.bias</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">uwall_d_nuc.force2</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the squared force due to this bias potential</td></tr></table></span>
<div class="tooltip" style="color:green">UPPER_WALLS<div class="right">Defines a wall for the value of one or more collective variables, <a href="https://www.plumed.org/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the arguments on which the bias is acting<i></i></div></div>=<b name="data/amylase/opes_flooding_qmmm/plumed.datd_acid">d_acid</b> <div class="tooltip">AT<div class="right">the positions of the wall<i></i></div></div>=+4.0 <div class="tooltip">KAPPA<div class="right">the force constant for the wall<i></i></div></div>=500.0 <div class="tooltip">EXP<div class="right"> the powers for the walls<i></i></div></div>=2 <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/amylase/opes_flooding_qmmm/plumed.datuwall_d_acid" onclick='showPath("data/amylase/opes_flooding_qmmm/plumed.dat","data/amylase/opes_flooding_qmmm/plumed.datuwall_d_acid","data/amylase/opes_flooding_qmmm/plumed.datuwall_d_acid","black")'>uwall_d_acid</b><span style="display:none;" id="data/amylase/opes_flooding_qmmm/plumed.datuwall_d_acid">The UPPER_WALLS action with label <b>uwall_d_acid</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">uwall_d_acid.bias</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">uwall_d_acid.force2</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the squared force due to this bias potential</td></tr></table></span>
<br/><b name="data/amylase/opes_flooding_qmmm/plumed.datd_gly-wat" onclick='showPath("data/amylase/opes_flooding_qmmm/plumed.dat","data/amylase/opes_flooding_qmmm/plumed.datd_gly-wat","data/amylase/opes_flooding_qmmm/plumed.datd_gly-wat","black")'>d_gly-wat</b><span style="display:none;" id="data/amylase/opes_flooding_qmmm/plumed.datd_gly-wat">The DISTANCE action with label <b>d_gly-wat</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d_gly-wat</td><td width="5%"><font color="black">scalar</font></td><td>the DISTANCE between this pair of atoms</td></tr></table></span>: <div class="tooltip" style="color:green">DISTANCE<div class="right">Calculate the distance between a pair of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=7699,26287
<div class="tooltip" style="color:green">UPPER_WALLS<div class="right">Defines a wall for the value of one or more collective variables, <a href="https://www.plumed.org/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the arguments on which the bias is acting<i></i></div></div>=<b name="data/amylase/opes_flooding_qmmm/plumed.datd_gly-wat">d_gly-wat</b> <div class="tooltip">AT<div class="right">the positions of the wall<i></i></div></div>=+4.0 <div class="tooltip">KAPPA<div class="right">the force constant for the wall<i></i></div></div>=500.0 <div class="tooltip">EXP<div class="right"> the powers for the walls<i></i></div></div>=2 <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/amylase/opes_flooding_qmmm/plumed.datuwall_d_gly-wat" onclick='showPath("data/amylase/opes_flooding_qmmm/plumed.dat","data/amylase/opes_flooding_qmmm/plumed.datuwall_d_gly-wat","data/amylase/opes_flooding_qmmm/plumed.datuwall_d_gly-wat","black")'>uwall_d_gly-wat</b><span style="display:none;" id="data/amylase/opes_flooding_qmmm/plumed.datuwall_d_gly-wat">The UPPER_WALLS action with label <b>uwall_d_gly-wat</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">uwall_d_gly-wat.bias</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">uwall_d_gly-wat.force2</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the squared force due to this bias potential</td></tr></table></span>
<br/><span style="color:blue" class="comment">#d_strHbond1: DISTANCE ATOMS=7704,4655</span>
<span style="color:blue" class="comment">#UPPER_WALLS ARG=d_strHbond1 AT=+2.5 KAPPA=1000.0 EXP=2 LABEL=uwall_d_strHbond1</span>
<span style="color:blue" class="comment">#d_strHbond2: DISTANCE ATOMS=7708,4654</span>
<span style="color:blue" class="comment">#UPPER_WALLS ARG=d_strHbond2 AT=+2.5 KAPPA=1000.0 EXP=2 LABEL=uwall_d_strHbond2</span>
<span style="color:blue" class="comment">##################################</span>

<br/><span style="color:blue" class="comment">#metad: METAD ARG=d_gly SIGMA=0.1 HEIGHT=2.0 PACE=100 </span>
<br/><b name="data/amylase/opes_flooding_qmmm/plumed.datchi_exc" onclick='showPath("data/amylase/opes_flooding_qmmm/plumed.dat","data/amylase/opes_flooding_qmmm/plumed.datchi_exc","data/amylase/opes_flooding_qmmm/plumed.datchi_exc","black")'>chi_exc</b><span style="display:none;" id="data/amylase/opes_flooding_qmmm/plumed.datchi_exc">The CUSTOM action with label <b>chi_exc</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">chi_exc</td><td width="5%"><font color="black">scalar</font></td><td>an arbitrary function</td></tr></table></span>: <div class="tooltip" style="color:green">CUSTOM<div class="right">Calculate a combination of variables using a custom expression. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_u_s_t_o_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input to this function<i></i></div></div>=<b name="data/amylase/opes_flooding_qmmm/plumed.datd_gly">d_gly</b> <div class="tooltip">FUNC<div class="right">the function you wish to evaluate<i></i></div></div>=step(x-1.8 <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO
<br/><span id="data/amylase/opes_flooding_qmmm/plumed.datdefopes_short"><b name="data/amylase/opes_flooding_qmmm/plumed.datopes" onclick='showPath("data/amylase/opes_flooding_qmmm/plumed.dat","data/amylase/opes_flooding_qmmm/plumed.datopes","data/amylase/opes_flooding_qmmm/plumed.datopes","black")'>opes</b><span style="display:none;" id="data/amylase/opes_flooding_qmmm/plumed.datopes">The OPES_METAD action with label <b>opes</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">opes.bias</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">opes.rct</td><td width="5%"><font color="black">scalar</font></td><td>estimate of c(t). log(exp(beta V)/beta, should become flat as the simulation converges. Do NOT use for reweighting</td></tr><tr><td width="5%">opes.zed</td><td width="5%"><font color="black">scalar</font></td><td>estimate of Z_n. should become flat once no new CV-space region is explored</td></tr><tr><td width="5%">opes.neff</td><td width="5%"><font color="black">scalar</font></td><td>effective sample size</td></tr><tr><td width="5%">opes.nker</td><td width="5%"><font color="black">scalar</font></td><td>total number of compressed kernels used to represent the bias</td></tr></table></span>: <div class="tooltip" style="color:green">OPES_METAD<div class="right">On-the-fly probability enhanced sampling with metadynamics-like target distribution. This action has <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/amylase/opes_flooding_qmmm/plumed.datdefopes");'>hidden defaults</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s__m_e_t_a_d.html">More details</a><i></i></div></div> ...
  <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/amylase/opes_flooding_qmmm/plumed.datd_gly">d_gly</b>,<b name="data/amylase/opes_flooding_qmmm/plumed.datd_acid">d_acid</b>
  <div class="tooltip">PACE<div class="right">the frequency for kernel deposition<i></i></div></div>=100
  <div class="tooltip">ADAPTIVE_SIGMA_STRIDE<div class="right">number of steps for measuring adaptive sigma<i></i></div></div>=200
  <div class="tooltip">BARRIER<div class="right">the free energy barrier to be overcome<i></i></div></div>=50
  <div class="tooltip">EXCLUDED_REGION<div class="right">kernels are not deposited when the action provided here has a nonzero value, see example above<i></i></div></div>=<b name="data/amylase/opes_flooding_qmmm/plumed.datchi_exc">chi_exc</b>
  <div class="tooltip">TEMP<div class="right"> temperature<i></i></div></div>=300.0
...
</span><span id="data/amylase/opes_flooding_qmmm/plumed.datdefopes_long" style="display:none;"><b name="data/amylase/opes_flooding_qmmm/plumed.datopes" onclick='showPath("data/amylase/opes_flooding_qmmm/plumed.dat","data/amylase/opes_flooding_qmmm/plumed.datopes","data/amylase/opes_flooding_qmmm/plumed.datopes","black")'>opes</b>: <div class="tooltip" style="color:green">OPES_METAD<div class="right">On-the-fly probability enhanced sampling with metadynamics-like target distribution. This action uses the <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/amylase/opes_flooding_qmmm/plumed.datdefopes");'>defaults shown here</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s__m_e_t_a_d.html">More details</a><i></i></div></div> ...
  <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/amylase/opes_flooding_qmmm/plumed.datd_gly">d_gly</b>,<b name="data/amylase/opes_flooding_qmmm/plumed.datd_acid">d_acid</b>
  <div class="tooltip">PACE<div class="right">the frequency for kernel deposition<i></i></div></div>=100
  <div class="tooltip">ADAPTIVE_SIGMA_STRIDE<div class="right">number of steps for measuring adaptive sigma<i></i></div></div>=200
  <div class="tooltip">BARRIER<div class="right">the free energy barrier to be overcome<i></i></div></div>=50
  <div class="tooltip">EXCLUDED_REGION<div class="right">kernels are not deposited when the action provided here has a nonzero value, see example above<i></i></div></div>=<b name="data/amylase/opes_flooding_qmmm/plumed.datchi_exc">chi_exc</b>
  <div class="tooltip">TEMP<div class="right"> temperature<i></i></div></div>=300.0
 <div class="tooltip">SIGMA<div class="right"> the initial widths of the kernels<i></i></div></div>=ADAPTIVE <div class="tooltip">COMPRESSION_THRESHOLD<div class="right"> merge kernels if closer than this threshold, in units of sigma<i></i></div></div>=1 <div class="tooltip">FILE<div class="right"> a file in which the list of all deposited kernels is stored<i></i></div></div>=KERNELS
...
</span><br/><div class="tooltip" style="color:green">COMMITTOR<div class="right">Does a committor analysis. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_m_m_i_t_t_o_r.html" style="color:green">More details</a><i></i></div></div> ...
 <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/amylase/opes_flooding_qmmm/plumed.datd_gly">d_gly</b>
 <div class="tooltip">STRIDE<div class="right"> the frequency with which the CVs are analyzed<i></i></div></div>=10
 <div class="tooltip">BASIN_LL1<div class="right">List of lower limits for basin #<i></i></div></div>=3.3
 <div class="tooltip">BASIN_UL1<div class="right">List of upper limits for basin #<i></i></div></div>=10.0
... COMMITTOR

<br/><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/amylase/opes_flooding_qmmm/plumed.datd_gly">d_gly</b>,<b name="data/amylase/opes_flooding_qmmm/plumed.datd_acid">d_acid</b>,<b name="data/amylase/opes_flooding_qmmm/plumed.datopes">opes.*</b>,<b name="data/amylase/opes_flooding_qmmm/plumed.datuwall_d_nuc">uwall_d_nuc.*</b>,<b name="data/amylase/opes_flooding_qmmm/plumed.datuwall_d_acid">uwall_d_acid.*</b>,<b name="data/amylase/opes_flooding_qmmm/plumed.datuwall_d_gly-wat">uwall_d_gly-wat</b> <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=1 <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=COLVAR
<br/><div class="tooltip" style="color:green">FLUSH<div class="right">This command instructs plumed to flush all the open files with a user specified frequency. <a href="https://www.plumed.org/doc-master/user-doc/html/_f_l_u_s_h.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">STRIDE<div class="right">the frequency with which all the open files should be flushed<i></i></div></div>=1
</pre>
{% endraw %}