**Project ID:** [plumID:19.058]({{ '/' | absolute_url }}eggs/19/058/)  
**Source:** plumed_sphere.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [zipped raw stdout](plumed_sphere.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_sphere.dat.plumed.stderr.txt.zip) - [stderr](plumed_sphere.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed_sphere.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_sphere.dat.plumed_master.stderr.txt.zip) - [stderr](plumed_sphere.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/plumed_sphere.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed_sphere.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed_sphere.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<div class="tooltip" style="color:green">RESTART<div class="right">Activate restart. <a href="https://www.plumed.org/doc-master/user-doc/html/_r_e_s_t_a_r_t.html" style="color:green">More details</a><i></i></div></div>
<br/><span style="color:blue" class="comment"># This should be the COM of whole molecule</span>
<span style="display:none;" id="data/plumed_sphere.dat">The RESTART action with label <b></b> calculates something</span><div class="tooltip" style="color:green">COM<div class="right">Calculate the center of mass for a group of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the list of atoms which are involved the virtual atom's definition<i></i></div></div>=1-216 <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/plumed_sphere.datcom" onclick='showPath("data/plumed_sphere.dat","data/plumed_sphere.datcom","data/plumed_sphere.datcom","violet")'>com</b><span style="display:none;" id="data/plumed_sphere.datcom">The COM action with label <b>com</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">com</td><td width="5%"><font color="violet">atoms</font></td><td>virtual atom calculated by COM action</td></tr></table></span>
<br/><span style="color:blue" class="comment"># The difference between the largest and smallest distance</span>
<span id="data/plumed_sphere.datd1_short"><div class="tooltip" style="color:green">DISTANCES<div class="right">Calculate the distances between multiple piars of atoms This action is <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/plumed_sphere.datd1");'>a shortcut</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">More details</a><i></i></div></div> <div class="tooltip">GROUPA<div class="right">Calculate the distances between all the atoms in GROUPA and all the atoms in GROUPB<i></i></div></div>=<b name="data/plumed_sphere.datcom">com</b> <div class="tooltip">GROUPB<div class="right">Calculate the distances between all the atoms in GROUPA and all the atoms in GROUPB<i></i></div></div>=1-216 <div class="tooltip">MIN<div class="right">calculate the minimum value<i></i></div></div>={BETA=10} <div class="tooltip">MAX<div class="right">calculate the maximum value<i></i></div></div>={BETA=.001} <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/plumed_sphere.datd1" onclick='showPath("data/plumed_sphere.dat","data/plumed_sphere.datd1","data/plumed_sphere.datd1_shortcut","blue")'>d1</b><span style="display:none;" id="data/plumed_sphere.datd1_shortcut">The DISTANCES action with label <b>d1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d1</td><td width="5%"><font color="blue">vector</font></td><td>the value calculated by this action</td></tr><tr><td width="5%">d1_min</td><td width="5%"><font color="black">scalar</font></td><td>the minimum colvar</td></tr><tr><td width="5%">d1_max</td><td width="5%"><font color="black">scalar</font></td><td>the maximum colvar</td></tr></table></span>
</span><span id="data/plumed_sphere.datd1_long" style="display:none;"><span style="color:blue" class="comment"># PLUMED interprets the command:
</span><span class="toggler" style="color:red" onclick='toggleDisplay("data/plumed_sphere.datd1")'># DISTANCES GROUPA=com GROUPB=1-216 MIN={BETA=10} MAX={BETA=.001} LABEL=d1</span>
<span style="color:blue" class="comment"># as follows (Click the red comment above to revert to the short version of the input):</span>
<b name="data/plumed_sphere.datd1_vatom1" onclick='showPath("data/plumed_sphere.dat","data/plumed_sphere.datd1_vatom1","data/plumed_sphere.datd1_vatom1","violet")'>d1_vatom1</b><span style="display:none;" id="data/plumed_sphere.datd1_vatom1">The CENTER_FAST action with label <b>d1_vatom1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d1_vatom1</td><td width="5%"><font color="violet">atoms</font></td><td>virtual atom calculated by CENTER_FAST action</td></tr></table></span>: <div class="tooltip" style="color:green">CENTER<div class="right">Calculate the center for a group of atoms, with arbitrary weights. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_e_n_t_e_r.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the group of atoms that you are calculating the Gyration Tensor for<i></i></div></div>=<b name="data/plumed_sphere.datcom">com</b>,1 
<b name="data/plumed_sphere.datd1_vatom2" onclick='showPath("data/plumed_sphere.dat","data/plumed_sphere.datd1_vatom2","data/plumed_sphere.datd1_vatom2","violet")'>d1_vatom2</b><span style="display:none;" id="data/plumed_sphere.datd1_vatom2">The CENTER_FAST action with label <b>d1_vatom2</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d1_vatom2</td><td width="5%"><font color="violet">atoms</font></td><td>virtual atom calculated by CENTER_FAST action</td></tr></table></span>: <div class="tooltip" style="color:green">CENTER<div class="right">Calculate the center for a group of atoms, with arbitrary weights. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_e_n_t_e_r.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the group of atoms that you are calculating the Gyration Tensor for<i></i></div></div>=<b name="data/plumed_sphere.datcom">com</b>,2 
<b name="data/plumed_sphere.datd1_vatom3" onclick='showPath("data/plumed_sphere.dat","data/plumed_sphere.datd1_vatom3","data/plumed_sphere.datd1_vatom3","violet")'>d1_vatom3</b><span style="display:none;" id="data/plumed_sphere.datd1_vatom3">The CENTER_FAST action with label <b>d1_vatom3</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d1_vatom3</td><td width="5%"><font color="violet">atoms</font></td><td>virtual atom calculated by CENTER_FAST action</td></tr></table></span>: <div class="tooltip" style="color:green">CENTER<div class="right">Calculate the center for a group of atoms, with arbitrary weights. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_e_n_t_e_r.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the group of atoms that you are calculating the Gyration Tensor for<i></i></div></div>=<b name="data/plumed_sphere.datcom">com</b>,3 
<b name="data/plumed_sphere.datd1_vatom4" onclick='showPath("data/plumed_sphere.dat","data/plumed_sphere.datd1_vatom4","data/plumed_sphere.datd1_vatom4","violet")'>d1_vatom4</b><span style="display:none;" id="data/plumed_sphere.datd1_vatom4">The CENTER_FAST action with label <b>d1_vatom4</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d1_vatom4</td><td width="5%"><font color="violet">atoms</font></td><td>virtual atom calculated by CENTER_FAST action</td></tr></table></span>: <div class="tooltip" style="color:green">CENTER<div class="right">Calculate the center for a group of atoms, with arbitrary weights. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_e_n_t_e_r.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the group of atoms that you are calculating the Gyration Tensor for<i></i></div></div>=<b name="data/plumed_sphere.datcom">com</b>,4 
<b name="data/plumed_sphere.datd1_vatom5" onclick='showPath("data/plumed_sphere.dat","data/plumed_sphere.datd1_vatom5","data/plumed_sphere.datd1_vatom5","violet")'>d1_vatom5</b><span style="display:none;" id="data/plumed_sphere.datd1_vatom5">The CENTER_FAST action with label <b>d1_vatom5</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d1_vatom5</td><td width="5%"><font color="violet">atoms</font></td><td>virtual atom calculated by CENTER_FAST action</td></tr></table></span>: <div class="tooltip" style="color:green">CENTER<div class="right">Calculate the center for a group of atoms, with arbitrary weights. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_e_n_t_e_r.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the group of atoms that you are calculating the Gyration Tensor for<i></i></div></div>=<b name="data/plumed_sphere.datcom">com</b>,5 
<b name="data/plumed_sphere.datd1_vatom6" onclick='showPath("data/plumed_sphere.dat","data/plumed_sphere.datd1_vatom6","data/plumed_sphere.datd1_vatom6","violet")'>d1_vatom6</b><span style="display:none;" id="data/plumed_sphere.datd1_vatom6">The CENTER_FAST action with label <b>d1_vatom6</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d1_vatom6</td><td width="5%"><font color="violet">atoms</font></td><td>virtual atom calculated by CENTER_FAST action</td></tr></table></span>: <div class="tooltip" style="color:green">CENTER<div class="right">Calculate the center for a group of atoms, with arbitrary weights. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_e_n_t_e_r.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the group of atoms that you are calculating the Gyration Tensor for<i></i></div></div>=<b name="data/plumed_sphere.datcom">com</b>,6 
<span style="color:blue" class="comment"># A further 216 CENTER like the ones above were also created but are not shown</span>
<b name="data/plumed_sphere.datd1_grp" onclick='showPath("data/plumed_sphere.dat","data/plumed_sphere.datd1_grp","data/plumed_sphere.datd1_grp","violet")'>d1_grp</b><span style="display:none;" id="data/plumed_sphere.datd1_grp">The GROUP action with label <b>d1_grp</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d1_grp</td><td width="5%"><font color="violet">atoms</font></td><td>indices of atoms specified in GROUP</td></tr></table></span>: <div class="tooltip" style="color:green">GROUP<div class="right">Define a group of atoms so that a particular list of atoms can be referenced with a single label in definitions of CVs or virtual atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_g_r_o_u_p.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the numerical indexes for the set of atoms in the group<i></i></div></div>=<b name="data/plumed_sphere.datd1_vatom1">d1_vatom1</b>,<b name="data/plumed_sphere.datd1_vatom2">d1_vatom2</b>,<b name="data/plumed_sphere.datd1_vatom3">d1_vatom3</b>,<b name="data/plumed_sphere.datd1_vatom4">d1_vatom4</b>,<b name="data/plumed_sphere.datd1_vatom5">d1_vatom5</b>,<b name="data/plumed_sphere.datd1_vatom6">d1_vatom6</b>,d1_vatom7,d1_vatom8,d1_vatom9,d1_vatom10,d1_vatom11,d1_vatom12,d1_vatom13,d1_vatom14,d1_vatom15,d1_vatom16,d1_vatom17,d1_vatom18,d1_vatom19,d1_vatom20,d1_vatom21,d1_vatom22,d1_vatom23,d1_vatom24,d1_vatom25,d1_vatom26,d1_vatom27,d1_vatom28,d1_vatom29,d1_vatom30,d1_vatom31,d1_vatom32,d1_vatom33,d1_vatom34,d1_vatom35,d1_vatom36,d1_vatom37,d1_vatom38,d1_vatom39,d1_vatom40,d1_vatom41,d1_vatom42,d1_vatom43,d1_vatom44,d1_vatom45,d1_vatom46,d1_vatom47,d1_vatom48,d1_vatom49,d1_vatom50,d1_vatom51,d1_vatom52,d1_vatom53,d1_vatom54,d1_vatom55,d1_vatom56,d1_vatom57,d1_vatom58,d1_vatom59,d1_vatom60,d1_vatom61,d1_vatom62,d1_vatom63,d1_vatom64,d1_vatom65,d1_vatom66,d1_vatom67,d1_vatom68,d1_vatom69,d1_vatom70,d1_vatom71,d1_vatom72,d1_vatom73,d1_vatom74,d1_vatom75,d1_vatom76,d1_vatom77,d1_vatom78,d1_vatom79,d1_vatom80,d1_vatom81,d1_vatom82,d1_vatom83,d1_vatom84,d1_vatom85,d1_vatom86,d1_vatom87,d1_vatom88,d1_vatom89,d1_vatom90,d1_vatom91,d1_vatom92,d1_vatom93,d1_vatom94,d1_vatom95,d1_vatom96,d1_vatom97,d1_vatom98,d1_vatom99,d1_vatom100,d1_vatom101,d1_vatom102,d1_vatom103,d1_vatom104,d1_vatom105,d1_vatom106,d1_vatom107,d1_vatom108,d1_vatom109,d1_vatom110,d1_vatom111,d1_vatom112,d1_vatom113,d1_vatom114,d1_vatom115,d1_vatom116,d1_vatom117,d1_vatom118,d1_vatom119,d1_vatom120,d1_vatom121,d1_vatom122,d1_vatom123,d1_vatom124,d1_vatom125,d1_vatom126,d1_vatom127,d1_vatom128,d1_vatom129,d1_vatom130,d1_vatom131,d1_vatom132,d1_vatom133,d1_vatom134,d1_vatom135,d1_vatom136,d1_vatom137,d1_vatom138,d1_vatom139,d1_vatom140,d1_vatom141,d1_vatom142,d1_vatom143,d1_vatom144,d1_vatom145,d1_vatom146,d1_vatom147,d1_vatom148,d1_vatom149,d1_vatom150,d1_vatom151,d1_vatom152,d1_vatom153,d1_vatom154,d1_vatom155,d1_vatom156,d1_vatom157,d1_vatom158,d1_vatom159,d1_vatom160,d1_vatom161,d1_vatom162,d1_vatom163,d1_vatom164,d1_vatom165,d1_vatom166,d1_vatom167,d1_vatom168,d1_vatom169,d1_vatom170,d1_vatom171,d1_vatom172,d1_vatom173,d1_vatom174,d1_vatom175,d1_vatom176,d1_vatom177,d1_vatom178,d1_vatom179,d1_vatom180,d1_vatom181,d1_vatom182,d1_vatom183,d1_vatom184,d1_vatom185,d1_vatom186,d1_vatom187,d1_vatom188,d1_vatom189,d1_vatom190,d1_vatom191,d1_vatom192,d1_vatom193,d1_vatom194,d1_vatom195,d1_vatom196,d1_vatom197,d1_vatom198,d1_vatom199,d1_vatom200,d1_vatom201,d1_vatom202,d1_vatom203,d1_vatom204,d1_vatom205,d1_vatom206,d1_vatom207,d1_vatom208,d1_vatom209,d1_vatom210,d1_vatom211,d1_vatom212,d1_vatom213,d1_vatom214,d1_vatom215,d1_vatom216 
<b name="data/plumed_sphere.datd1" onclick='showPath("data/plumed_sphere.dat","data/plumed_sphere.datd1","data/plumed_sphere.datd1","blue")'>d1</b><span style="display:none;" id="data/plumed_sphere.datd1">The DISTANCE action with label <b>d1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d1</td><td width="5%"><font color="blue">vector</font></td><td>the DISTANCE for each set of specified atoms</td></tr></table></span>: <div class="tooltip" style="color:green">DISTANCE<div class="right">Calculate the distance between a pair of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS1<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=<b name="data/plumed_sphere.datcom">com</b>,1 <div class="tooltip">ATOMS2<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=<b name="data/plumed_sphere.datcom">com</b>,2 <div class="tooltip">ATOMS3<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=<b name="data/plumed_sphere.datcom">com</b>,3 <div class="tooltip">ATOMS4<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=<b name="data/plumed_sphere.datcom">com</b>,4 <div class="tooltip">ATOMS5<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=<b name="data/plumed_sphere.datcom">com</b>,5     <span style="color:blue" class="comment"># Action input conctinues with 211 further ATOMSn keywords, </span>
<b name="data/plumed_sphere.datd1_me_min" onclick='showPath("data/plumed_sphere.dat","data/plumed_sphere.datd1_me_min","data/plumed_sphere.datd1_me_min","blue")'>d1_me_min</b><span style="display:none;" id="data/plumed_sphere.datd1_me_min">The CUSTOM action with label <b>d1_me_min</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d1_me_min</td><td width="5%"><font color="blue">vector</font></td><td>the vector obtained by doing an element-wise application of an arbitrary function to the input vectors</td></tr></table></span>: <div class="tooltip" style="color:green">CUSTOM<div class="right">Calculate a combination of variables using a custom expression. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_u_s_t_o_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input to this function<i></i></div></div>=<b name="data/plumed_sphere.datd1">d1</b> <div class="tooltip">FUNC<div class="right">the function you wish to evaluate<i></i></div></div>=exp(10/x <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO 
<b name="data/plumed_sphere.datd1_mec_min" onclick='showPath("data/plumed_sphere.dat","data/plumed_sphere.datd1_mec_min","data/plumed_sphere.datd1_mec_min","black")'>d1_mec_min</b><span style="display:none;" id="data/plumed_sphere.datd1_mec_min">The SUM action with label <b>d1_mec_min</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d1_mec_min</td><td width="5%"><font color="black">scalar</font></td><td>the sum of all the elements in the input vector</td></tr></table></span>: <div class="tooltip" style="color:green">SUM<div class="right">Calculate the sum of the arguments <a href="https://www.plumed.org/doc-master/user-doc/html/_s_u_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input to this function<i></i></div></div>=<b name="data/plumed_sphere.datd1_me_min">d1_me_min</b> <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO 
<b name="data/plumed_sphere.datd1_min" onclick='showPath("data/plumed_sphere.dat","data/plumed_sphere.datd1_min","data/plumed_sphere.datd1_min","black")'>d1_min</b><span style="display:none;" id="data/plumed_sphere.datd1_min">The CUSTOM action with label <b>d1_min</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d1_min</td><td width="5%"><font color="black">scalar</font></td><td>an arbitrary function</td></tr></table></span>: <div class="tooltip" style="color:green">CUSTOM<div class="right">Calculate a combination of variables using a custom expression. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_u_s_t_o_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input to this function<i></i></div></div>=<b name="data/plumed_sphere.datd1_mec_min">d1_mec_min</b> <div class="tooltip">FUNC<div class="right">the function you wish to evaluate<i></i></div></div>=10/log(x <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO 
<b name="data/plumed_sphere.datd1_me_max" onclick='showPath("data/plumed_sphere.dat","data/plumed_sphere.datd1_me_max","data/plumed_sphere.datd1_me_max","blue")'>d1_me_max</b><span style="display:none;" id="data/plumed_sphere.datd1_me_max">The CUSTOM action with label <b>d1_me_max</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d1_me_max</td><td width="5%"><font color="blue">vector</font></td><td>the vector obtained by doing an element-wise application of an arbitrary function to the input vectors</td></tr></table></span>: <div class="tooltip" style="color:green">CUSTOM<div class="right">Calculate a combination of variables using a custom expression. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_u_s_t_o_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input to this function<i></i></div></div>=<b name="data/plumed_sphere.datd1">d1</b> <div class="tooltip">FUNC<div class="right">the function you wish to evaluate<i></i></div></div>=exp(x/.001 <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO 
<b name="data/plumed_sphere.datd1_mec_max" onclick='showPath("data/plumed_sphere.dat","data/plumed_sphere.datd1_mec_max","data/plumed_sphere.datd1_mec_max","black")'>d1_mec_max</b><span style="display:none;" id="data/plumed_sphere.datd1_mec_max">The SUM action with label <b>d1_mec_max</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d1_mec_max</td><td width="5%"><font color="black">scalar</font></td><td>the sum of all the elements in the input vector</td></tr></table></span>: <div class="tooltip" style="color:green">SUM<div class="right">Calculate the sum of the arguments <a href="https://www.plumed.org/doc-master/user-doc/html/_s_u_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input to this function<i></i></div></div>=<b name="data/plumed_sphere.datd1_me_max">d1_me_max</b> <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO 
<b name="data/plumed_sphere.datd1_max" onclick='showPath("data/plumed_sphere.dat","data/plumed_sphere.datd1_max","data/plumed_sphere.datd1_max","black")'>d1_max</b><span style="display:none;" id="data/plumed_sphere.datd1_max">The CUSTOM action with label <b>d1_max</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d1_max</td><td width="5%"><font color="black">scalar</font></td><td>an arbitrary function</td></tr></table></span>: <div class="tooltip" style="color:green">CUSTOM<div class="right">Calculate a combination of variables using a custom expression. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_u_s_t_o_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input to this function<i></i></div></div>=<b name="data/plumed_sphere.datd1_mec_max">d1_mec_max</b> <div class="tooltip">FUNC<div class="right">the function you wish to evaluate<i></i></div></div>=<b name="data/plumed_sphere.dat">.001*log(x</b> <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO 
<span style="color:blue"># --- End of included input --- </span></span><br/><div class="tooltip" style="color:green">MOVINGRESTRAINT<div class="right">Add a time-dependent, harmonic restraint on one or more variables. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_v_i_n_g_r_e_s_t_r_a_i_n_t.html" style="color:green">More details</a><i></i></div></div> ...
    <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/plumed_sphere.datd1">d1.min</b>
    <div class="tooltip">STEP0<div class="right">This keyword appears multiple times as STEPx with x=0,1,2,<i></i></div></div>=0      <div class="tooltip">AT0<div class="right">ATx is equal to the position of the restraint at time STEPx<i></i></div></div>=0.5  <div class="tooltip">KAPPA0<div class="right">KAPPAx is equal to the value of the force constants at time STEPx<i></i></div></div>=0.0
    <div class="tooltip">STEP1<div class="right">This keyword appears multiple times as STEPx with x=0,1,2,<i></i></div></div>=20000  <div class="tooltip">AT1<div class="right">ATx is equal to the position of the restraint at time STEPx<i></i></div></div>=0.5  <div class="tooltip">KAPPA1<div class="right">KAPPAx is equal to the value of the force constants at time STEPx<i></i></div></div>=50000.0
    <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/plumed_sphere.datm1" onclick='showPath("data/plumed_sphere.dat","data/plumed_sphere.datm1","data/plumed_sphere.datm1","black")'>m1</b><span style="display:none;" id="data/plumed_sphere.datm1">The MOVINGRESTRAINT action with label <b>m1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">m1.bias</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">m1.force2</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the squared force due to this bias potential</td></tr><tr><td width="5%">m1.d1_min_cntr</td><td width="5%"><font color="black">scalar</font></td><td>one or multiple instances of this quantity can be referenced elsewhere in the input file. these quantities will named with  the arguments of the bias followed by the character string _cntr. These quantities give the instantaneous position of the center of the harmonic potential. This particular component measures this quantity for the input CV named d1_min</td></tr><tr><td width="5%">m1.d1_min_work</td><td width="5%"><font color="black">scalar</font></td><td>one or multiple instances of this quantity can be referenced elsewhere in the input file. These quantities will named with the arguments of the bias followed by the character string _work. These quantities tell the user how much work has been done by the potential in dragging the system along the various colvar axis. This particular component measures this quantity for the input CV named d1_min</td></tr><tr><td width="5%">m1.d1_min_kappa</td><td width="5%"><font color="black">scalar</font></td><td>one or multiple instances of this quantity can be referenced elsewhere in the input file. These quantities will named with the arguments of the bias followed by the character string _kappa. These quantities tell the user the time dependent value of kappa. This particular component measures this quantity for the input CV named d1_min</td></tr><tr><td width="5%">m1.work</td><td width="5%"><font color="black">scalar</font></td><td>the total work performed changing this restraint</td></tr></table></span>
    <div class="tooltip">VERSE<div class="right"> Tells plumed whether the restraint is only acting for CV larger (U) or smaller (L) than the restraint or whether it is acting on both sides (B)<i></i></div></div>=L
... MOVINGRESTRAINT
<br/><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/plumed_sphere.datd1">d1.*</b>,<b name="data/plumed_sphere.datm1">m1</b> <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=colvar <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=10
<div class="tooltip" style="color:green">FLUSH<div class="right">This command instructs plumed to flush all the open files with a user specified frequency. <a href="https://www.plumed.org/doc-master/user-doc/html/_f_l_u_s_h.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">STRIDE<div class="right">the frequency with which all the open files should be flushed<i></i></div></div>=10
</pre>
{% endraw %}