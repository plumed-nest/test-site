**Project ID:** [plumID:21.009]({{ '/' | absolute_url }}eggs/21/009/)  
**Source:** npt-committor/recross/plumed.inp  
**Originally used with PLUMED version:** 2.6  
**Stable:** [zipped raw stdout](plumed.inp.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed.stderr.txt.zip) - [stderr](plumed.inp.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.inp.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed_master.stderr.txt.zip) - [stderr](plumed.inp.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/npt-committor/recross/plumed.inp"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.inp.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.inp.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<div class="tooltip" style="color:green">UNITS<div class="right">This command sets the internal units for the code. <a href="https://www.plumed.org/doc-master/user-doc/html/_u_n_i_t_s.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">LENGTH<div class="right">the units of lengths<i></i></div></div>=A
<br/><div class="tooltip" style="color:green">COORDINATIONNUMBER<div class="right">Calculate the coordination numbers of atoms so that you can then calculate functions of the distribution of <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html" style="color:green">More details</a><i></i></div></div> ...
  <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/npt-committor/recross/plumed.inpcoord" onclick='showPath("data/npt-committor/recross/plumed.inp","data/npt-committor/recross/plumed.inpcoord")'>coord</b>
  <div class="tooltip">SPECIES<div class="right">this keyword is used for colvars such as coordination number<i></i></div></div>=1-512
  <div class="tooltip">SWITCH<div class="right">This keyword is used if you want to employ an alternative to the continuous switching function defined above<i></i></div></div>={RATIONAL R_0=5.0 D_MAX=10.0}
  <div class="tooltip">MORE_THAN<div class="right">calculate the number of variables more than a certain target value<i></i></div></div>={RATIONAL R_0=5.0 D_MAX=5.5}
  <div class="tooltip">LOWMEM<div class="right"> lower the memory requirements<i></i></div></div>
... COORDINATIONNUMBER
<br/><span style="display:none;" id="data/npt-committor/recross/plumed.inpcoord">The COORDINATIONNUMBER action with label <b>coord</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">coord.morethan</td><td>the number of values more than a target value</td></tr></table></span><div class="tooltip" style="color:green">COMMITTOR<div class="right">Does a committor analysis. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_m_m_i_t_t_o_r.html" style="color:green">More details</a><i></i></div></div> ...
  <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/npt-committor/recross/plumed.inpcoord">coord.morethan</b>
  <div class="tooltip">STRIDE<div class="right"> the frequency with which the CVs are analyzed<i></i></div></div>=1
  <div class="tooltip">BASIN_LL1<div class="right">List of lower limits for basin #<i></i></div></div>=0
  <div class="tooltip">BASIN_UL1<div class="right">List of upper limits for basin #<i></i></div></div>=19
  <div class="tooltip">BASIN_LL2<div class="right">List of lower limits for basin #<i></i></div></div>=19
  <div class="tooltip">BASIN_UL2<div class="right">List of upper limits for basin #<i></i></div></div>=120
  <div class="tooltip">NOSTOP<div class="right"> if true do not stop the simulation when reaching a basin but just keep track of it<i></i></div></div>
  <div class="tooltip">FILE<div class="right">the name of the file on which to output the reached basin<i></i></div></div>=commit
... COMMITTOR
<br/><div class="tooltip" style="color:green">FLUSH<div class="right">This command instructs plumed to flush all the open files with a user specified frequency. <a href="https://www.plumed.org/doc-master/user-doc/html/_f_l_u_s_h.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">STRIDE<div class="right">the frequency with which all the open files should be flushed<i></i></div></div>=200000
<div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/npt-committor/recross/plumed.inpcoord">coord.morethan</b> <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=2000 <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=colvar
</pre>
{% endraw %}
