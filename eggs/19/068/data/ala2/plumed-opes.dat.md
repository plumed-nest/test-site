**Project ID:** [plumID:19.068]({{ '/' | absolute_url }}eggs/19/068/)  
**Source:** ala2/plumed-opes.dat  
**Originally used with PLUMED version:** 2.7  
**Stable:** [zipped raw stdout](plumed-opes.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed-opes.dat.plumed.stderr.txt.zip) - [stderr](plumed-opes.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed-opes.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed-opes.dat.plumed_master.stderr.txt.zip) - [stderr](plumed-opes.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/ala2/plumed-opes.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed-opes.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed-opes.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<div class="tooltip" style="color:blue"># vim:ft=plumed<div class="right">Enables syntax highlighting for PLUMED files in vim. See <a href="https://www.plumed.org/doc-master/user-doc/html/_vim_syntax.html">here for more details. </a><i></i></div></div>
<br/><b name="data/ala2/plumed-opes.datphi" onclick='showPath("data/ala2/plumed-opes.dat","data/ala2/plumed-opes.datphi")'>phi</b>: <div class="tooltip" style="color:green">TORSION<div class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the four atoms involved in the torsional angle<i></i></div></div>=5,7,9,15
<span style="display:none;" id="data/ala2/plumed-opes.datphi">The TORSION action with label <b>phi</b> calculates a scalar quantity</span><b name="data/ala2/plumed-opes.datpsi" onclick='showPath("data/ala2/plumed-opes.dat","data/ala2/plumed-opes.datpsi")'>psi</b>: <div class="tooltip" style="color:green">TORSION<div class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the four atoms involved in the torsional angle<i></i></div></div>=7,9,15,17
<br/><span style="display:none;" id="data/ala2/plumed-opes.datpsi">The TORSION action with label <b>psi</b> calculates a scalar quantity</span><b name="data/ala2/plumed-opes.datopes" onclick='showPath("data/ala2/plumed-opes.dat","data/ala2/plumed-opes.datopes")'>opes</b>: <div class="tooltip" style="color:green">OPES_METAD<div class="right">On-the-fly probability enhanced sampling with metadynamics-like target distribution. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s__m_e_t_a_d.html" style="color:green">More details</a><i></i></div></div> ...
  <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/ala2/plumed-opes.datphi">phi</b>,<b name="data/ala2/plumed-opes.datpsi">psi</b>
  <div class="tooltip">FILE<div class="right"> a file in which the list of all deposited kernels is stored<i></i></div></div>=Kernels.data
  <div class="tooltip">TEMP<div class="right"> temperature<i></i></div></div>=300.0
  <div class="tooltip">PACE<div class="right">the frequency for kernel deposition<i></i></div></div>=500
  <div class="tooltip">SIGMA<div class="right"> the initial widths of the kernels<i></i></div></div>=0.15,0.15
  <div class="tooltip">BARRIER<div class="right">the free energy barrier to be overcome<i></i></div></div>=50
  <div class="tooltip">BIASFACTOR<div class="right">the gamma bias factor used for the well-tempered target distribution<i></i></div></div>=10
  <div class="tooltip">STATE_WFILE<div class="right">write to this file the compressed kernels and all the info needed to RESTART the simulation<i></i></div></div>=State.data
  <div class="tooltip">STATE_WSTRIDE<div class="right">number of MD steps between writing the STATE_WFILE<i></i></div></div>=10000
  <div class="tooltip">STORE_STATES<div class="right"> append to STATE_WFILE instead of ovewriting it each time<i></i></div></div>
...
<br/><span style="display:none;" id="data/ala2/plumed-opes.datopes">The OPES_METAD action with label <b>opes</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">opes.bias</td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">opes.rct</td><td>estimate of c(t)</td></tr><tr><td width="5%">opes.zed</td><td>estimate of Z_n</td></tr><tr><td width="5%">opes.neff</td><td>effective sample size</td></tr><tr><td width="5%">opes.nker</td><td>total number of compressed kernels used to represent the bias</td></tr></table></span><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">FMT<div class="right">the format that should be used to output real numbers<i></i></div></div>=%g <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=500 <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=Colvar.data <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/ala2/plumed-opes.datphi">phi</b>,<b name="data/ala2/plumed-opes.datpsi">psi</b>,<b name="data/ala2/plumed-opes.datopes">opes</b>
<br/><div class="tooltip" style="color:green">ENDPLUMED<div class="right">Terminate plumed input. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html" style="color:green">More details</a><i></i></div></div><span style="color:blue">

A slightly better performing result can be obtained with the following simpler input:

  opes: OPES_METAD ARG=phi,psi PACE=50 BARRIER=50 NLIST

but it was not used, to have a more fair comparison with standard metadynamics ala2 simulations.
(if not set, SIGMA is chosen adaptively, similarly to METAD ADAPTIVE=DIFF)
</span></pre>
{% endraw %}
