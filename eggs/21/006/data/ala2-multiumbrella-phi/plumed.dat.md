**Project ID:** [plumID:21.006]({{ '/' | absolute_url }}eggs/21/006/)  
**Source:** ala2-multiumbrella-phi/plumed.dat  
**Originally used with PLUMED version:** 2.8  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/ala2-multiumbrella-phi/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<div class="tooltip" style="color:blue"># vim:ft=plumed<div class="right">Enables syntax highlighting for PLUMED files in vim. See <a href="https://www.plumed.org/doc-master/user-doc/html/_vim_syntax.html">here for more details. </a><i></i></div></div>
<br/><span style="color:blue" class="comment">#+++++++++++++++++++++++++++++++++++++++++++++++++++#</span>
<span style="color:blue" class="comment">#                                                   #</span>
<span style="color:blue" class="comment">#  This input generates a multiumbrella simulation  #</span>
<span style="color:blue" class="comment">#  that samples along the phi collective variable   #</span>
<span style="color:blue" class="comment">#                                                   #</span>
<span style="color:blue" class="comment">#+++++++++++++++++++++++++++++++++++++++++++++++++++#</span>
<br/><b name="data/ala2-multiumbrella-phi/plumed.datphi" onclick='showPath("data/ala2-multiumbrella-phi/plumed.dat","data/ala2-multiumbrella-phi/plumed.datphi","data/ala2-multiumbrella-phi/plumed.datphi","black")'>phi</b><span style="display:none;" id="data/ala2-multiumbrella-phi/plumed.datphi">The TORSION action with label <b>phi</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">phi</td><td width="5%"><font color="black">scalar</font></td><td>the TORSION involving these atoms</td></tr></table></span>: <div class="tooltip" style="color:green">TORSION<div class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the four atoms involved in the torsional angle<i></i></div></div>=5,7,9,15
<b name="data/ala2-multiumbrella-phi/plumed.datpsi" onclick='showPath("data/ala2-multiumbrella-phi/plumed.dat","data/ala2-multiumbrella-phi/plumed.datpsi","data/ala2-multiumbrella-phi/plumed.datpsi","black")'>psi</b><span style="display:none;" id="data/ala2-multiumbrella-phi/plumed.datpsi">The TORSION action with label <b>psi</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">psi</td><td width="5%"><font color="black">scalar</font></td><td>the TORSION involving these atoms</td></tr></table></span>: <div class="tooltip" style="color:green">TORSION<div class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the four atoms involved in the torsional angle<i></i></div></div>=7,9,15,17
<b name="data/ala2-multiumbrella-phi/plumed.datene" onclick='showPath("data/ala2-multiumbrella-phi/plumed.dat","data/ala2-multiumbrella-phi/plumed.datene","data/ala2-multiumbrella-phi/plumed.datene","black")'>ene</b><span style="display:none;" id="data/ala2-multiumbrella-phi/plumed.datene">The ENERGY action with label <b>ene</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ene</td><td width="5%"><font color="black">scalar</font></td><td>the value calculated by this action</td></tr></table></span>: <div class="tooltip" style="color:green">ENERGY<div class="right">Calculate the total potential energy of the simulation box. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_n_e_r_g_y.html" style="color:green">More details</a><i></i></div></div>
<br/><span id="data/ala2-multiumbrella-phi/plumed.datdefecv_short"><b name="data/ala2-multiumbrella-phi/plumed.datecv" onclick='showPath("data/ala2-multiumbrella-phi/plumed.dat","data/ala2-multiumbrella-phi/plumed.datecv","data/ala2-multiumbrella-phi/plumed.datecv","black")'>ecv</b><span style="display:none;" id="data/ala2-multiumbrella-phi/plumed.datecv">The ECV_UMBRELLAS_LINE action with label <b>ecv</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ecv.phi</td><td width="5%"><font color="black">scalar</font></td><td>the value of the argument named phi</td></tr></table></span>: <div class="tooltip" style="color:green">ECV_UMBRELLAS_LINE<div class="right">Target a multiumbrella ensemble, by combining systems each with a parabolic bias potential at a different location. This action has <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/ala2-multiumbrella-phi/plumed.datdefecv");'>hidden defaults</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_c_v__u_m_b_r_e_l_l_a_s__l_i_n_e.html">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/ala2-multiumbrella-phi/plumed.datphi">phi</b> <div class="tooltip">CV_MIN<div class="right">the minimum of the CV range to be explored<i></i></div></div>=-pi <div class="tooltip">CV_MAX<div class="right">the maximum of the CV range to be explored<i></i></div></div>=pi <div class="tooltip">SIGMA<div class="right">sigma of the umbrella Gaussians<i></i></div></div>=0.15 <div class="tooltip">BARRIER<div class="right">a guess of the free energy barrier to be overcome (better to stay higher than lower)<i></i></div></div>=50
</span><span id="data/ala2-multiumbrella-phi/plumed.datdefecv_long" style="display:none;"><b name="data/ala2-multiumbrella-phi/plumed.datecv" onclick='showPath("data/ala2-multiumbrella-phi/plumed.dat","data/ala2-multiumbrella-phi/plumed.datecv","data/ala2-multiumbrella-phi/plumed.datecv","black")'>ecv</b>: <div class="tooltip" style="color:green">ECV_UMBRELLAS_LINE<div class="right">Target a multiumbrella ensemble, by combining systems each with a parabolic bias potential at a different location. This action uses the <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/ala2-multiumbrella-phi/plumed.datdefecv");'>defaults shown here</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_c_v__u_m_b_r_e_l_l_a_s__l_i_n_e.html">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/ala2-multiumbrella-phi/plumed.datphi">phi</b> <div class="tooltip">CV_MIN<div class="right">the minimum of the CV range to be explored<i></i></div></div>=-pi <div class="tooltip">CV_MAX<div class="right">the maximum of the CV range to be explored<i></i></div></div>=pi <div class="tooltip">SIGMA<div class="right">sigma of the umbrella Gaussians<i></i></div></div>=0.15 <div class="tooltip">BARRIER<div class="right">a guess of the free energy barrier to be overcome (better to stay higher than lower)<i></i></div></div>=50  <div class="tooltip">TEMP<div class="right"> temperature<i></i></div></div>=-1 <div class="tooltip">SPACING<div class="right"> the distance between umbrellas, in units of SIGMA<i></i></div></div>=1
</span><span id="data/ala2-multiumbrella-phi/plumed.datdefopes_short"><b name="data/ala2-multiumbrella-phi/plumed.datopes" onclick='showPath("data/ala2-multiumbrella-phi/plumed.dat","data/ala2-multiumbrella-phi/plumed.datopes","data/ala2-multiumbrella-phi/plumed.datopes","black")'>opes</b><span style="display:none;" id="data/ala2-multiumbrella-phi/plumed.datopes">The OPES_EXPANDED action with label <b>opes</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">opes.bias</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the bias potential</td></tr></table></span>: <div class="tooltip" style="color:green">OPES_EXPANDED<div class="right">On-the-fly probability enhanced sampling with expanded ensembles for the target distribution. This action has <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/ala2-multiumbrella-phi/plumed.datdefopes");'>hidden defaults</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s__e_x_p_a_n_d_e_d.html">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label of the ECVs that define the expansion<i></i></div></div>=<b name="data/ala2-multiumbrella-phi/plumed.datecv">ecv</b> <div class="tooltip">PACE<div class="right">how often the bias is updated<i></i></div></div>=500 <div class="tooltip">FILE<div class="right"> a file with the estimate of the relative Delta F for each component of the target and of the global c(t)<i></i></div></div>=DeltaFs.data <div class="tooltip">STATE_WFILE<div class="right">write to this file the Delta F estimates and all the info needed to RESTART the simulation<i></i></div></div>=State.data
</span><span id="data/ala2-multiumbrella-phi/plumed.datdefopes_long" style="display:none;"><b name="data/ala2-multiumbrella-phi/plumed.datopes" onclick='showPath("data/ala2-multiumbrella-phi/plumed.dat","data/ala2-multiumbrella-phi/plumed.datopes","data/ala2-multiumbrella-phi/plumed.datopes","black")'>opes</b>: <div class="tooltip" style="color:green">OPES_EXPANDED<div class="right">On-the-fly probability enhanced sampling with expanded ensembles for the target distribution. This action uses the <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/ala2-multiumbrella-phi/plumed.datdefopes");'>defaults shown here</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s__e_x_p_a_n_d_e_d.html">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the label of the ECVs that define the expansion<i></i></div></div>=<b name="data/ala2-multiumbrella-phi/plumed.datecv">ecv</b> <div class="tooltip">PACE<div class="right">how often the bias is updated<i></i></div></div>=500 <div class="tooltip">FILE<div class="right"> a file with the estimate of the relative Delta F for each component of the target and of the global c(t)<i></i></div></div>=DeltaFs.data <div class="tooltip">STATE_WFILE<div class="right">write to this file the Delta F estimates and all the info needed to RESTART the simulation<i></i></div></div>=State.data  <div class="tooltip">OBSERVATION_STEPS<div class="right"> number of unbiased initial PACE steps to collect statistics for initialization<i></i></div></div>=100 <div class="tooltip">PRINT_STRIDE<div class="right"> stride for printing to DELTAFS file, in units of PACE<i></i></div></div>=100
</span><br/><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">FMT<div class="right">the format that should be used to output real numbers<i></i></div></div>=%g <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=500 <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=Colvar.data <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/ala2-multiumbrella-phi/plumed.datphi">phi</b>,<b name="data/ala2-multiumbrella-phi/plumed.datpsi">psi</b>,<b name="data/ala2-multiumbrella-phi/plumed.datene">ene</b>,<b name="data/ala2-multiumbrella-phi/plumed.datopes">opes.bias</b>
<br/><span style="display:none;" id="data/ala2-multiumbrella-phi/plumed.dat">The PRINT action with label <b></b> calculates something</span><div class="tooltip" style="color:green">ENDPLUMED<div class="right">Terminate plumed input. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html" style="color:green">More details</a><i></i></div></div><span style="color:blue" class="comment">

This choice of SIGMA will generate 43 umbrellas.
</span></pre>
{% endraw %}