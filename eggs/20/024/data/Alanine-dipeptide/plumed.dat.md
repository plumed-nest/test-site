**Project ID:** [plumID:20.024]({{ '/' | absolute_url }}eggs/20/024/)  
**Source:** Alanine-dipeptide/plumed.dat  
**Originally used with PLUMED version:** 2.7  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/Alanine-dipeptide/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-failed-red.svg" alt="tested onmaster" /></a></td></tr><tr><td style="padding:1px"><img src="https://img.shields.io/badge/with-LOAD-yellow.svg" alt="tested on master" /></td></tr>
</table></div></div>
<pre style="width=97%;">
<div class="tooltip" style="color:green">LOAD<div class="right">Loads a library, possibly defining new actions. <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">FILE<div class="right">file to be loaded<i></i></div></div>=../GAMBES.cpp

<br/><b name="data/Alanine-dipeptide/plumed.datphi" onclick='showPath("data/Alanine-dipeptide/plumed.dat","data/Alanine-dipeptide/plumed.datphi")'>phi</b>: <div class="tooltip" style="color:green">TORSION<div class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the four atoms involved in the torsional angle<i></i></div></div>=5,7,9,15
<span style="display:none;" id="data/Alanine-dipeptide/plumed.datphi">The TORSION action with label <b>phi</b> calculates a scalar quantity</span><b name="data/Alanine-dipeptide/plumed.datpsi" onclick='showPath("data/Alanine-dipeptide/plumed.dat","data/Alanine-dipeptide/plumed.datpsi")'>psi</b>: <div class="tooltip" style="color:green">TORSION<div class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the four atoms involved in the torsional angle<i></i></div></div>=7,9,15,17

<br/><span style="display:none;" id="data/Alanine-dipeptide/plumed.datpsi">The TORSION action with label <b>psi</b> calculates a scalar quantity</span><div class="tooltip" style="color:green">GAMBES<div class="right">This action is not part of PLUMED and was included by using a LOAD command <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></div></div> ...
  ARG=<b name="data/Alanine-dipeptide/plumed.datphi">phi</b>,<b name="data/Alanine-dipeptide/plumed.datpsi">psi</b>
  NSTATES=2
  FILENAME=state
  PACE=500
  LABEL=<b name="data/Alanine-dipeptide/plumed.datext" onclick='showPath("data/Alanine-dipeptide/plumed.dat","data/Alanine-dipeptide/plumed.datext")'>ext</b>
  BIAS_CUTOFF
  CUTOFF=30
  LAMBDA=1
... GAMBES


<br/><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div> <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=100 <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=COLVAR <div class="tooltip">FMT<div class="right">the format that should be used to output real numbers<i></i></div></div>=%.9f
</pre>
{% endraw %}
