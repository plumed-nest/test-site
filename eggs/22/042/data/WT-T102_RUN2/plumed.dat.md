**Project ID:** [plumID:22.042]({{ '/' | absolute_url }}eggs/22/042/)  
**Source:** WT-T102_RUN2/plumed.dat  
**Originally used with PLUMED version:** 2.7.3  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/WT-T102_RUN2/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<b name="data/WT-T102_RUN2/plumed.datphi" onclick='showPath("data/WT-T102_RUN2/plumed.dat","data/WT-T102_RUN2/plumed.datphi")'>phi</b>: <div class="tooltip" style="color:green">TORSION<div class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the four atoms involved in the torsional angle<i></i></div></div>=1377,1379,1381,1391
<span style="display:none;" id="data/WT-T102_RUN2/plumed.datphi">The TORSION action with label <b>phi</b> calculates a scalar quantity</span><b name="data/WT-T102_RUN2/plumed.datpsi" onclick='showPath("data/WT-T102_RUN2/plumed.dat","data/WT-T102_RUN2/plumed.datpsi")'>psi</b>: <div class="tooltip" style="color:green">TORSION<div class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the four atoms involved in the torsional angle<i></i></div></div>=1379,1381,1391,1393
<br/><span style="display:none;" id="data/WT-T102_RUN2/plumed.datpsi">The TORSION action with label <b>psi</b> calculates a scalar quantity</span><div class="tooltip" style="color:green">METAD<div class="right">Used to performed metadynamics on one or more collective variables. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_e_t_a_d.html" style="color:green">More details</a><i></i></div></div> ...
  <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/WT-T102_RUN2/plumed.datphi">phi</b>,<b name="data/WT-T102_RUN2/plumed.datpsi">psi</b>
  <div class="tooltip">PACE<div class="right">the frequency for hill addition<i></i></div></div>=100
  <div class="tooltip">HEIGHT<div class="right">the heights of the Gaussian hills<i></i></div></div>=0.5
  <div class="tooltip">SIGMA<div class="right">the widths of the Gaussian hills<i></i></div></div>=0.1,0.1
  <div class="tooltip">BIASFACTOR<div class="right">use well tempered metadynamics and use this bias factor<i></i></div></div>=15.0
  <div class="tooltip">FILE<div class="right"> a file in which the list of added hills is stored<i></i></div></div>=HILLS
  <div class="tooltip">GRID_MIN<div class="right">the lower bounds for the grid<i></i></div></div>=-pi,-pi
  <div class="tooltip">GRID_MAX<div class="right">the upper bounds for the grid<i></i></div></div>=pi,pi
  <div class="tooltip">TEMP<div class="right">the system temperature - this is only needed if you are doing well-tempered metadynamics<i></i></div></div>=300
  <div class="tooltip">FMT<div class="right">specify format for HILLS files (useful for decrease the number of digits in regtests)<i></i></div></div>=%14.6f
... METAD
<br/><span style="display:none;" id="data/WT-T102_RUN2/plumed.dat">The METAD action with label <b></b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">.bias</td><td>the instantaneous value of the bias potential</td></tr></table></span><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div> <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=100 <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=COLVAR
</pre>
{% endraw %}
