**Project ID:** [plumID:19.015]({{ '/' | absolute_url }}eggs/19/015/)  
**Source:** surface/100_polar/plumed_kinetics.dat  
**Originally used with PLUMED version:** 2.3  
**Stable:** [zipped raw stdout](plumed_kinetics.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_kinetics.dat.plumed.stderr.txt.zip) - [stderr](plumed_kinetics.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed_kinetics.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_kinetics.dat.plumed_master.stderr.txt.zip) - [stderr](plumed_kinetics.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/surface/100_polar/plumed_kinetics.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed_kinetics.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-passing-green.svg" alt="tested onv2.10" /></a></td></tr><tr><td style="padding:1px"><a href="plumed_kinetics.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue" class="comment">#######IBU 28##########</span>

<br/><span style="color:blue" class="comment">#torsion1 between vector C1,C2 and C10,C11 with axis C2,C10</span>
<b name="data/surface/100_polar/plumed_kinetics.datt1" onclick='showPath("data/surface/100_polar/plumed_kinetics.dat","data/surface/100_polar/plumed_kinetics.datt1","data/surface/100_polar/plumed_kinetics.datt1","black")'>t1</b><span style="display:none;" id="data/surface/100_polar/plumed_kinetics.datt1">The TORSION action with label <b>t1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">t1</td><td width="5%"><font color="black">scalar</font></td><td>the TORSION involving these atoms</td></tr></table></span>: <span class="plumedtooltip" style="color:green">TORSION<span class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">VECTOR1<span class="right">two atoms that define a vector<i></i></span></span>=895,894 <span class="plumedtooltip">AXIS<span class="right">two atoms that define an axis<i></i></span></span>=895,903 <span class="plumedtooltip">VECTOR2<span class="right">two atoms that define a vector<i></i></span></span>=903,904

<span style="color:blue" class="comment">#torsion2 between vector C7,C10 and C11,C12 with axis C10,C11</span>
<b name="data/surface/100_polar/plumed_kinetics.datt2" onclick='showPath("data/surface/100_polar/plumed_kinetics.dat","data/surface/100_polar/plumed_kinetics.datt2","data/surface/100_polar/plumed_kinetics.datt2","black")'>t2</b><span style="display:none;" id="data/surface/100_polar/plumed_kinetics.datt2">The TORSION action with label <b>t2</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">t2</td><td width="5%"><font color="black">scalar</font></td><td>the TORSION involving these atoms</td></tr></table></span>: <span class="plumedtooltip" style="color:green">TORSION<span class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">VECTOR1<span class="right">two atoms that define a vector<i></i></span></span>=903,900 <span class="plumedtooltip">AXIS<span class="right">two atoms that define an axis<i></i></span></span>=903,904 <span class="plumedtooltip">VECTOR2<span class="right">two atoms that define a vector<i></i></span></span>=904,905

<span style="color:blue" class="comment">#metadynamics</span>
<span class="plumedtooltip" style="color:green">METAD<span class="right">Used to performed metadynamics on one or more collective variables. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_e_t_a_d.html" style="color:green">More details</a><i></i></span></span> ...
<span class="plumedtooltip">ARG<span class="right">the labels of the scalars on which the bias will act<i></i></span></span>=<b name="data/surface/100_polar/plumed_kinetics.datt1">t1</b>,<b name="data/surface/100_polar/plumed_kinetics.datt2">t2</b>
<span class="plumedtooltip">SIGMA<span class="right">the widths of the Gaussian hills<i></i></span></span>=0.1,0.1
<span class="plumedtooltip">HEIGHT<span class="right">the heights of the Gaussian hills<i></i></span></span>=0.24
<span class="plumedtooltip">PACE<span class="right">the frequency for hill addition<i></i></span></span>=1000
<span class="plumedtooltip">BIASFACTOR<span class="right">use well tempered metadynamics and use this bias factor<i></i></span></span>=5.0
<span class="plumedtooltip">TEMP<span class="right">the system temperature - this is only needed if you are doing well-tempered metadynamics<i></i></span></span>=300.0
<span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/surface/100_polar/plumed_kinetics.datmetad" onclick='showPath("data/surface/100_polar/plumed_kinetics.dat","data/surface/100_polar/plumed_kinetics.datmetad","data/surface/100_polar/plumed_kinetics.datmetad","black")'>metad</b><span style="display:none;" id="data/surface/100_polar/plumed_kinetics.datmetad">The METAD action with label <b>metad</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">metad.bias</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the bias potential</td></tr></table></span>
<span class="plumedtooltip">FILE<span class="right"> a file in which the list of added hills is stored<i></i></span></span>=HILLS
<span class="plumedtooltip">GRID_MIN<span class="right">the lower bounds for the grid<i></i></span></span>=-pi,-pi
<span class="plumedtooltip">GRID_MAX<span class="right">the upper bounds for the grid<i></i></span></span>=pi,pi
<span class="plumedtooltip">GRID_BIN<span class="right">the number of bins for the grid<i></i></span></span>=350,350
... METAD

<br/><span class="plumedtooltip" style="color:green">COMMITTOR<span class="right">Does a committor analysis. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_m_m_i_t_t_o_r.html" style="color:green">More details</a><i></i></span></span> ...
  <span class="plumedtooltip">ARG<span class="right">the labels of the values which is being used to define the committor surface<i></i></span></span>=<b name="data/surface/100_polar/plumed_kinetics.datt1">t1</b>,<b name="data/surface/100_polar/plumed_kinetics.datt2">t2</b>

<span style="color:blue" class="comment">#C1 basin</span>
  <span class="plumedtooltip">BASIN_LL1<span class="right">List of lower limits for basin #<i></i></span></span>=-3.15,-3.15
  <span class="plumedtooltip">BASIN_UL1<span class="right">List of upper limits for basin #<i></i></span></span>=-2.3,-2.85
  <span class="plumedtooltip">BASIN_LL2<span class="right">List of lower limits for basin #<i></i></span></span>=-3.15,3.13
  <span class="plumedtooltip">BASIN_UL2<span class="right">List of upper limits for basin #<i></i></span></span>=-2.3,3.15
  <span class="plumedtooltip">BASIN_LL3<span class="right">List of lower limits for basin #<i></i></span></span>=3.13,3.13
  <span class="plumedtooltip">BASIN_UL3<span class="right">List of upper limits for basin #<i></i></span></span>=3.15,3.15
  <span class="plumedtooltip">BASIN_LL4<span class="right">List of lower limits for basin #<i></i></span></span>=3.13,-3.15
  <span class="plumedtooltip">BASIN_UL4<span class="right">List of upper limits for basin #<i></i></span></span>=3.15,-2.85
  
<span style="color:blue" class="comment">#C2 basin</span>
   <span class="plumedtooltip">BASIN_LL5<span class="right">List of lower limits for basin #<i></i></span></span>=-2.7,-1.3
   <span class="plumedtooltip">BASIN_UL5<span class="right">List of upper limits for basin #<i></i></span></span>=-1.9,-1.0

<span style="color:blue" class="comment">#C3 basin</span>
   <span class="plumedtooltip">BASIN_LL6<span class="right">List of lower limits for basin #<i></i></span></span>=-2.7,0.9
   <span class="plumedtooltip">BASIN_UL6<span class="right">List of upper limits for basin #<i></i></span></span>=-2.3,1.2

<span style="color:blue" class="comment">#C4 basin</span>
   <span class="plumedtooltip">BASIN_LL7<span class="right">List of lower limits for basin #<i></i></span></span>=-0.1,-3.15
   <span class="plumedtooltip">BASIN_UL7<span class="right">List of upper limits for basin #<i></i></span></span>=0.85,-2.85
   <span class="plumedtooltip">BASIN_LL8<span class="right">List of lower limits for basin #<i></i></span></span>=-0.1,3.13
   <span class="plumedtooltip">BASIN_UL8<span class="right">List of upper limits for basin #<i></i></span></span>=0.85,3.15

<span style="color:blue" class="comment">#C5 basin</span>
<span style="color:blue" class="comment">#   BASIN_LL5=0.5,-1.3</span>
<span style="color:blue" class="comment">#   BASIN_UL5=1.3,-1.0</span>

<span style="color:blue" class="comment">#C6 basin</span>
   <span class="plumedtooltip">BASIN_LL9<span class="right">List of lower limits for basin #<i></i></span></span>=0.5,0.9
   <span class="plumedtooltip">BASIN_UL9<span class="right">List of upper limits for basin #<i></i></span></span>=1.0,1.2
  
... COMMITTOR

<br/><span style="display:none;" id="data/surface/100_polar/plumed_kinetics.dat">The COMMITTOR action with label <b></b> calculates something</span><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=<b name="data/surface/100_polar/plumed_kinetics.datt1">t1</b>,<b name="data/surface/100_polar/plumed_kinetics.datt2">t2</b>,<b name="data/surface/100_polar/plumed_kinetics.datmetad">metad.bias</b> <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=10 <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=COLVAR
</pre>
{% endraw %}
