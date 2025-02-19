**Project ID:** [plumID:25.006]({{ '/' | absolute_url }}eggs/25/006/)  
**Source:** PROTACs_PBMetaD_PLUMED-NEST/Input_Files/plumed_lastbias.dat  
**Originally used with PLUMED version:** 2.8.2  
**Stable:** [zipped raw stdout](plumed_lastbias.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_lastbias.dat.plumed.stderr.txt.zip) - [stderr](plumed_lastbias.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed_lastbias.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_lastbias.dat.plumed_master.stderr.txt.zip) - [stderr](plumed_lastbias.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/PROTACs_PBMetaD_PLUMED-NEST/Input_Files/plumed_lastbias.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed_lastbias.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-failed-red.svg" alt="tested onv2.10" /></a></td></tr><tr><td style="padding:1px"><a href="plumed_lastbias.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-failed-red.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue" class="comment">##Reweighting</span>
<br/><span class="plumedtooltip" style="color:green">RESTART<span class="right">Activate restart. <a href="https://www.plumed.org/doc-master/user-doc/html/_r_e_s_t_a_r_t.html" style="color:green">More details</a><i></i></span></span>
<br/><span style="display:none;" id="data/PROTACs_PBMetaD_PLUMED-NEST/Input_Files/plumed_lastbias.dat">The RESTART action with label <b></b> calculates something</span><span class="plumedtooltip" style="color:green">INCLUDE<span class="right">Includes an external input file, similar to #include in C preprocessor. <a href="https://www.plumed.org/doc-master/user-doc/html/_i_n_c_l_u_d_e.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">FILE<span class="right">file to be included<i></i></span></span>=plumed_read.dat

<span class="plumedtooltip" style="color:green">PBMETAD<span class="right">Used to performed Parallel Bias metadynamics. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_b_m_e_t_a_d.html" style="color:green">More details</a><i></i></span></span> ...
 <span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/PROTACs_PBMetaD_PLUMED-NEST/Input_Files/plumed_lastbias.datpbmetad" onclick='showPath("data/PROTACs_PBMetaD_PLUMED-NEST/Input_Files/plumed_lastbias.dat","data/PROTACs_PBMetaD_PLUMED-NEST/Input_Files/plumed_lastbias.datpbmetad","data/PROTACs_PBMetaD_PLUMED-NEST/Input_Files/plumed_lastbias.datpbmetad","brown")'>pbmetad</b>
 <span class="plumedtooltip">ARG<span class="right">the labels of the scalars on which the bias will act<i></i></span></span>=t_brd4_4,t_brd4_5,t_brd4_6,t_brd4_7,t_linker_1,t_linker_2,t_linker_3,t_linker_4,t_linker_5,t_linker_6,t_linker_7,t_linker_8,t_linker_9,t_vhl_1,t_vhl_2,t_vhl_3,t_vhl_4,t_vhl_5,t_vhl_6,t_vhl_7,t_vhl_8,t_vhl_9,t_vhl_10,t_vhl_11,t_vhl_12,t_vhl_13
 <span class="plumedtooltip">PACE<span class="right">the frequency for hill addition, one for all biases<i></i></span></span>=500000000
 <span class="plumedtooltip">BIASFACTOR<span class="right">use well tempered metadynamics with this bias factor, one for all biases<i></i></span></span>=24
 <span class="plumedtooltip">HEIGHT<span class="right">the height of the Gaussian hills, one for all biases<i></i></span></span>=0 
 <span class="plumedtooltip">SIGMA<span class="right">the widths of the Gaussian hills<i></i></span></span>=0.2,0.2,0.2,0.2,0.2,0.2,0.2,0.2,0.2,0.2,0.2,0.2,0.2,0.2,0.2,0.2,0.2,0.2,0.2,0.2,0.2,0.2,0.2,0.2,0.2,0.2
 <span class="plumedtooltip">GRID_MIN<span class="right">the lower bounds for the grid<i></i></span></span>=-pi,-pi,-pi,-pi,-pi,-pi,-pi,-pi,-pi,-pi,-pi,-pi,-pi,-pi,-pi,-pi,-pi,-pi,-pi,-pi,-pi,-pi,-pi,-pi,-pi,-pi
 <span class="plumedtooltip">GRID_MAX<span class="right">the upper bounds for the grid<i></i></span></span>=pi,pi,pi,pi,pi,pi,pi,pi,pi,pi,pi,pi,pi,pi,pi,pi,pi,pi,pi,pi,pi,pi,pi,pi,pi,pi
 <span class="plumedtooltip">TEMP<span class="right">the system temperature - this is only needed if you are doing well-tempered metadynamics<i></i></span></span>=300
... PBMETAD

<br/><span style="display:none;" id="data/PROTACs_PBMetaD_PLUMED-NEST/Input_Files/plumed_lastbias.datpbmetad">The PBMETAD action with label <b>pbmetad</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">pbmetad.bias</td><td>the instantaneous value of the bias potential</td></tr></table></span><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></span></span> ...
 <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=rgyr,cmap,energy,volume,<b name="data/PROTACs_PBMetaD_PLUMED-NEST/Input_Files/plumed_lastbias.datpbmetad">pbmetad.*</b>
 <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=colvar_main.lastbias_8-microsec.data
 <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=500
...
<br/><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></span></span> ...
 <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=d_tbut_ph_brd4,d_tbut_S_5ring_brd4,d_tbut_N_ring_brd4,d_tbut_N_5ring_brd4,d_ph_brd4_linker,d_ph_vhl_linker,d_ph_brd4_ph_vhl,d_ph_vhl_S_5ring_brd4,d_ph_vhl_N_ring_brd4,d_ph_vhl_N_5ring_brd4,d_s_vhl_ph_brd4,d_s_S_5ring_brd4,d_s_N_ring_brd4,d_s_N_5ring_brd4,d_n_vhl_ph_brd4,d_n_vhl_S_5ring_brd4,d_n_vhl_N_ring_brd4,d_n_vhl_N_5ring_brd4,<b name="data/PROTACs_PBMetaD_PLUMED-NEST/Input_Files/plumed_lastbias.datpbmetad">pbmetad.*</b>
 <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=colvar_distances.lastbias_8-microsec.data 
 <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=500
...
<br/><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></span></span> ...
 <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=t_brd4_1,t_brd4_2,t_brd4_3,t_brd4_4,t_brd4_5,t_brd4_6,t_brd4_7,t_linker_1,t_linker_2,t_linker_3,t_linker_4,t_linker_5,t_linker_6,t_linker_7,t_linker_8,t_linker_9,t_vhl_1,t_vhl_2,t_vhl_3,t_vhl_4,t_vhl_5,t_vhl_6,t_vhl_7,t_vhl_8,t_vhl_9,t_vhl_10,t_vhl_11,t_vhl_12,t_vhl_13,<b name="data/PROTACs_PBMetaD_PLUMED-NEST/Input_Files/plumed_lastbias.datpbmetad">pbmetad.*</b>
 <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=colvar_angles.lastbias_8-microsec.data 
 <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=500
... 
</pre>
{% endraw %}
