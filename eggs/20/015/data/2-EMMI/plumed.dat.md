**Project ID:** [plumID:20.015]({{ '/' | absolute_url }}eggs/20/015/)  
**Source:** 2-EMMI/plumed.dat  
**Originally used with PLUMED version:** 2.6-dev  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/2-EMMI/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-failed-red.svg" alt="tested onv2.10" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-failed-red.svg" alt="tested onmaster" /></a></td></tr><tr><td style="padding:1px"><img src="https://img.shields.io/badge/with-LOAD-yellow.svg" alt="tested on master" /></td></tr>
</table></div></div>
<pre style="width=97%;">
<span style="color:blue" class="comment"># uncomment next line if your restart</span>
<span style="color:blue" class="comment">#RESTART</span>
<br/><span style="color:blue" class="comment"># load extra file</span>
<span style="color:blue" class="comment"># set to correct location</span>
<span class="plumedtooltip" style="color:green">LOAD<span class="right">Loads a library, possibly defining new actions. <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">FILE<span class="right">file to be loaded<i></i></span></span>=EMMIVox.cpp

<span style="color:blue" class="comment"># include topology info - set path a PDB file</span>
<span style="display:none;" id="data/2-EMMI/plumed.dat">The LOAD action with label <b></b> calculates something</span><span class="plumedtooltip" style="color:green">MOLINFO<span class="right">This command is used to provide information on the molecules that are present in your system. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">STRUCTURE<span class="right">a file in pdb format containing a reference structure<i></i></span></span>=<b name="data/2-EMMI/plumed.dat">../0-TOPO/step5_charmm2gmx.pdb</b> <span class="plumedtooltip">WHOLE<span class="right"> The reference structure is whole, i<i></i></span></span>
<br/><span style="color:blue" class="comment"># define all heavy atoms - set path to index file</span>
<b name="data/2-EMMI/plumed.datprotein-h" onclick='showPath("data/2-EMMI/plumed.dat","data/2-EMMI/plumed.datprotein-h","data/2-EMMI/plumed.datprotein-h","brown")'>protein-h</b>: <span class="plumedtooltip" style="color:green">GROUP<span class="right">Define a group of atoms so that a particular list of atoms can be referenced with a single label in definitions of CVs or virtual atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_g_r_o_u_p.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">NDX_FILE<span class="right">the name of index file (gromacs syntax)<i></i></span></span>=<b name="data/2-EMMI/plumed.dat">../0-TOPO/index.ndx</b> <span class="plumedtooltip">NDX_GROUP<span class="right">the name of the group to be imported (gromacs syntax) - first group found is used by default<i></i></span></span>=PROT-H

<span style="color:blue" class="comment"># make protein whole and in the cell where map is defined</span>
<span style="display:none;" id="data/2-EMMI/plumed.datprotein-h">The GROUP action with label <b>protein-h</b> calculates something</span><span class="plumedtooltip" style="color:green">WHOLEMOLECULES<span class="right">This action is used to rebuild molecules that can become split by the periodic boundary conditions. <a href="https://www.plumed.org/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html" style="color:green">More details</a><i></i></span></span> ...
<span class="plumedtooltip">ADDREFERENCE<span class="right"> Define the reference position of the first atom of each entity using a PDB file<i></i></span></span>
<span class="plumedtooltip">EMST<span class="right"> only for backward compatibility, as of PLUMED 2<i></i></span></span>
<span class="plumedtooltip">ENTITY0<span class="right">the atoms that make up a molecule that you wish to align<i></i></span></span>=1-6701
<span class="plumedtooltip">ENTITY1<span class="right">the atoms that make up a molecule that you wish to align<i></i></span></span>=6702-6741
... WHOLEMOLECULES
<br/><span style="color:blue" class="comment"># create EMMI score</span>
<span class="plumedtooltip" style="color:green">EMMIVOX<span class="right">Bayesian single-structure and ensemble refinement with cryo-EM maps. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_m_m_i_v_o_x.html" style="color:green">More details</a><i></i></span></span> ...
<span style="color:blue" class="comment"># name of this action</span>
<span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/2-EMMI/plumed.datgmm" onclick='showPath("data/2-EMMI/plumed.dat","data/2-EMMI/plumed.datgmm","data/2-EMMI/plumed.datgmm","brown")'>gmm</b>
<span style="color:blue" class="comment"># general parameters - do not change this! </span>
<span class="plumedtooltip">TEMP<span class="right">temperature<i></i></span></span>=303.15 <span class="plumedtooltip">NL_STRIDE<span class="right">neighbor list update frequency<i></i></span></span>=50 NL_CUTOFF=0.5 NS_CUTOFF=1.0
<span style="color:blue" class="comment"># define atoms for cryo-EM restraint and read experimental data</span>
<span style="color:blue" class="comment"># set path to map file if not in current directory</span>
<span class="plumedtooltip">ATOMS<span class="right">atoms used in the calculation of the density map, typically all heavy atoms<i></i></span></span>=<b name="data/2-EMMI/plumed.datprotein-h">protein-h</b> <span class="plumedtooltip">DATA_FILE<span class="right">file with cryo-EM map<i></i></span></span>=map_zoned_align.dat
<span style="color:blue" class="comment"># info about the experimental map</span>
<span class="plumedtooltip">NORM_DENSITY<span class="right">integral of experimental density<i></i></span></span>=2068.185 <span class="plumedtooltip">RESOLUTION<span class="right">cryo-EM map resolution<i></i></span></span>=0.1 VOXEL=0.1012
<span style="color:blue" class="comment"># data likelihood (or noise model): Marginal</span>
NOISETYPE=MARGINAL <span class="plumedtooltip">SIGMA_MIN<span class="right">minimum density error<i></i></span></span>=0.2
<span style="color:blue" class="comment"># write output</span>
<span class="plumedtooltip">STATUS_FILE<span class="right">write a file with all the data useful for restart<i></i></span></span>=EMMIStatus <span class="plumedtooltip">WRITE_STRIDE<span class="right">stride for writing status file<i></i></span></span>=2500
...
<br/><span style="color:blue" class="comment"># translate into bias - updated every 2 time steps</span>
<span style="display:none;" id="data/2-EMMI/plumed.datgmm">The EMMIVOX action with label <b>gmm</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">gmm.scoreb</td><td>Bayesian score</td></tr><tr><td width="5%">gmm.scale</td><td>scale factor</td></tr><tr><td width="5%">gmm.offset</td><td>offset</td></tr><tr><td width="5%">gmm.accB</td><td>Bfactor MC acceptance</td></tr><tr><td width="5%">gmm.kbt</td><td>temperature in energy unit</td></tr></table></span><b name="data/2-EMMI/plumed.datemr" onclick='showPath("data/2-EMMI/plumed.dat","data/2-EMMI/plumed.datemr","data/2-EMMI/plumed.datemr","brown")'>emr</b>: <span class="plumedtooltip" style="color:green">BIASVALUE<span class="right">Takes the value of one variable and use it as a bias <a href="https://www.plumed.org/doc-master/user-doc/html/_b_i_a_s_v_a_l_u_e.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the labels of the scalar/vector arguments whose values will be used as a bias on the system<i></i></span></span>=<b name="data/2-EMMI/plumed.datgmm">gmm.scoreb</b> <span class="plumedtooltip">STRIDE<span class="right">the frequency with which the forces due to the bias should be calculated<i></i></span></span>=2

<span style="color:blue" class="comment"># print output to file</span>
<span style="display:none;" id="data/2-EMMI/plumed.datemr">The BIASVALUE action with label <b>emr</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">emr.bias</td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">emr._bias</td><td>one or multiple instances of this quantity can be referenced elsewhere in the input file</td></tr></table></span><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=<b name="data/2-EMMI/plumed.datgmm">gmm.*</b> <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=COLVAR <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=2500
</pre>
{% endraw %}
