**Project ID:** [plumID:19.059]({{ '/' | absolute_url }}eggs/19/059/)  
**Source:** plumed_be-common.dat  
**Originally used with PLUMED version:** 2.2.3  
**Stable:** [zipped raw stdout](plumed_be-common.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_be-common.dat.plumed.stderr.txt.zip) - [stderr](plumed_be-common.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed_be-common.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_be-common.dat.plumed_master.stderr.txt.zip) - [stderr](plumed_be-common.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/plumed_be-common.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed_be-common.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-passing-green.svg" alt="tested onv2.10" /></a></td></tr><tr><td style="padding:1px"><a href="plumed_be-common.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue" class="comment">#RESTART</span>
<span style="color:blue" class="comment"># randomize the exchange (not between consecutive indeces, here just 2 replicas, so it is not relevant)</span>
<span class="plumedtooltip" style="color:green">RANDOM_EXCHANGES<span class="right">Set random pattern for exchanges. <a href="https://www.plumed.org/doc-master/user-doc/html/_r_a_n_d_o_m__e_x_c_h_a_n_g_e_s.html" style="color:green">More details</a><i></i></span></span>
<span style="color:blue" class="comment"># set up the two torsion collective variables </span>
<span style="color:blue" class="comment"># omega (use cv1 so it will be compatible with the METAGUI analysis plugin)</span>
<span style="display:none;" id="data/plumed_be-common.dat">The RANDOM_EXCHANGES action with label <b></b> calculates something</span><b name="data/plumed_be-common.datcv1" onclick='showPath("data/plumed_be-common.dat","data/plumed_be-common.datcv1","data/plumed_be-common.datcv1","black")'>cv1</b><span style="display:none;" id="data/plumed_be-common.datcv1">The TORSION action with label <b>cv1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cv1</td><td width="5%"><font color="black">scalar</font></td><td>the TORSION involving these atoms</td></tr></table></span>: <span class="plumedtooltip" style="color:green">TORSION<span class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=19,40,42,45
<span style="color:blue" class="comment"># psi (use cv2 so it will be compatible with the METAGUI analysis plugin)</span>
<b name="data/plumed_be-common.datcv2" onclick='showPath("data/plumed_be-common.dat","data/plumed_be-common.datcv2","data/plumed_be-common.datcv2","black")'>cv2</b><span style="display:none;" id="data/plumed_be-common.datcv2">The TORSION action with label <b>cv2</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cv2</td><td width="5%"><font color="black">scalar</font></td><td>the TORSION involving these atoms</td></tr></table></span>: <span class="plumedtooltip" style="color:green">TORSION<span class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=41,45,53,55
</pre>
{% endraw %}
