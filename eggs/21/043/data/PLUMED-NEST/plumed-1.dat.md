**Project ID:** [plumID:21.043]({{ '/' | absolute_url }}eggs/21/043/)  
**Source:** PLUMED-NEST/plumed-1.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [zipped raw stdout](plumed-1.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed-1.dat.plumed.stderr.txt.zip) - [stderr](plumed-1.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed-1.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed-1.dat.plumed_master.stderr.txt.zip) - [stderr](plumed-1.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/PLUMED-NEST/plumed-1.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed-1.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed-1.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue">#RESTART</span>
<br/><div class="tooltip" style="color:green">FIT_TO_TEMPLATE<div class="right">This action is used to align a molecule to a template. <a href="https://www.plumed.org/doc-master/user-doc/html/_f_i_t__t_o__t_e_m_p_l_a_t_e.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">REFERENCE<div class="right">a file in pdb format containing the reference structure and the atoms involved in the CV<i></i></div></div>=step5_charmm2gmx-modified.pdb
<b name="data/PLUMED-NEST/plumed-1.data0" onclick='showPath("data/PLUMED-NEST/plumed-1.dat","data/PLUMED-NEST/plumed-1.data0")'>a0</b>: <div class="tooltip" style="color:green">FIXEDATOM<div class="right">Add a virtual atom in a fixed position. <a href="https://www.plumed.org/doc-master/user-doc/html/_f_i_x_e_d_a_t_o_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">AT<div class="right">coordinates of the virtual atom<i></i></div></div>=0,0,0
<b name="data/PLUMED-NEST/plumed-1.dataz" onclick='showPath("data/PLUMED-NEST/plumed-1.dat","data/PLUMED-NEST/plumed-1.dataz")'>az</b>: <div class="tooltip" style="color:green">FIXEDATOM<div class="right">Add a virtual atom in a fixed position. <a href="https://www.plumed.org/doc-master/user-doc/html/_f_i_x_e_d_a_t_o_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">AT<div class="right">coordinates of the virtual atom<i></i></div></div>=0,0,1
<b name="data/PLUMED-NEST/plumed-1.datphi" onclick='showPath("data/PLUMED-NEST/plumed-1.dat","data/PLUMED-NEST/plumed-1.datphi")'>phi</b>: <div class="tooltip" style="color:green">TORSION<div class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the four atoms involved in the torsional angle<i></i></div></div>=70,143,<b name="data/PLUMED-NEST/plumed-1.data0">a0</b>,<b name="data/PLUMED-NEST/plumed-1.dataz">az</b>
<span style="display:none;" id="data/PLUMED-NEST/plumed-1.datphi">The TORSION action with label <b>phi</b> calculates a scalar quantity</span><b name="data/PLUMED-NEST/plumed-1.dattheta" onclick='showPath("data/PLUMED-NEST/plumed-1.dat","data/PLUMED-NEST/plumed-1.dattheta")'>theta</b>: <div class="tooltip" style="color:green">TORSION<div class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the four atoms involved in the torsional angle<i></i></div></div>=2549,2420,<b name="data/PLUMED-NEST/plumed-1.data0">a0</b>,<b name="data/PLUMED-NEST/plumed-1.dataz">az</b>
<br/><span style="color:blue">##ZANGLES ATOMS=70,143 LABEL=phi</span>
<span style="color:blue">##ZANGLES ATOMS=2549,2420 LABEL=theta</span>
<span style="color:blue"># Activate metadynamics in phi and psi</span>
<span style="color:blue"># depositing a Gaussian every 500 time steps,</span>
<span style="color:blue"># with height equal to 1.0 kJoule/mol,</span>
<span style="color:blue"># and width 0.35 rad for both CVs. </span>
<br/><span style="display:none;" id="data/PLUMED-NEST/plumed-1.dattheta">The TORSION action with label <b>theta</b> calculates a scalar quantity</span><div class="tooltip" style="color:green">METAD<div class="right">Used to performed metadynamics on one or more collective variables. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_e_t_a_d.html" style="color:green">More details</a><i></i></div></div> ...
<div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/PLUMED-NEST/plumed-1.datmetad" onclick='showPath("data/PLUMED-NEST/plumed-1.dat","data/PLUMED-NEST/plumed-1.datmetad")'>metad</b>
<div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/PLUMED-NEST/plumed-1.datphi">phi</b>,<b name="data/PLUMED-NEST/plumed-1.dattheta">theta</b>
<div class="tooltip">PACE<div class="right">the frequency for hill addition<i></i></div></div>=500
<div class="tooltip">HEIGHT<div class="right">the heights of the Gaussian hills<i></i></div></div>=1.0
<div class="tooltip">SIGMA<div class="right">the widths of the Gaussian hills<i></i></div></div>=0.35,0.35
<div class="tooltip">FILE<div class="right"> a file in which the list of added hills is stored<i></i></div></div>=HILLS
<div class="tooltip">BIASFACTOR<div class="right">use well tempered metadynamics and use this bias factor<i></i></div></div>=10.0
<div class="tooltip">TEMP<div class="right">the system temperature - this is only needed if you are doing well-tempered metadynamics<i></i></div></div>=310.0
<div class="tooltip">GRID_MIN<div class="right">the lower bounds for the grid<i></i></div></div>=-pi,-pi
<div class="tooltip">GRID_MAX<div class="right">the upper bounds for the grid<i></i></div></div>=pi,pi
<div class="tooltip">GRID_SPACING<div class="right">the approximate grid spacing (to be used as an alternative or together with GRID_BIN)<i></i></div></div>=0.1,0.1
... METAD
<br/><span style="display:none;" id="data/PLUMED-NEST/plumed-1.datmetad">The METAD action with label <b>metad</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">metad.bias</td><td>the instantaneous value of the bias potential</td></tr></table></span><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=500 <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/PLUMED-NEST/plumed-1.datphi">phi</b>,<b name="data/PLUMED-NEST/plumed-1.dattheta">theta</b>,<b name="data/PLUMED-NEST/plumed-1.datmetad">metad.bias</b> <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=COLVAR
</pre>
{% endraw %}
