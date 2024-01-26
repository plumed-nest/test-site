**Project ID:** [plumID:19.060]({{ '/' | absolute_url }}eggs/19/060/)  
**Source:** 3_ala4/simulation/plumed.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/3_ala4/simulation/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-failed-red.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-failed-red.svg" alt="tested onmaster" /></a></td></tr><tr><td style="padding:1px"><img src="https://img.shields.io/badge/with-LOAD-yellow.svg" alt="tested on master" /></td></tr>
</table></div></div>
<pre style="width=97%;">
<div class="tooltip" style="color:blue"># vim:ft=plumed<div class="right">Enables syntax highlighting for PLUMED files in vim. See <a href="https://www.plumed.org/doc-master/user-doc/html/_vim_syntax.html">here for more details. </a><i></i></div></div>
<br/><div class="tooltip" style="color:green">LOAD<div class="right">Loads a library, possibly defining new actions. <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">FILE<div class="right">file to be loaded<i></i></div></div>=../../0_code/NeuralNetworkVes.cpp
<br/><b name="data/3_ala4/simulation/plumed.datphi1" onclick='showPath("data/3_ala4/simulation/plumed.dat","data/3_ala4/simulation/plumed.datphi1")'>phi1</b>: <div class="tooltip" style="color:green">TORSION<div class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the four atoms involved in the torsional angle<i></i></div></div>=5,7,9,15
<span style="display:none;" id="data/3_ala4/simulation/plumed.datphi1">The TORSION action with label <b>phi1</b> calculates a scalar quantity</span><b name="data/3_ala4/simulation/plumed.datphi2" onclick='showPath("data/3_ala4/simulation/plumed.dat","data/3_ala4/simulation/plumed.datphi2")'>phi2</b>: <div class="tooltip" style="color:green">TORSION<div class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the four atoms involved in the torsional angle<i></i></div></div>=15,17,19,25
<span style="display:none;" id="data/3_ala4/simulation/plumed.datphi2">The TORSION action with label <b>phi2</b> calculates a scalar quantity</span><b name="data/3_ala4/simulation/plumed.datphi3" onclick='showPath("data/3_ala4/simulation/plumed.dat","data/3_ala4/simulation/plumed.datphi3")'>phi3</b>: <div class="tooltip" style="color:green">TORSION<div class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the four atoms involved in the torsional angle<i></i></div></div>=25,27,29,35
<span style="display:none;" id="data/3_ala4/simulation/plumed.datphi3">The TORSION action with label <b>phi3</b> calculates a scalar quantity</span><b name="data/3_ala4/simulation/plumed.datpsi1" onclick='showPath("data/3_ala4/simulation/plumed.dat","data/3_ala4/simulation/plumed.datpsi1")'>psi1</b>: <div class="tooltip" style="color:green">TORSION<div class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the four atoms involved in the torsional angle<i></i></div></div>=7,9,15,17
<span style="display:none;" id="data/3_ala4/simulation/plumed.datpsi1">The TORSION action with label <b>psi1</b> calculates a scalar quantity</span><b name="data/3_ala4/simulation/plumed.datpsi2" onclick='showPath("data/3_ala4/simulation/plumed.dat","data/3_ala4/simulation/plumed.datpsi2")'>psi2</b>: <div class="tooltip" style="color:green">TORSION<div class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the four atoms involved in the torsional angle<i></i></div></div>=17,19,25,27
<span style="display:none;" id="data/3_ala4/simulation/plumed.datpsi2">The TORSION action with label <b>psi2</b> calculates a scalar quantity</span><b name="data/3_ala4/simulation/plumed.datpsi3" onclick='showPath("data/3_ala4/simulation/plumed.dat","data/3_ala4/simulation/plumed.datpsi3")'>psi3</b>: <div class="tooltip" style="color:green">TORSION<div class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the four atoms involved in the torsional angle<i></i></div></div>=27,29,35,37
<br/><span style="color:blue"># the following is a fake example using the grid-based version</span>
<span style="color:blue"># see below ENDPLUMED for the MC-based version used in the paper</span>
<br/><span style="display:none;" id="data/3_ala4/simulation/plumed.datpsi3">The TORSION action with label <b>psi3</b> calculates a scalar quantity</span><div class="tooltip" style="color:green">NN_VES<div class="right">This action is not part of PLUMED and was included by using a LOAD command <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></div></div> ...
  TEMP=300.0
  LABEL=<b name="data/3_ala4/simulation/plumed.datbias" onclick='showPath("data/3_ala4/simulation/plumed.dat","data/3_ala4/simulation/plumed.datbias")'>bias</b>
  ARG=<b name="data/3_ala4/simulation/plumed.datphi1">phi1</b>,<b name="data/3_ala4/simulation/plumed.datphi2">phi2</b>,<b name="data/3_ala4/simulation/plumed.datphi3">phi3</b>,<b name="data/3_ala4/simulation/plumed.datpsi1">psi1</b>,<b name="data/3_ala4/simulation/plumed.datpsi2">psi2</b>,<b name="data/3_ala4/simulation/plumed.datpsi3">psi3</b>
  NODES=96,48,24
  OPTIM=ADAM
  ACTIVATION=RELU
  GRID_MIN=-pi,-pi,-pi,-pi,-pi,-pi
  GRID_MAX=pi,pi,pi,pi,pi,pi
  GRID_BIN=10,10,10,10,10,10 <span style="color:blue"># set to 10 to avoid std_bad_alloc</span>
  AVE_STRIDE=500
  PRINT_STRIDE=100
  TARGET_STRIDE=1
  LRATE=0.001
  GAMMA=10
  TAU_KL=100000
  DECAY=2000
  ADAPTIVE_DECAY=20
... NN_VES

<br/><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div> <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=100 <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=COLVAR
<br/><div class="tooltip" style="color:green">ENDPLUMED<div class="right">Terminate plumed input. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html" style="color:green">More details</a><i></i></div></div><span style="color:blue">

# The following input is related to the MC-based version used in the paper. 
This is not compatible with newer plumed versions, if you want to try it you should use the code NeuralNetworkVes_ORIGINAL.cpp. 

NN_VES ...
  TEMP=300.0
  LABEL=bias
  ARG=phi1,phi2,phi3,psi1,psi2,psi3
  NODES=96,48,24
  OPTIM=ADAM
  ACTIVATION=RELU
  GRID_MIN=-pi,-pi,-pi,-pi,-pi,-pi
  GRID_MAX=pi,pi,pi,pi,pi,pi
  GRID_BIN=300,300,300,300,300,300
  AVE_STRIDE=500
  PRINT_STRIDE=100
  TARGET_STRIDE=1
  LRATE=0.001
  GAMMA=10
  TAU_KL=100000
  MODE_DECAY=4
  DECAY_STEP_START=10000
  DECAY=2000
  ADAPTIVE_DECAY=20
  MC_POINTS=20000
  MC_SIGMA=0.5,0.5,0.5,0.5,0.5,0.5
  CALC_MC_ERR=0
  MC_CONVERGENCE_TEST=0
  L2_weight=0.2
  SERIAL
  CALC_RCT
... NN_VES
</span></pre>
{% endraw %}
