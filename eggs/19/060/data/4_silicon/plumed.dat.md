**Project ID:** [plumID:19.060]({{ '/' | absolute_url }}eggs/19/060/)  
**Source:** 4_silicon/plumed.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/4_silicon/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-failed-red.svg" alt="tested onv2.10" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-failed-red.svg" alt="tested onmaster" /></a></td></tr><tr><td style="padding:1px"><img src="https://img.shields.io/badge/with-LOAD-yellow.svg" alt="tested on master" /></td></tr>
</table></div></div>
<pre style="width=97%;">
<span class="plumedtooltip" style="color:blue"># vim:ft=plumed<span class="right">Enables syntax highlighting for PLUMED files in vim. See <a href="https://www.plumed.org/doc-master/user-doc/html/_vim_syntax.html">here for more details. </a><i></i></span></span>
<br/><span class="plumedtooltip" style="color:green">LOAD<span class="right">Loads a library, possibly defining new actions. <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">FILE<span class="right">file to be loaded<i></i></span></span>=../0_code/NeuralNetworkVes.cpp

<span style="display:none;" id="data/4_silicon/plumed.dat">The LOAD action with label <b></b> calculates something</span><span class="plumedtooltip" style="color:green">ENVIRONMENTSIMILARITY<span class="right">Measure how similar the environment around atoms is to that found in some reference crystal structure. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_n_v_i_r_o_n_m_e_n_t_s_i_m_i_l_a_r_i_t_y.html" style="color:green">More details</a><i></i></span></span> ...
 <span class="plumedtooltip">SPECIES<span class="right">this keyword is used for colvars such as coordination number<i></i></span></span>=1-216
 <span class="plumedtooltip">SIGMA<span class="right"> the width to use for the gaussian kernels<i></i></span></span>=0.04
 <span class="plumedtooltip">LATTICE_CONSTANTS<span class="right">Lattice constants<i></i></span></span>=0.5431
 <span class="plumedtooltip">CRYSTAL_STRUCTURE<span class="right"> Targeted crystal structure<i></i></span></span>=DIAMOND
 <span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/4_silicon/plumed.datrefcv" onclick='showPath("data/4_silicon/plumed.dat","data/4_silicon/plumed.datrefcv","data/4_silicon/plumed.datrefcv","brown")'>refcv</b>
 <span class="plumedtooltip">MORE_THAN<span class="right">calculate the number of variables that are more than a certain target value<i></i></span></span>={RATIONAL R_0=0.5 NN=12 MM=24}
 <span class="plumedtooltip">MEAN<span class="right"> calculate the mean of all the quantities<i></i></span></span>
... ENVIRONMENTSIMILARITY
<br/><span style="display:none;" id="data/4_silicon/plumed.datrefcv">The ENVIRONMENTSIMILARITY action with label <b>refcv</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">refcv.value</td><td>the environmental similar parameter for each of the input atoms</td></tr><tr><td width="5%">refcv.morethan</td><td>the number of colvars that have a value more than a threshold</td></tr><tr><td width="5%">refcv.mean</td><td>the mean of the colvars</td></tr></table></span><b name="data/4_silicon/plumed.datene" onclick='showPath("data/4_silicon/plumed.dat","data/4_silicon/plumed.datene","data/4_silicon/plumed.datene","brown")'>ene</b>: <span class="plumedtooltip" style="color:green">ENERGY<span class="right">Calculate the total potential energy of the simulation box. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_n_e_r_g_y.html" style="color:green">More details</a><i></i></span></span>
<br/><span style="display:none;" id="data/4_silicon/plumed.datene">The ENERGY action with label <b>ene</b> calculates something</span><b name="data/4_silicon/plumed.datq6" onclick='showPath("data/4_silicon/plumed.dat","data/4_silicon/plumed.datq6","data/4_silicon/plumed.datq6","brown")'>q6</b>: <span class="plumedtooltip" style="color:green">Q6<span class="right">Calculate sixth order Steinhardt parameters. <a href="https://www.plumed.org/doc-master/user-doc/html/_q6.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">SPECIES<span class="right">this keyword is used for colvars such as coordination number<i></i></span></span>=1-216 <span class="plumedtooltip">SWITCH<span class="right">the switching function that it used in the construction of the contact matrix<i></i></span></span>={CUBIC D_0=0.235 D_MAX=0.3} <span class="plumedtooltip">LOWMEM<span class="right"> this flag does nothing and is present only to ensure back-compatibility<i></i></span></span> <span class="plumedtooltip">VMEAN<span class="right"> calculate the norm of the mean vector<i></i></span></span>
<br/><span style="color:blue" class="comment"># nn bias</span>
<span style="display:none;" id="data/4_silicon/plumed.datq6">The Q6 action with label <b>q6</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">q6._vmean</td><td>the norm of the mean vector</td></tr><tr><td width="5%">q6.value</td><td>the norms of the vectors of spherical harmonic coefficients</td></tr></table></span><span class="plumedtooltip" style="color:green">NN_VES<span class="right">This action is not part of PLUMED and was included by using a LOAD command <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></span></span> ...
LABEL=<b name="data/4_silicon/plumed.datnn" onclick='showPath("data/4_silicon/plumed.dat","data/4_silicon/plumed.datnn","data/4_silicon/plumed.datnn","brown")'>nn</b>
ARG=<b name="data/4_silicon/plumed.datrefcv">refcv.morethan</b>
NODES=48,24,12
OPTIM=ADAM
ACTIVATION=RELU
GRID_MIN=0.
GRID_MAX=216.
GRID_BIN=500
TEMP=1700.
AVE_STRIDE=500
PRINT_STRIDE=1000
TARGET_STRIDE=1
GAMMA=70
LRATE=0.001
TAU_KL=5000
DECAY=2000
ADAPTIVE_DECAY=0.5
... NN_VES

<br/><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=500  <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=* <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=COLVAR


<span class="plumedtooltip" style="color:green">ENDPLUMED<span class="right">Terminate plumed input. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html" style="color:green">More details</a><i></i></span></span><span style="color:blue" class="comment">

METAD ...
 ARG=refcv.morethan
 BIASFACTOR=50
 GRID_MIN=-5
 GRID_MAX=220.0
 GRID_BIN=1000
 ADAPTIVE=DIFF
 SIGMA=250
 SIGMA_MIN=0.5
 SIGMA_MAX=20.
 TEMP=1600.
 PACE=500
 LABEL=metad
 HEIGHT=60.
 CALC_RCT
... METAD
# to avoid other structures
Q6 SPECIES=1-216 SWITCH={CUBIC D_0=0.235 D_MAX=0.3} VMEAN LABEL=q6
#diff: MATHEVAL ARG=q6.vmean,refcv.mean FUNC=(x-0.035)/(0.42-0.035)-(y-0.34)/(0.85-0.34) PERIODIC=NO
#UPPER_WALLS ARG=diff AT=0.15 KAPPA=50000 EXP=2 LABEL=uwall
</span></pre>
{% endraw %}
