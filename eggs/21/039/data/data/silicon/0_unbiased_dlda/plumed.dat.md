**Project ID:** [plumID:21.039]({{ '/' | absolute_url }}eggs/21/039/)  
**Source:** data/silicon/0_unbiased_dlda/plumed.dat  
**Originally used with PLUMED version:** 2.8  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/data/silicon/0_unbiased_dlda/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-failed-red.svg" alt="tested onmaster" /></a></td></tr><tr><td style="padding:1px"><img src="https://img.shields.io/badge/with-LOAD-yellow.svg" alt="tested on master" /></td></tr>
</table></div></div>
<pre style="width=97%;">
<div class="tooltip" style="color:blue"># vim:ft=plumed<div class="right">Enables syntax highlighting for PLUMED files in vim. See <a href="https://www.plumed.org/doc-master/user-doc/html/_vim_syntax.html">here for more details. </a><i></i></div></div>
<br/><span style="color:blue">####################################</span>
<span style="color:blue">#  >> Silicon <<</span>
<span style="color:blue">#  DRIVER - Compute descriptors</span>
<span style="color:blue">####################################</span>
<br/><span style="color:blue"># Load Structure factor code</span>
<div class="tooltip" style="color:green">LOAD<div class="right">Loads a library, possibly defining new actions. <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">FILE<div class="right">file to be loaded<i></i></div></div>=../StructureFactor_descriptor.test.cpp
<br/><div class="tooltip" style="color:green">UNITS<div class="right">This command sets the internal units for the code. <a href="https://www.plumed.org/doc-master/user-doc/html/_u_n_i_t_s.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">LENGTH<div class="right">the units of lengths<i></i></div></div>=A
<br/><span style="color:blue"># Define Descriptors</span>
<b name="data/data/silicon/0_unbiased_dlda/plumed.datcv" onclick='showPath("data/data/silicon/0_unbiased_dlda/plumed.dat","data/data/silicon/0_unbiased_dlda/plumed.datcv")'>cv</b>: <div class="tooltip" style="color:green">STRUCTURE_FACTOR_DESCRIPTOR_TEST<div class="right">This action is not part of PLUMED and was included by using a LOAD command <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></div></div> ACTIVE_SHELLS=27,72,99,144,171,216,243,288,315 STRUCTURE=DIAMOND UNIT_CELLS=3
<br/><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=1  <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=COLVAR_DRIVER_SOLID <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/data/silicon/0_unbiased_dlda/plumed.datcv">cv</b>
<br/><div class="tooltip" style="color:green">ENDPLUMED<div class="right">Terminate plumed input. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html" style="color:green">More details</a><i></i></div></div><span style="color:blue">
</span></pre>
{% endraw %}
