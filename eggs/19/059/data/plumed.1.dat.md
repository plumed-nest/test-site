**Project ID:** [plumID:19.059]({{ '/' | absolute_url }}eggs/19/059/)  
**Source:** plumed.1.dat  
**Originally used with PLUMED version:** 2.2.3  
**Stable:** [zipped raw stdout](plumed.1.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.1.dat.plumed.stderr.txt.zip) - [stderr](plumed.1.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.1.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.1.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.1.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/plumed.1.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.1.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.1.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue" class="comment">#RESTART</span>
<span id="data/plumed.1.datplumed_be-common.dat_short"><div class="tooltip" style="color:green">INCLUDE<div class="right">Includes an external input file, similar to #include in C preprocessor. <a href="https://www.plumed.org/doc-master/user-doc/html/_i_n_c_l_u_d_e.html">More details</a>. Show <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/plumed.1.datplumed_be-common.dat");'>included file</a><i></i></div></div> <div class="tooltip">FILE<div class="right">file to be included<i></i></div></div>=<a class="toggler" href='javascript:;' onclick='toggleDisplay("data/plumed.1.datplumed_be-common.dat");'>plumed_be-common.dat</a>
</span><span id="data/plumed.1.datplumed_be-common.dat_long" style="display:none;"><span style="color:blue" class="comment"># The command:
</span><span class="toggler" style="color:red" onclick='toggleDisplay("data/plumed.1.datplumed_be-common.dat")'># INCLUDE FILE=plumed_be-common.dat
</span><span style="color:blue" class="comment"># ensures PLUMED loads the contents of the file called plumed_be-common.dat</span>
<span style="color:blue" class="comment"># The contents of this file are shown below (click the red comment to hide them).</span>
<span style="color:blue" class="comment">#RESTART</span>
<span style="color:blue" class="comment"># randomize the exchange (not between consecutive indeces, here just 2 replicas, so it is not relevant)</span>
<span style="display:none;" id="data/plumed.1.datplumed_be-common.dat">The INCLUDE action with label <b>plumed_be-common.dat</b> calculates something</span><div class="tooltip" style="color:green">RANDOM_EXCHANGES<div class="right">Set random pattern for exchanges. <a href="https://www.plumed.org/doc-master/user-doc/html/_r_a_n_d_o_m__e_x_c_h_a_n_g_e_s.html" style="color:green">More details</a><i></i></div></div>
<span style="color:blue" class="comment"># set up the two torsion collective variables </span>
<span style="color:blue" class="comment"># omega (use cv1 so it will be compatible with the METAGUI analysis plugin)</span>
<span style="display:none;" id="data/plumed.1.dat">The RANDOM_EXCHANGES action with label <b></b> calculates something</span><b name="data/plumed.1.datcv1" onclick='showPath("data/plumed.1.dat","data/plumed.1.datcv1","data/plumed.1.datcv1","black")'>cv1</b><span style="display:none;" id="data/plumed.1.datcv1">The TORSION action with label <b>cv1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cv1</td><td width="5%"><font color="black">scalar</font></td><td>the TORSION involving these atoms</td></tr></table></span>: <div class="tooltip" style="color:green">TORSION<div class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the four atoms involved in the torsional angle<i></i></div></div>=19,40,42,45
<span style="color:blue" class="comment"># psi (use cv2 so it will be compatible with the METAGUI analysis plugin)</span>
<b name="data/plumed.1.datcv2" onclick='showPath("data/plumed.1.dat","data/plumed.1.datcv2","data/plumed.1.datcv2","black")'>cv2</b><span style="display:none;" id="data/plumed.1.datcv2">The TORSION action with label <b>cv2</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cv2</td><td width="5%"><font color="black">scalar</font></td><td>the TORSION involving these atoms</td></tr></table></span>: <div class="tooltip" style="color:green">TORSION<div class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the four atoms involved in the torsional angle<i></i></div></div>=41,45,53,55
<br/><span style="color:blue"># --- End of included input --- </span></span><br/><span style="color:blue" class="comment">#METAD activates metadynamics</span>
<span style="color:blue" class="comment">#ARG indicates variables to enhance (omega &amp; psi)</span>
<span style="color:blue" class="comment">#PACE indicates frequency of Gaussian deposition is 1000 time step (2ps)</span>
<span style="color:blue" class="comment">#HEIGHT indicates that height of the Gaussians is 0.2 kJ/mol</span>
<span style="color:blue" class="comment">#SIGMA indicates the width of the Gaussians on the biased cv, respectively</span>
<br/><span id="data/plumed.1.datdefbe_short"><b name="data/plumed.1.datbe" onclick='showPath("data/plumed.1.dat","data/plumed.1.datbe","data/plumed.1.datbe","black")'>be</b><span style="display:none;" id="data/plumed.1.datbe">The METAD action with label <b>be</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">be.bias</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the bias potential</td></tr></table></span>: <div class="tooltip" style="color:green">METAD<div class="right">Used to performed metadynamics on one or more collective variables. This action has <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/plumed.1.datdefbe");'>hidden defaults</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_e_t_a_d.html">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/plumed.1.datcv2">cv2</b> <div class="tooltip">PACE<div class="right">the frequency for hill addition<i></i></div></div>=1000 <div class="tooltip">HEIGHT<div class="right">the heights of the Gaussian hills<i></i></div></div>=0.2 <div class="tooltip">SIGMA<div class="right">the widths of the Gaussian hills<i></i></div></div>=0.23
</span><span id="data/plumed.1.datdefbe_long" style="display:none;"><b name="data/plumed.1.datbe" onclick='showPath("data/plumed.1.dat","data/plumed.1.datbe","data/plumed.1.datbe","black")'>be</b>: <div class="tooltip" style="color:green">METAD<div class="right">Used to performed metadynamics on one or more collective variables. This action uses the <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/plumed.1.datdefbe");'>defaults shown here</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_e_t_a_d.html">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/plumed.1.datcv2">cv2</b> <div class="tooltip">PACE<div class="right">the frequency for hill addition<i></i></div></div>=1000 <div class="tooltip">HEIGHT<div class="right">the heights of the Gaussian hills<i></i></div></div>=0.2 <div class="tooltip">SIGMA<div class="right">the widths of the Gaussian hills<i></i></div></div>=0.23  <div class="tooltip">FILE<div class="right"> a file in which the list of added hills is stored<i></i></div></div>=HILLS
</span><br/><span style="color:blue" class="comment">#print in other file the values of the CVS and the bias potential</span>
<span style="color:blue" class="comment">#STRIDE frequency of output</span>
<span style="color:blue" class="comment">#ARG things to print, omega, psi</span>
<span style="color:blue" class="comment">#FILE, name of the file to output; COLVAR</span>
<br/><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=500 <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/plumed.1.datcv1">cv1</b>,<b name="data/plumed.1.datcv2">cv2</b> <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=COLVAR
</pre>
{% endraw %}