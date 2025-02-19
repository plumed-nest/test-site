**Project ID:** [plumID:19.060]({{ '/' | absolute_url }}eggs/19/060/)  
**Source:** 2_ala2/simulation/plumed.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/2_ala2/simulation/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-failed-red.svg" alt="tested onv2.10" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-failed-red.svg" alt="tested onmaster" /></a></td></tr><tr><td style="padding:1px"><img src="https://img.shields.io/badge/with-LOAD-yellow.svg" alt="tested on master" /></td></tr>
</table></div></div>
<pre style="width=97%;">
<span style="color:blue" class="comment"># Load file</span>
<span class="plumedtooltip" style="color:green">LOAD<span class="right">Loads a library, possibly defining new actions. <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">FILE<span class="right">file to be loaded<i></i></span></span>=../../0_code/NeuralNetworkVes.cpp

<span style="color:blue" class="comment"># set up two variables for Phi and Psi dihedral angles </span>
<span style="display:none;" id="data/2_ala2/simulation/plumed.dat">The LOAD action with label <b></b> calculates something</span><b name="data/2_ala2/simulation/plumed.datphi" onclick='showPath("data/2_ala2/simulation/plumed.dat","data/2_ala2/simulation/plumed.datphi","data/2_ala2/simulation/plumed.datphi","brown")'>phi</b>: <span class="plumedtooltip" style="color:green">TORSION<span class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=5,7,9,15
<span style="display:none;" id="data/2_ala2/simulation/plumed.datphi">The TORSION action with label <b>phi</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">phi.value</td><td>the TORSION involving these atoms</td></tr></table></span><b name="data/2_ala2/simulation/plumed.datpsi" onclick='showPath("data/2_ala2/simulation/plumed.dat","data/2_ala2/simulation/plumed.datpsi","data/2_ala2/simulation/plumed.datpsi","brown")'>psi</b>: <span class="plumedtooltip" style="color:green">TORSION<span class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=7,9,15,17

<span style="color:blue" class="comment"># nn bias</span>
<span style="display:none;" id="data/2_ala2/simulation/plumed.datpsi">The TORSION action with label <b>psi</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">psi.value</td><td>the TORSION involving these atoms</td></tr></table></span><span class="plumedtooltip" style="color:green">NN_VES<span class="right">This action is not part of PLUMED and was included by using a LOAD command <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></span></span> ...
LABEL=<b name="data/2_ala2/simulation/plumed.datnn" onclick='showPath("data/2_ala2/simulation/plumed.dat","data/2_ala2/simulation/plumed.datnn","data/2_ala2/simulation/plumed.datnn","brown")'>nn</b>
ARG=<b name="data/2_ala2/simulation/plumed.datphi">phi</b> 
NODES=48,24,12 
OPTIM=ADAM
ACTIVATION=RELU
GRID_MIN=-pi 
GRID_MAX=pi 
GRID_BIN=50 
TEMP=300.
AVE_STRIDE=500
PRINT_STRIDE=1000 
TARGET_STRIDE=1 
GAMMA=10
LRATE=0.001 
TAU_KL=10000
DECAY=1000
ADAPTIVE_DECAY=0.5
... NN_VES
<br/><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=500 <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=* <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=COLVAR <span class="plumedtooltip">FMT<span class="right">the format that should be used to output real numbers<i></i></span></span>=%10.8f
</pre>
{% endraw %}
