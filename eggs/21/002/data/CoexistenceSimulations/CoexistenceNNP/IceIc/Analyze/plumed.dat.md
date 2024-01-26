**Project ID:** [plumID:21.002]({{ '/' | absolute_url }}eggs/21/002/)  
**Source:** CoexistenceSimulations/CoexistenceNNP/IceIc/Analyze/plumed.dat  
**Originally used with PLUMED version:** 2.8  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/CoexistenceSimulations/CoexistenceNNP/IceIc/Analyze/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue">#SETTINGS NREPLICAS=2</span>
<div class="tooltip" style="color:blue"># vim:ft=plumed<div class="right">Enables syntax highlighting for PLUMED files in vim. See <a href="https://www.plumed.org/doc-master/user-doc/html/_vim_syntax.html">here for more details. </a><i></i></div></div>
<br/><div class="tooltip" style="color:green">ENVIRONMENTSIMILARITY<div class="right">Measure how similar the environment around atoms is to that found in some reference crystal structure. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_n_v_i_r_o_n_m_e_n_t_s_i_m_i_l_a_r_i_t_y.html" style="color:green">More details</a><i></i></div></div> ...
 <div class="tooltip">SPECIES<div class="right">this keyword is used for colvars such as coordination number<i></i></div></div>=1-1728:3
 <div class="tooltip">SIGMA<div class="right"> Broadening parameter<i></i></div></div>=0.05
 <div class="tooltip">CRYSTAL_STRUCTURE<div class="right"> Targeted crystal structure<i></i></div></div>=CUSTOM
 <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/CoexistenceSimulations/CoexistenceNNP/IceIc/Analyze/plumed.datrefcv" onclick='showPath("data/CoexistenceSimulations/CoexistenceNNP/IceIc/Analyze/plumed.dat","data/CoexistenceSimulations/CoexistenceNNP/IceIc/Analyze/plumed.datrefcv")'>refcv</b>
 <div class="tooltip">REFERENCE_1<div class="right">PDB files with relative distances from central atom<i></i></div></div>=env1c.pdb
 <div class="tooltip">REFERENCE_2<div class="right">PDB files with relative distances from central atom<i></i></div></div>=env2c.pdb
 <div class="tooltip">MORE_THAN<div class="right">calculate the number of variables more than a certain target value<i></i></div></div>={RATIONAL R_0=0.5 NN=8 MM=16}
 <div class="tooltip">MEAN<div class="right">take the mean of these variables<i></i></div></div>
... ENVIRONMENTSIMILARITY
<br/><span style="display:none;" id="data/CoexistenceSimulations/CoexistenceNNP/IceIc/Analyze/plumed.datrefcv">The ENVIRONMENTSIMILARITY action with label <b>refcv</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">refcv.mean</td><td>the mean value</td></tr><tr><td width="5%">refcv.morethan</td><td>the number of values more than a target value</td></tr></table></span><b name="data/CoexistenceSimulations/CoexistenceNNP/IceIc/Analyze/plumed.datenergy" onclick='showPath("data/CoexistenceSimulations/CoexistenceNNP/IceIc/Analyze/plumed.dat","data/CoexistenceSimulations/CoexistenceNNP/IceIc/Analyze/plumed.datenergy")'>energy</b>: <div class="tooltip" style="color:green">ENERGY<div class="right">Calculate the total potential energy of the simulation box. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_n_e_r_g_y.html" style="color:green">More details</a><i></i></div></div>
<b name="data/CoexistenceSimulations/CoexistenceNNP/IceIc/Analyze/plumed.datvol" onclick='showPath("data/CoexistenceSimulations/CoexistenceNNP/IceIc/Analyze/plumed.dat","data/CoexistenceSimulations/CoexistenceNNP/IceIc/Analyze/plumed.datvol")'>vol</b>: <div class="tooltip" style="color:green">VOLUME<div class="right">Calculate the volume of the simulation box. <a href="https://www.plumed.org/doc-master/user-doc/html/_v_o_l_u_m_e.html" style="color:green">More details</a><i></i></div></div>
<br/><span style="display:none;" id="data/CoexistenceSimulations/CoexistenceNNP/IceIc/Analyze/plumed.datvol">The VOLUME action with label <b>vol</b> calculates a scalar quantity</span><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=500  <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div> <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=COLVAR
</pre>
{% endraw %}
