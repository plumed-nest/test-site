**Project ID:** [plumID:19.020]({{ '/' | absolute_url }}eggs/19/020/)  
**Source:** step-1/plumed.7.dat  
**Originally used with PLUMED version:** 2.2  
**Stable:** [zipped raw stdout](plumed.7.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.7.dat.plumed.stderr.txt.zip) - [stderr](plumed.7.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.7.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.7.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.7.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/step-1/plumed.7.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.7.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.7.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<div class="tooltip" style="color:green">MOLINFO<div class="right">This command is used to provide information on the molecules that are present in your system. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">STRUCTURE<div class="right">a file in pdb format containing a reference structure<i></i></div></div>=reference.pdb
<span style="display:none;" id="data/step-1/plumed.7.dat">The MOLINFO action with label <b></b> calculates something</span><div class="tooltip" style="color:green">WHOLEMOLECULES<div class="right">This action is used to rebuild molecules that can become split by the periodic boundary conditions. <a href="https://www.plumed.org/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">STRIDE<div class="right"> the frequency with which molecules are reassembled<i></i></div></div>=1 <div class="tooltip">ENTITY0<div class="right">the atoms that make up a molecule that you wish to align<i></i></div></div>=1-427
<br/><span id="data/step-1/plumed.7.data_short"><span id="data/step-1/plumed.7.datdefa_short"><b name="data/step-1/plumed.7.data" onclick='showPath("data/step-1/plumed.7.dat","data/step-1/plumed.7.data","data/step-1/plumed.7.data_shortcut","black")'>a</b><span style="display:none;" id="data/step-1/plumed.7.data_shortcut">The ALPHARMSD action with label <b>a</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">a</td><td width="5%"><font color="black">scalar</font></td><td>the value calculated by this action</td></tr></table></span>: <div class="tooltip" style="color:green">ALPHARMSD<div class="right">Probe the alpha helical content of a protein structure. This action is <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/step-1/plumed.7.data");'>a shortcut</a> and it has <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/step-1/plumed.7.datdefa");'>hidden defaults</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_a_l_p_h_a_r_m_s_d.html">More details</a><i></i></div></div> <div class="tooltip">RESIDUES<div class="right">this command is used to specify the set of residues that could conceivably form part of the secondary structure<i></i></div></div>=all <div class="tooltip">TYPE<div class="right"> the manner in which RMSD alignment is performed<i></i></div></div>=DRMSD <div class="tooltip">R_0<div class="right">The r_0 parameter of the switching function<i></i></div></div>=0.08 <div class="tooltip">NN<div class="right"> The n parameter of the switching function<i></i></div></div>=8 <div class="tooltip">MM<div class="right"> The m parameter of the switching function<i></i></div></div>=12 
</span><span id="data/step-1/plumed.7.datdefa_long" style="display:none;"><b name="data/step-1/plumed.7.data" onclick='showPath("data/step-1/plumed.7.dat","data/step-1/plumed.7.data","data/step-1/plumed.7.data_shortcut","black")'>a</b>: <div class="tooltip" style="color:green">ALPHARMSD<div class="right">Probe the alpha helical content of a protein structure. This action is <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/step-1/plumed.7.data");'>a shortcut</a> and uses the <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/step-1/plumed.7.datdefa");'>defaults shown here</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_a_l_p_h_a_r_m_s_d.html">More details</a><i></i></div></div> <div class="tooltip">RESIDUES<div class="right">this command is used to specify the set of residues that could conceivably form part of the secondary structure<i></i></div></div>=all <div class="tooltip">TYPE<div class="right"> the manner in which RMSD alignment is performed<i></i></div></div>=DRMSD <div class="tooltip">R_0<div class="right">The r_0 parameter of the switching function<i></i></div></div>=0.08 <div class="tooltip">NN<div class="right"> The n parameter of the switching function<i></i></div></div>=8 <div class="tooltip">MM<div class="right"> The m parameter of the switching function<i></i></div></div>=12  <div class="tooltip">D_0<div class="right"> The d_0 parameter of the switching function<i></i></div></div>=0.0
</span></span><span id="data/step-1/plumed.7.data_long" style="display:none;"><span style="color:blue" class="comment"># PLUMED interprets the command:
</span><span class="toggler" style="color:red" onclick='toggleDisplay("data/step-1/plumed.7.data")'># a: ALPHARMSD RESIDUES=all TYPE=DRMSD R_0=0.08 NN=8 MM=12 </span>
<span style="color:blue" class="comment"># as follows (Click the red comment above to revert to the short version of the input):</span>
<b name="data/step-1/plumed.7.data_rmsd" onclick='showPath("data/step-1/plumed.7.dat","data/step-1/plumed.7.data_rmsd","data/step-1/plumed.7.data_rmsd","blue")'>a_rmsd</b><span style="display:none;" id="data/step-1/plumed.7.data_rmsd">The SECONDARY_STRUCTURE_RMSD action with label <b>a_rmsd</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">a_rmsd</td><td width="5%"><font color="blue">vector</font></td><td>the value calculated by this action</td></tr></table></span>: <div class="tooltip" style="color:green">SECONDARY_STRUCTURE_RMSD<div class="right">Calclulate the distance between segments of a protein and a reference structure of interest <a href="https://www.plumed.org/doc-master/user-doc/html/_s_e_c_o_n_d_a_r_y__s_t_r_u_c_t_u_r_e__r_m_s_d.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">BONDLENGTH<div class="right">the length to use for bonds<i></i></div></div>=0.17 <div class="tooltip">ATOMS<div class="right">this is the full list of atoms that we are investigating<i></i></div></div>=7,9,11,19,20,21,23,25,31,32,33,35,37,46,47,48,50,52,58,59,60,62,64,74,75,76,78,80,85,86,87,89,91,97,98,99,101,103,116,117,118,120,122,131,132,133,135,137,155,156,157,159,161,179,180,181,183,185,198,199,200,202,204,208,209,210,212,214,225,226,227,229,231,249,250,251,253,255,268,269,270,272,274,278,279,280,282,284,293,294,295,297,299,317,318,319,321,323,341,342,343,345,347,358,359,360,362,364,373,374,375,377,379,385,386,387,389,391,396,397,398,400,402,406,407,408,410,412,420,421 <div class="tooltip">TYPE<div class="right"> the manner in which RMSD alignment is performed<i></i></div></div>=DRMSD <div class="tooltip">SEGMENT1<div class="right">this is the lists of atoms in the segment that are being considered<i></i></div></div>=0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29 <div class="tooltip">SEGMENT2<div class="right">this is the lists of atoms in the segment that are being considered<i></i></div></div>=5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34 <div class="tooltip">SEGMENT3<div class="right">this is the lists of atoms in the segment that are being considered<i></i></div></div>=10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39 <div class="tooltip">SEGMENT4<div class="right">this is the lists of atoms in the segment that are being considered<i></i></div></div>=15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44 <div class="tooltip">SEGMENT5<div class="right">this is the lists of atoms in the segment that are being considered<i></i></div></div>=20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48,49 <div class="tooltip">STRUCTURE1<div class="right">the reference structure<i></i></div></div>=0.733,0.519,5.298,1.763,0.81,4.301,3.166,0.543,4.881,1.527,-0.045,3.053,1.646,0.436,1.928,1.18,-1.312,3.254,0.924,-2.203,2.126,0.65,-3.626,2.626,-0.239,-1.711,1.261,-0.19,-1.815,0.032,-1.28,-1.172,1.891,-2.416,-0.661,1.127,-3.548,-0.217,2.056,-1.964,0.529,0.276,-2.364,0.659,-0.88,-1.13,1.391,0.856,-0.62,2.565,0.148,0.228,3.439,1.077,0.231,2.129,-1.032,0.179,2.733,-2.099,1.028,1.084,-0.833,1.872,0.593,-1.919,2.85,-0.462,-1.397,1.02,0.02,-3.049,1.317,0.227,-4.224,-0.051,-0.684,-2.696,-0.927,-1.261,-3.713,-1.933,-2.219,-3.074,-1.663,-0.171,-4.475,-1.916,-0.296,-5.673     <span style="color:blue" class="comment"># Action input conctinues with 16 further SEGMENTn keywords, </span>
<b name="data/step-1/plumed.7.data_lt" onclick='showPath("data/step-1/plumed.7.dat","data/step-1/plumed.7.data_lt","data/step-1/plumed.7.data_lt","blue")'>a_lt</b><span style="display:none;" id="data/step-1/plumed.7.data_lt">The LESS_THAN action with label <b>a_lt</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">a_lt</td><td width="5%"><font color="blue">vector</font></td><td>the vector obtained by doing an element-wise application of a function that is one if the input is less than a threshold to the input vectors</td></tr></table></span>: <div class="tooltip" style="color:green">LESS_THAN<div class="right">Use a switching function to determine how many of the input variables are less than a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_l_e_s_s__t_h_a_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input to this function<i></i></div></div>=<b name="data/step-1/plumed.7.data_rmsd">a_rmsd</b> <div class="tooltip">SWITCH<div class="right">This keyword is used if you want to employ an alternative to the continuous swiching function defined above<i></i></div></div>={RATIONAL R_0=0.08 D_0=0.0 NN=8 MM=12} 
<b name="data/step-1/plumed.7.data" onclick='showPath("data/step-1/plumed.7.dat","data/step-1/plumed.7.data","data/step-1/plumed.7.data","black")'>a</b><span style="display:none;" id="data/step-1/plumed.7.data">The SUM action with label <b>a</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">a</td><td width="5%"><font color="black">scalar</font></td><td>the sum of all the elements in the input vector</td></tr></table></span>: <div class="tooltip" style="color:green">SUM<div class="right">Calculate the sum of the arguments <a href="https://www.plumed.org/doc-master/user-doc/html/_s_u_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input to this function<i></i></div></div>=<b name="data/step-1/plumed.7.data_lt">a_lt</b> <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO 
<span style="color:blue"># --- End of included input --- </span></span><b name="data/step-1/plumed.7.datg" onclick='showPath("data/step-1/plumed.7.dat","data/step-1/plumed.7.datg","data/step-1/plumed.7.datg","black")'>g</b><span style="display:none;" id="data/step-1/plumed.7.datg">The GYRATION action with label <b>g</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">g</td><td width="5%"><font color="black">scalar</font></td><td>the radius of gyration</td></tr></table></span>: <div class="tooltip" style="color:green">GYRATION<div class="right">Calculate the radius of gyration, or other properties related to it. <a href="https://www.plumed.org/doc-master/user-doc/html/_g_y_r_a_t_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">TYPE<div class="right"> The type of calculation relative to the Gyration Tensor you want to perform<i></i></div></div>=RADIUS <div class="tooltip">ATOMS<div class="right">the group of atoms that you are calculating the Gyration Tensor for<i></i></div></div>=9,23,35,50,62,78,89,101,120,135,159,183,202,212,229,253,272,282,297,321,345,362,377,389,400,410
<b name="data/step-1/plumed.7.datene" onclick='showPath("data/step-1/plumed.7.dat","data/step-1/plumed.7.datene","data/step-1/plumed.7.datene","black")'>ene</b><span style="display:none;" id="data/step-1/plumed.7.datene">The ENERGY action with label <b>ene</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ene</td><td width="5%"><font color="black">scalar</font></td><td>the value calculated by this action</td></tr></table></span>: <div class="tooltip" style="color:green">ENERGY<div class="right">Calculate the total potential energy of the simulation box. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_n_e_r_g_y.html" style="color:green">More details</a><i></i></div></div>
<br/><b name="data/step-1/plumed.7.datwte" onclick='showPath("data/step-1/plumed.7.dat","data/step-1/plumed.7.datwte","data/step-1/plumed.7.datwte","black")'>wte</b><span style="display:none;" id="data/step-1/plumed.7.datwte">The METAD action with label <b>wte</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">wte.bias</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the bias potential</td></tr></table></span>: <div class="tooltip" style="color:green">METAD<div class="right">Used to performed metadynamics on one or more collective variables. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_e_t_a_d.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/step-1/plumed.7.datene">ene</b> <div class="tooltip">PACE<div class="right">the frequency for hill addition<i></i></div></div>=250 <div class="tooltip">HEIGHT<div class="right">the heights of the Gaussian hills<i></i></div></div>=2.5 <div class="tooltip">SIGMA<div class="right">the widths of the Gaussian hills<i></i></div></div>=500.0 <div class="tooltip">FILE<div class="right"> a file in which the list of added hills is stored<i></i></div></div>=HILLS_PTWTE <div class="tooltip">BIASFACTOR<div class="right">use well tempered metadynamics and use this bias factor<i></i></div></div>=50.0 <div class="tooltip">TEMP<div class="right">the system temperature - this is only needed if you are doing well-tempered metadynamics<i></i></div></div>=400
<br/><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/step-1/plumed.7.data">a</b>,<b name="data/step-1/plumed.7.datg">g</b>,<b name="data/step-1/plumed.7.datene">ene</b>,<b name="data/step-1/plumed.7.datwte">wte.bias</b> <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=50 <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=COLVAR_WTE
<br/><div class="tooltip" style="color:green">ENDPLUMED<div class="right">Terminate plumed input. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html" style="color:green">More details</a><i></i></div></div><span style="color:blue" class="comment">
</span></pre>
{% endraw %}