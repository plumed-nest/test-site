**Project ID:** [plumID:20.022]({{ '/' | absolute_url }}eggs/20/022/)  
**Source:** model/plumed.dat  
**Originally used with PLUMED version:** 2.8  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/model/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<div class="tooltip" style="color:blue"># vim:ft=plumed<div class="right">Enables syntax highlighting for PLUMED files in vim. See <a href="https://www.plumed.org/doc-master/user-doc/html/_vim_syntax.html">here for more details. </a><i></i></div></div>
<br/><span style="color:blue">#+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++#</span>
<span style="color:blue">#                                                           #</span>
<span style="color:blue">#  This input generates a simulation that samples the same  #</span>
<span style="color:blue">#  distribution as 28 umbrella-sampling windows             #</span>
<span style="color:blue">#                                                           #</span>
<span style="color:blue">#+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++#</span>
<br/><div class="tooltip" style="color:green">UNITS<div class="right">This command sets the internal units for the code. <a href="https://www.plumed.org/doc-master/user-doc/html/_u_n_i_t_s.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">NATURAL<div class="right"> use natural units<i></i></div></div>
<br/><b name="data/model/plumed.datp" onclick='showPath("data/model/plumed.dat","data/model/plumed.datp")'>p</b>: <div class="tooltip" style="color:green">POSITION<div class="right">Calculate the components of the position of an atom. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_o_s_i_t_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOM<div class="right">the atom number<i></i></div></div>=1
<br/><span style="display:none;" id="data/model/plumed.datp">The POSITION action with label <b>p</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">p.x</td><td>the x-component of the atom position</td></tr><tr><td width="5%">p.y</td><td>the y-component of the atom position</td></tr><tr><td width="5%">p.z</td><td>the z-component of the atom position</td></tr></table></span><b name="data/model/plumed.datecv" onclick='showPath("data/model/plumed.dat","data/model/plumed.datecv")'>ecv</b>: <div class="tooltip" style="color:green">ECV_UMBRELLAS_LINE<div class="right">Target a multiumbrella ensemble, by combining systems each with a parabolic bias potential at a different location. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_c_v__u_m_b_r_e_l_l_a_s__l_i_n_e.html" style="color:green">More details</a><i></i></div></div> ...
  <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/model/plumed.datp">p.x</b>
  <div class="tooltip">CV_MIN<div class="right">the minimum of the CV range to be explored<i></i></div></div>=-2.5
  <div class="tooltip">CV_MAX<div class="right">the maximum of the CV range to be explored<i></i></div></div>=2.5
  <div class="tooltip">SIGMA<div class="right">sigma of the umbrella Gaussians<i></i></div></div>=0.185815
...
<span style="display:none;" id="data/model/plumed.datecv">The ECV_UMBRELLAS_LINE action with label <b>ecv</b> calculates a scalar quantity</span><b name="data/model/plumed.datopes" onclick='showPath("data/model/plumed.dat","data/model/plumed.datopes")'>opes</b>: <div class="tooltip" style="color:green">OPES_EXPANDED<div class="right">On-the-fly probability enhanced sampling with expanded ensembles for the target distribution. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s__e_x_p_a_n_d_e_d.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label of the ECVs that define the expansion<i></i></div></div>=<b name="data/model/plumed.datecv">ecv</b> <div class="tooltip">FILE<div class="right"> a file with the estimate of the relative Delta F for each component of the target and of the global c(t)<i></i></div></div>=DeltaFs.data <div class="tooltip">PACE<div class="right">how often the bias is updated<i></i></div></div>=500
<br/><span style="display:none;" id="data/model/plumed.datopes">The OPES_EXPANDED action with label <b>opes</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">opes.bias</td><td>the instantaneous value of the bias potential</td></tr></table></span><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">FMT<div class="right">the format that should be used to output real numbers<i></i></div></div>=%g <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=500 <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=Colvar.data <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/model/plumed.datp">p.x</b>,<b name="data/model/plumed.datp">p.y</b>,<b name="data/model/plumed.datopes">opes</b>
<br/><div class="tooltip" style="color:green">ENDPLUMED<div class="right">Terminate plumed input. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html" style="color:green">More details</a><i></i></div></div><span style="color:blue">

will produce 10 independent run, use instead WALKERS_MPI to make multiple walkers share bias

to print the running FES with GNUPLOT:
p '<awk ''END{for(i=3;i<=NF;i++)print -2.5+(i-3)*5/(NF-3),$i}'' DeltaFs.0.data'w lp
</span></pre>
{% endraw %}
