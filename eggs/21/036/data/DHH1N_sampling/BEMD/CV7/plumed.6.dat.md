**Project ID:** [plumID:21.036]({{ '/' | absolute_url }}eggs/21/036/)  
**Source:** DHH1N_sampling/BEMD/CV7/plumed.6.dat  
**Originally used with PLUMED version:** 2.5.2  
**Stable:** [zipped raw stdout](plumed.6.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.6.dat.plumed.stderr.txt.zip) - [stderr](plumed.6.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.6.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.6.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.6.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/DHH1N_sampling/BEMD/CV7/plumed.6.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.6.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.6.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue" class="comment">#RESTART</span>
<br/><div class="tooltip" style="color:green">MOLINFO<div class="right">This command is used to provide information on the molecules that are present in your system. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">STRUCTURE<div class="right">a file in pdb format containing a reference structure<i></i></div></div>=Protein.pdb <div class="tooltip">MOLTYPE<div class="right"> what kind of molecule is contained in the pdb file - usually not needed since protein/RNA/DNA are compatible<i></i></div></div>=protein
<br/><span style="display:none;" id="data/DHH1N_sampling/BEMD/CV7/plumed.6.dat">The MOLINFO action with label <b></b> calculates something</span><div class="tooltip" style="color:green">WHOLEMOLECULES<div class="right">This action is used to rebuild molecules that can become split by the periodic boundary conditions. <a href="https://www.plumed.org/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ENTITY0<div class="right">the atoms that make up a molecule that you wish to align<i></i></div></div>=1-709
<br/><div class="tooltip" style="color:green">RANDOM_EXCHANGES<div class="right">Set random pattern for exchanges. <a href="https://www.plumed.org/doc-master/user-doc/html/_r_a_n_d_o_m__e_x_c_h_a_n_g_e_s.html" style="color:green">More details</a><i></i></div></div>
<br/><span id="data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7_short"><span id="data/DHH1N_sampling/BEMD/CV7/plumed.6.datdefcv7_short"><b name="data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7" onclick='showPath("data/DHH1N_sampling/BEMD/CV7/plumed.6.dat","data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7","data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7_shortcut","black")'>cv7</b><span style="display:none;" id="data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7_shortcut">The PARABETARMSD action with label <b>cv7</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cv7</td><td width="5%"><font color="black">scalar</font></td><td>the value calculated by this action</td></tr></table></span>: <div class="tooltip" style="color:green">PARABETARMSD<div class="right">Probe the parallel beta sheet content of your protein structure. This action is <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7");'>a shortcut</a> and it has <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/DHH1N_sampling/BEMD/CV7/plumed.6.datdefcv7");'>hidden defaults</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_a_r_a_b_e_t_a_r_m_s_d.html">More details</a><i></i></div></div> <div class="tooltip">RESIDUES<div class="right">this command is used to specify the set of residues that could conceivably form part of the secondary structure<i></i></div></div>=1-45 <div class="tooltip">TYPE<div class="right"> the manner in which RMSD alignment is performed<i></i></div></div>=DRMSD <div class="tooltip">NN<div class="right"> The n parameter of the switching function<i></i></div></div>=8 <div class="tooltip">MM<div class="right"> The m parameter of the switching function<i></i></div></div>=12 <div class="tooltip">R_0<div class="right">The r_0 parameter of the switching function<i></i></div></div>=0.08 <div class="tooltip">NOPBC<div class="right"> ignore the periodic boundary conditions<i></i></div></div>
</span><span id="data/DHH1N_sampling/BEMD/CV7/plumed.6.datdefcv7_long" style="display:none;"><b name="data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7" onclick='showPath("data/DHH1N_sampling/BEMD/CV7/plumed.6.dat","data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7","data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7_shortcut","black")'>cv7</b>: <div class="tooltip" style="color:green">PARABETARMSD<div class="right">Probe the parallel beta sheet content of your protein structure. This action is <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7");'>a shortcut</a> and uses the <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/DHH1N_sampling/BEMD/CV7/plumed.6.datdefcv7");'>defaults shown here</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_a_r_a_b_e_t_a_r_m_s_d.html">More details</a><i></i></div></div> <div class="tooltip">RESIDUES<div class="right">this command is used to specify the set of residues that could conceivably form part of the secondary structure<i></i></div></div>=1-45 <div class="tooltip">TYPE<div class="right"> the manner in which RMSD alignment is performed<i></i></div></div>=DRMSD <div class="tooltip">NN<div class="right"> The n parameter of the switching function<i></i></div></div>=8 <div class="tooltip">MM<div class="right"> The m parameter of the switching function<i></i></div></div>=12 <div class="tooltip">R_0<div class="right">The r_0 parameter of the switching function<i></i></div></div>=0.08 <div class="tooltip">NOPBC<div class="right"> ignore the periodic boundary conditions<i></i></div></div>  <div class="tooltip">D_0<div class="right"> The d_0 parameter of the switching function<i></i></div></div>=0.0 <div class="tooltip">STYLE<div class="right"> Parallel beta sheets can either form in a single chain or from a pair of chains<i></i></div></div>=all
</span></span><span id="data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7_long" style="display:none;"><span style="color:blue" class="comment"># PLUMED interprets the command:
</span><span class="toggler" style="color:red" onclick='toggleDisplay("data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7")'># cv7: PARABETARMSD RESIDUES=1-45 TYPE=DRMSD NN=8 MM=12 R_0=0.08 NOPBC</span>
<span style="color:blue" class="comment"># as follows (Click the red comment above to revert to the short version of the input):</span>
<b name="data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7_both" onclick='showPath("data/DHH1N_sampling/BEMD/CV7/plumed.6.dat","data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7_both","data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7_both","blue")'>cv7_both</b><span style="display:none;" id="data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7_both">The SECONDARY_STRUCTURE_RMSD action with label <b>cv7_both</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cv7_both.struct-1</td><td width="5%"><font color="blue">vector</font></td><td>the vectors containing the rmsd distances between the residues and each of the reference structures  This is the 1th of these quantities</td></tr><tr><td width="5%">cv7_both.struct-2</td><td width="5%"><font color="blue">vector</font></td><td>the vectors containing the rmsd distances between the residues and each of the reference structures  This is the 2th of these quantities</td></tr></table></span>: <div class="tooltip" style="color:green">SECONDARY_STRUCTURE_RMSD<div class="right">Calclulate the distance between segments of a protein and a reference structure of interest <a href="https://www.plumed.org/doc-master/user-doc/html/_s_e_c_o_n_d_a_r_y__s_t_r_u_c_t_u_r_e__r_m_s_d.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">BONDLENGTH<div class="right">the length to use for bonds<i></i></div></div>=0.17 <div class="tooltip">ATOMS<div class="right">this is the full list of atoms that we are investigating<i></i></div></div>=1,5,7,8,9,10,12,14,19,20,21,23,25,38,39,40,42,44,52,53,54,56,58,66,67,68,70,72,80,81,82,84,86,100,101,102,104,106,114,115,116,118,120,128,129,130,132,134,142,143,144,146,148,156,157,158,160,162,170,171,172,174,176,181,182,183,185,187,195,196,197,199,201,209,210,211,213,215,221,222,223,225,227,240,241,242,244,246,252,253,254,256,258,276,277,278,280,282,288,289,290,292,294,312,313,314,316,318,334,335,336,338,340,348,349,350,352,354,358,359,360,362,364,377,378,379,381,383,391,392,393,395,397,410,411,412,416,418,424,425,426,428,430,446,447,448,450,452,468,469,470,472,474,480,481,482,484,486,494,495,496,498,500,518,519,520,524,526,532,533,534,536,538,549,550,551,553,555,563,564,565,567,569,575,576,577,579,581,587,588,589,591,593,603,604,605,607,609,622,623,624,626,628,636,637,638,640,642,650,651,652,654,656,672,673,674,676,678,679,680,681,683,685,693,694 <div class="tooltip">TYPE<div class="right"> the manner in which RMSD alignment is performed<i></i></div></div>=DRMSD <div class="tooltip">NOPBC<div class="right"> ignore the periodic boundary conditions<i></i></div></div> <div class="tooltip">SEGMENT1<div class="right">this is the lists of atoms in the segment that are being considered<i></i></div></div>=0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44 <div class="tooltip">SEGMENT2<div class="right">this is the lists of atoms in the segment that are being considered<i></i></div></div>=0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,35,36,37,38,39,40,41,42,43,44,45,46,47,48,49 <div class="tooltip">SEGMENT3<div class="right">this is the lists of atoms in the segment that are being considered<i></i></div></div>=0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,40,41,42,43,44,45,46,47,48,49,50,51,52,53,54 <div class="tooltip">SEGMENT4<div class="right">this is the lists of atoms in the segment that are being considered<i></i></div></div>=0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,45,46,47,48,49,50,51,52,53,54,55,56,57,58,59 <div class="tooltip">SEGMENT5<div class="right">this is the lists of atoms in the segment that are being considered<i></i></div></div>=0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,50,51,52,53,54,55,56,57,58,59,60,61,62,63,64 <div class="tooltip">STRUCTURE1<div class="right">the reference structure<i></i></div></div>=1.244,-4.62,-2.127,-0.016,-4.5,-1.395,0.105,-5.089,0.024,-0.287,-3,-1.301,0.55,-2.245,-0.822,-1.445,-2.551,-1.779,-1.752,-1.13,-1.677,-2.113,-0.55,-3.059,-2.906,-0.961,-0.689,-3.867,-1.738,-0.695,-2.774,0.034,0.19,-3.788,0.331,1.201,-3.188,0.3,2.624,-4.294,1.743,0.937,-3.503,2.671,0.821,4.746,-2.363,0.188,3.427,-1.839,0.545,3.135,-1.958,2.074,3.346,-0.365,0.181,4.237,0.412,0.521,2.261,0.013,-0.487,2.024,1.401,-0.875,1.489,1.514,-2.313,0.914,1.902,0.044,-0.173,1.33,0.052,1.202,2.94,0.828,0.19,3.507,1.718,0.772,3.801,3.104,-0.229,4.791,1.038,0.523,5.771,0.996 <div class="tooltip">STRUCTURE2<div class="right">the reference structure<i></i></div></div>=-1.439,-5.122,-1.144,-0.816,-3.803,-1.013,0.099,-3.509,-2.206,-1.928,-2.77,-0.952,-2.991,-2.97,-1.551,-1.698,-1.687,-0.215,-2.681,-0.613,-0.143,-3.323,-0.477,1.267,-1.984,0.681,-0.574,-0.807,0.921,-0.273,-2.716,1.492,-1.329,-2.196,2.731,-1.883,-2.263,2.692,-3.418,-2.989,3.949,-1.433,-4.214,3.989,-1.583,2.464,-4.352,2.149,3.078,-3.17,1.541,3.398,-3.415,0.06,2.08,-2.021,1.639,0.938,-2.178,1.225,2.525,-0.886,2.183,1.692,0.303,2.346,1.541,0.665,3.842,2.42,1.41,1.608,3.567,1.733,1.937,1.758,1.976,0.6,2.373,2.987,-0.238,2.367,2.527,-1.72,1.684,4.331,-0.148,0.486,4.43,-0.415     <span style="color:blue" class="comment"># Action input conctinues with 698 further SEGMENTn keywords, </span>
<b name="data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7_low" onclick='showPath("data/DHH1N_sampling/BEMD/CV7/plumed.6.dat","data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7_low","data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7_low","blue")'>cv7_low</b><span style="display:none;" id="data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7_low">The LOWEST action with label <b>cv7_low</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cv7_low</td><td width="5%"><font color="blue">vector</font></td><td>the smallest element in the input vector</td></tr></table></span>: <div class="tooltip" style="color:green">LOWEST<div class="right">This function can be used to find the lowest colvar by magnitude in a set. <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_w_e_s_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input to this function<i></i></div></div>=<b name="data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7_both">cv7_both.struct-1</b>,<b name="data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7_both">cv7_both.struct-2</b> 
<b name="data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7_lt" onclick='showPath("data/DHH1N_sampling/BEMD/CV7/plumed.6.dat","data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7_lt","data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7_lt","blue")'>cv7_lt</b><span style="display:none;" id="data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7_lt">The LESS_THAN action with label <b>cv7_lt</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cv7_lt</td><td width="5%"><font color="blue">vector</font></td><td>the vector obtained by doing an element-wise application of a function that is one if the input is less than a threshold to the input vectors</td></tr></table></span>: <div class="tooltip" style="color:green">LESS_THAN<div class="right">Use a switching function to determine how many of the input variables are less than a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_l_e_s_s__t_h_a_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input to this function<i></i></div></div>=<b name="data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7_low">cv7_low</b> <div class="tooltip">SWITCH<div class="right">This keyword is used if you want to employ an alternative to the continuous swiching function defined above<i></i></div></div>={RATIONAL R_0=0.08 D_0=0.0 NN=8 MM=12} 
<b name="data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7" onclick='showPath("data/DHH1N_sampling/BEMD/CV7/plumed.6.dat","data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7","data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7","black")'>cv7</b><span style="display:none;" id="data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7">The SUM action with label <b>cv7</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cv7</td><td width="5%"><font color="black">scalar</font></td><td>the sum of all the elements in the input vector</td></tr></table></span>: <div class="tooltip" style="color:green">SUM<div class="right">Calculate the sum of the arguments <a href="https://www.plumed.org/doc-master/user-doc/html/_s_u_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input to this function<i></i></div></div>=<b name="data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7_lt">cv7_lt</b> <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO 
<span style="color:blue"># --- End of included input --- </span></span><br/><b name="data/DHH1N_sampling/BEMD/CV7/plumed.6.datlwall" onclick='showPath("data/DHH1N_sampling/BEMD/CV7/plumed.6.dat","data/DHH1N_sampling/BEMD/CV7/plumed.6.datlwall","data/DHH1N_sampling/BEMD/CV7/plumed.6.datlwall","black")'>lwall</b><span style="display:none;" id="data/DHH1N_sampling/BEMD/CV7/plumed.6.datlwall">The LOWER_WALLS action with label <b>lwall</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">lwall.bias</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">lwall.force2</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the squared force due to this bias potential</td></tr></table></span>: <div class="tooltip" style="color:green">LOWER_WALLS<div class="right">Defines a wall for the value of one or more collective variables, <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the arguments on which the bias is acting<i></i></div></div>=<b name="data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7">cv7</b> <div class="tooltip">AT<div class="right">the positions of the wall<i></i></div></div>=0.0 <div class="tooltip">KAPPA<div class="right">the force constant for the wall<i></i></div></div>=30.0
<b name="data/DHH1N_sampling/BEMD/CV7/plumed.6.datuwall" onclick='showPath("data/DHH1N_sampling/BEMD/CV7/plumed.6.dat","data/DHH1N_sampling/BEMD/CV7/plumed.6.datuwall","data/DHH1N_sampling/BEMD/CV7/plumed.6.datuwall","black")'>uwall</b><span style="display:none;" id="data/DHH1N_sampling/BEMD/CV7/plumed.6.datuwall">The UPPER_WALLS action with label <b>uwall</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">uwall.bias</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">uwall.force2</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the squared force due to this bias potential</td></tr></table></span>: <div class="tooltip" style="color:green">UPPER_WALLS<div class="right">Defines a wall for the value of one or more collective variables, <a href="https://www.plumed.org/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the arguments on which the bias is acting<i></i></div></div>=<b name="data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7">cv7</b> <div class="tooltip">AT<div class="right">the positions of the wall<i></i></div></div>=8.0 <div class="tooltip">KAPPA<div class="right">the force constant for the wall<i></i></div></div>=30.0
<br/><b name="data/DHH1N_sampling/BEMD/CV7/plumed.6.datmetad" onclick='showPath("data/DHH1N_sampling/BEMD/CV7/plumed.6.dat","data/DHH1N_sampling/BEMD/CV7/plumed.6.datmetad","data/DHH1N_sampling/BEMD/CV7/plumed.6.datmetad","black")'>metad</b><span style="display:none;" id="data/DHH1N_sampling/BEMD/CV7/plumed.6.datmetad">The METAD action with label <b>metad</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">metad.bias</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the bias potential</td></tr></table></span>: <div class="tooltip" style="color:green">METAD<div class="right">Used to performed metadynamics on one or more collective variables. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_e_t_a_d.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7">cv7</b> <div class="tooltip">PACE<div class="right">the frequency for hill addition<i></i></div></div>=2500 <div class="tooltip">HEIGHT<div class="right">the heights of the Gaussian hills<i></i></div></div>=0.3 <div class="tooltip">SIGMA<div class="right">the widths of the Gaussian hills<i></i></div></div>=0.1 <div class="tooltip">FILE<div class="right"> a file in which the list of added hills is stored<i></i></div></div>=HILLS <div class="tooltip">GRID_MIN<div class="right">the lower bounds for the grid<i></i></div></div>=0.0 <div class="tooltip">GRID_MAX<div class="right">the upper bounds for the grid<i></i></div></div>=30.0 <div class="tooltip">GRID_SPACING<div class="right">the approximate grid spacing (to be used as an alternative or together with GRID_BIN)<i></i></div></div>=0.025
<br/><span style="color:blue" class="comment">#PRINT STRIDE=10 ARG=cv7,metad.bias FILE=COLVAR</span>
<div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=10 <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/DHH1N_sampling/BEMD/CV7/plumed.6.datcv7">cv7</b>,<b name="data/DHH1N_sampling/BEMD/CV7/plumed.6.datmetad">metad.bias</b>,<b name="data/DHH1N_sampling/BEMD/CV7/plumed.6.datuwall">uwall.bias</b>,<b name="data/DHH1N_sampling/BEMD/CV7/plumed.6.datlwall">lwall.bias</b> <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=COLVAR
</pre>
{% endraw %}