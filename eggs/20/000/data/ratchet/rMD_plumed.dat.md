**Project ID:** [plumID:20.000]({{ '/' | absolute_url }}eggs/20/000/)  
**Source:** ratchet/rMD_plumed.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [zipped raw stdout](rMD_plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](rMD_plumed.dat.plumed.stderr.txt.zip) - [stderr](rMD_plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](rMD_plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](rMD_plumed.dat.plumed_master.stderr.txt.zip) - [stderr](rMD_plumed.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/ratchet/rMD_plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="rMD_plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="rMD_plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue" class="comment">#</span>
<span style="color:blue" class="comment"># This is the input file needed to perform Ratchet&amp;Pawl MD simulation</span>
<span style="color:blue" class="comment"># based on the CV given by the distance between the ligand&#x27;s center </span>
<span style="color:blue" class="comment"># of mass and the center of the binding pocket.</span>
<span style="color:blue" class="comment">#</span>
<span style="color:blue" class="comment"># This input file can be used with all the PLUMED versions &gt;=2.3</span>
<span style="color:blue" class="comment">#</span>
<br/><span style="color:blue" class="comment"># Definition of the center of mass of the ligand, considering only its heavy atoms</span>
<div class="tooltip" style="color:green">COM<div class="right">Calculate the center of mass for a group of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the list of atoms which are involved the virtual atom's definition<i></i></div></div>=1,5,6,10,14,17,18,19,22,23,24,25,26,29  <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/ratchet/rMD_plumed.datixo" onclick='showPath("data/ratchet/rMD_plumed.dat","data/ratchet/rMD_plumed.datixo","data/ratchet/rMD_plumed.datixo","violet")'>ixo</b><span style="display:none;" id="data/ratchet/rMD_plumed.datixo">The COM action with label <b>ixo</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ixo</td><td width="5%"><font color="violet">atoms</font></td><td>virtual atom calculated by COM action</td></tr></table></span>
<br/><span style="color:blue" class="comment"># Definition of the center of mass of the pocket</span>
<div class="tooltip" style="color:green">COM<div class="right">Calculate the center of mass for a group of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the list of atoms which are involved the virtual atom's definition<i></i></div></div>=1396,1398,1400,1403,1404,1406,1408,1409,1411,1413,1415,1416,1449,1451,1453,1456,1458,1459,1495,1497,1499,1501,1505,1509,1510,2838,2840,2842,2845,2846,2848,2850,2852,2854,2856,2857,3605,3607,3609,3612,3613,3615,3617,3618,3620,3622,3624,3625 <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/ratchet/rMD_plumed.datpkt" onclick='showPath("data/ratchet/rMD_plumed.dat","data/ratchet/rMD_plumed.datpkt","data/ratchet/rMD_plumed.datpkt","violet")'>pkt</b><span style="display:none;" id="data/ratchet/rMD_plumed.datpkt">The COM action with label <b>pkt</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">pkt</td><td width="5%"><font color="violet">atoms</font></td><td>virtual atom calculated by COM action</td></tr></table></span>
<br/><span style="color:blue" class="comment"># Definition of the distance between the ligand and the pocket as a 3d vector xyz</span>
<span style="color:blue" class="comment"># (the membrane is in the plane xy)</span>
<div class="tooltip" style="color:green">DISTANCE<div class="right">Calculate the distance between a pair of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=<b name="data/ratchet/rMD_plumed.datixo">ixo</b>,<b name="data/ratchet/rMD_plumed.datpkt">pkt</b> <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/ratchet/rMD_plumed.datd1" onclick='showPath("data/ratchet/rMD_plumed.dat","data/ratchet/rMD_plumed.datd1","data/ratchet/rMD_plumed.datd1","black")'>d1</b><span style="display:none;" id="data/ratchet/rMD_plumed.datd1">The DISTANCE action with label <b>d1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d1.x</td><td width="5%"><font color="black">scalar</font></td><td>the x-component of the vector connecting the two atoms</td></tr><tr><td width="5%">d1.y</td><td width="5%"><font color="black">scalar</font></td><td>the y-component of the vector connecting the two atoms</td></tr><tr><td width="5%">d1.z</td><td width="5%"><font color="black">scalar</font></td><td>the z-component of the vector connecting the two atoms</td></tr></table></span> <div class="tooltip">COMPONENTS<div class="right"> calculate the x, y and z components of the distance separately and store them as label<i></i></div></div> <div class="tooltip">NOPBC<div class="right"> ignore the periodic boundary conditions when calculating distances<i></i></div></div>
<br/><span style="color:blue" class="comment"># Definition of the periodicity of the components of the distance </span>
<span style="color:blue" class="comment"># (to avoid jumps in the variable during the simulation due to the </span>
<span style="color:blue" class="comment"># rototranslation of the system)</span>
<b name="data/ratchet/rMD_plumed.datd1x" onclick='showPath("data/ratchet/rMD_plumed.dat","data/ratchet/rMD_plumed.datd1x","data/ratchet/rMD_plumed.datd1x","black")'>d1x</b><span style="display:none;" id="data/ratchet/rMD_plumed.datd1x">The COMBINE action with label <b>d1x</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d1x</td><td width="5%"><font color="black">scalar</font></td><td>a linear compbination</td></tr></table></span>: <div class="tooltip" style="color:green">COMBINE<div class="right">Calculate a polynomial combination of a set of other variables. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_m_b_i_n_e.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input to this function<i></i></div></div>=<b name="data/ratchet/rMD_plumed.datd1">d1.x</b> <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=-4.7,4.7
<b name="data/ratchet/rMD_plumed.datd1y" onclick='showPath("data/ratchet/rMD_plumed.dat","data/ratchet/rMD_plumed.datd1y","data/ratchet/rMD_plumed.datd1y","black")'>d1y</b><span style="display:none;" id="data/ratchet/rMD_plumed.datd1y">The COMBINE action with label <b>d1y</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d1y</td><td width="5%"><font color="black">scalar</font></td><td>a linear compbination</td></tr></table></span>: <div class="tooltip" style="color:green">COMBINE<div class="right">Calculate a polynomial combination of a set of other variables. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_m_b_i_n_e.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input to this function<i></i></div></div>=<b name="data/ratchet/rMD_plumed.datd1">d1.y</b> <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=-4.7,4.7
<b name="data/ratchet/rMD_plumed.datd1z" onclick='showPath("data/ratchet/rMD_plumed.dat","data/ratchet/rMD_plumed.datd1z","data/ratchet/rMD_plumed.datd1z","black")'>d1z</b><span style="display:none;" id="data/ratchet/rMD_plumed.datd1z">The COMBINE action with label <b>d1z</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d1z</td><td width="5%"><font color="black">scalar</font></td><td>a linear compbination</td></tr></table></span>: <div class="tooltip" style="color:green">COMBINE<div class="right">Calculate a polynomial combination of a set of other variables. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_m_b_i_n_e.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input to this function<i></i></div></div>=<b name="data/ratchet/rMD_plumed.datd1">d1.z</b> <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=-8.2,8.2
<br/><span style="color:blue" class="comment"># Activation of the Ratchet&amp;Pawl MD, to observe the transition of the ligand. </span>
<span style="color:blue" class="comment"># Starting from the bound structure, the bias will move the system outside </span>
<span style="color:blue" class="comment"># the binding cavity with a k=100 kJ/mol/nm until the ligand is 4 nm outside</span>
<span style="color:blue" class="comment"># the binding cavity </span>
<div class="tooltip" style="color:green">ABMD<div class="right">Adds a ratchet-and-pawl like restraint on one or more variables. <a href="https://www.plumed.org/doc-master/user-doc/html/_a_b_m_d.html" style="color:green">More details</a><i></i></div></div> ...
  <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/ratchet/rMD_plumed.datd1z">d1z</b>
  <div class="tooltip">TO<div class="right">The array of target values<i></i></div></div>=-4.0
  <div class="tooltip">KAPPA<div class="right">The array of force constants<i></i></div></div>=100.0
<div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/ratchet/rMD_plumed.datrmd" onclick='showPath("data/ratchet/rMD_plumed.dat","data/ratchet/rMD_plumed.datrmd","data/ratchet/rMD_plumed.datrmd","black")'>rmd</b><span style="display:none;" id="data/ratchet/rMD_plumed.datrmd">The ABMD action with label <b>rmd</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">rmd.bias</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">rmd.d1z_min</td><td width="5%"><font color="black">scalar</font></td><td>one or multiple instances of this quantity can be referenced elsewhere in the input file.  These quantities will be named with the arguments of the bias followed by the character string _min. These quantities tell the user the minimum value assumed by rho_m(t). This particular component measures this quantity for the input CV named d1z</td></tr><tr><td width="5%">rmd.force2</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the squared force due to this bias potential</td></tr></table></span>
... ABMD

<br/><span style="color:blue" class="comment"># Here we print all the data regarding rMD_data</span>
<div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/ratchet/rMD_plumed.datrmd">rmd</b> <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=500 <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=rMD_data
<span style="color:blue" class="comment"># Here we print the distance between the molecule and the binding pocket</span>
<span style="display:none;" id="data/ratchet/rMD_plumed.dat">The PRINT action with label <b></b> calculates something</span><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/ratchet/rMD_plumed.datd1z">d1z</b> <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=500 <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=IXO_dist.dat
<br/><div class="tooltip" style="color:green">ENDPLUMED<div class="right">Terminate plumed input. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html" style="color:green">More details</a><i></i></div></div><span style="color:blue" class="comment">
</span></pre>
{% endraw %}