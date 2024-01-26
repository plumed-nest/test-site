**Project ID:** [plumID:19.071]({{ '/' | absolute_url }}eggs/19/071/)  
**Source:** MFI_paper_scripts/Ibuprofen_patching/plumed_c4c5c6_escape.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [zipped raw stdout](plumed_c4c5c6_escape.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_c4c5c6_escape.dat.plumed.stderr.txt.zip) - [stderr](plumed_c4c5c6_escape.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed_c4c5c6_escape.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_c4c5c6_escape.dat.plumed_master.stderr.txt.zip) - [stderr](plumed_c4c5c6_escape.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/MFI_paper_scripts/Ibuprofen_patching/plumed_c4c5c6_escape.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed_c4c5c6_escape.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed_c4c5c6_escape.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue">#torsion1 between vector C1,C2 and C10,C11 with axis C2,C10</span>
<b name="data/MFI_paper_scripts/Ibuprofen_patching/plumed_c4c5c6_escape.datt1" onclick='showPath("data/MFI_paper_scripts/Ibuprofen_patching/plumed_c4c5c6_escape.dat","data/MFI_paper_scripts/Ibuprofen_patching/plumed_c4c5c6_escape.datt1")'>t1</b>: <div class="tooltip" style="color:green">TORSION<div class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">VECTOR1<div class="right">two atoms that define a vector<i></i></div></div>=5911,5910 <div class="tooltip">AXIS<div class="right">two atoms that define an axis<i></i></div></div>=5919,5911 <div class="tooltip">VECTOR2<div class="right">two atoms that define a vector<i></i></div></div>=5919,5920
<br/><span style="color:blue">#torsion2 between vector C7,C10 and C11,C12 with axis C10,C11</span>
<span style="display:none;" id="data/MFI_paper_scripts/Ibuprofen_patching/plumed_c4c5c6_escape.datt1">The TORSION action with label <b>t1</b> calculates a scalar quantity</span><b name="data/MFI_paper_scripts/Ibuprofen_patching/plumed_c4c5c6_escape.datt2" onclick='showPath("data/MFI_paper_scripts/Ibuprofen_patching/plumed_c4c5c6_escape.dat","data/MFI_paper_scripts/Ibuprofen_patching/plumed_c4c5c6_escape.datt2")'>t2</b>: <div class="tooltip" style="color:green">TORSION<div class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">VECTOR1<div class="right">two atoms that define a vector<i></i></div></div>=5919,5916 <div class="tooltip">AXIS<div class="right">two atoms that define an axis<i></i></div></div>=5920,5919 <div class="tooltip">VECTOR2<div class="right">two atoms that define a vector<i></i></div></div>=5920,5921
<br/><span style="color:blue">#metadynamics</span>
<span style="display:none;" id="data/MFI_paper_scripts/Ibuprofen_patching/plumed_c4c5c6_escape.datt2">The TORSION action with label <b>t2</b> calculates a scalar quantity</span><div class="tooltip" style="color:green">METAD<div class="right">Used to performed metadynamics on one or more collective variables. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_e_t_a_d.html" style="color:green">More details</a><i></i></div></div> ...
<div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/MFI_paper_scripts/Ibuprofen_patching/plumed_c4c5c6_escape.datt1">t1</b>,<b name="data/MFI_paper_scripts/Ibuprofen_patching/plumed_c4c5c6_escape.datt2">t2</b>
<div class="tooltip">SIGMA<div class="right">the widths of the Gaussian hills<i></i></div></div>=0.1,0.1
<div class="tooltip">HEIGHT<div class="right">the heights of the Gaussian hills<i></i></div></div>=0.24
<div class="tooltip">PACE<div class="right">the frequency for hill addition<i></i></div></div>=1000
<div class="tooltip">BIASFACTOR<div class="right">use well tempered metadynamics and use this bias factor<i></i></div></div>=5.0
<div class="tooltip">TEMP<div class="right">the system temperature - this is only needed if you are doing well-tempered metadynamics<i></i></div></div>=300.0
<div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/MFI_paper_scripts/Ibuprofen_patching/plumed_c4c5c6_escape.datmetad" onclick='showPath("data/MFI_paper_scripts/Ibuprofen_patching/plumed_c4c5c6_escape.dat","data/MFI_paper_scripts/Ibuprofen_patching/plumed_c4c5c6_escape.datmetad")'>metad</b>
<div class="tooltip">FILE<div class="right"> a file in which the list of added hills is stored<i></i></div></div>=HILLS
<div class="tooltip">GRID_MIN<div class="right">the lower bounds for the grid<i></i></div></div>=-pi,-pi
<div class="tooltip">GRID_MAX<div class="right">the upper bounds for the grid<i></i></div></div>=pi,pi
<div class="tooltip">GRID_BIN<div class="right">the number of bins for the grid<i></i></div></div>=350,350
... METAD

<br/><span style="display:none;" id="data/MFI_paper_scripts/Ibuprofen_patching/plumed_c4c5c6_escape.datmetad">The METAD action with label <b>metad</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">metad.bias</td><td>the instantaneous value of the bias potential</td></tr></table></span><div class="tooltip" style="color:green">COMMITTOR<div class="right">Does a committor analysis. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_m_m_i_t_t_o_r.html" style="color:green">More details</a><i></i></div></div> ...
  <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/MFI_paper_scripts/Ibuprofen_patching/plumed_c4c5c6_escape.datt1">t1</b>,<b name="data/MFI_paper_scripts/Ibuprofen_patching/plumed_c4c5c6_escape.datt2">t2</b>

<span style="color:blue">#C1 basin</span>
  <div class="tooltip">BASIN_LL1<div class="right">List of lower limits for basin #<i></i></div></div>=-pi,-pi
  <div class="tooltip">BASIN_UL1<div class="right">List of upper limits for basin #<i></i></div></div>=-2.93,-2.7
  <div class="tooltip">BASIN_LL2<div class="right">List of lower limits for basin #<i></i></div></div>=-pi,3.13
  <div class="tooltip">BASIN_UL2<div class="right">List of upper limits for basin #<i></i></div></div>=-3.13,pi
  <div class="tooltip">BASIN_LL3<div class="right">List of lower limits for basin #<i></i></div></div>=3.13,3.13
  <div class="tooltip">BASIN_UL3<div class="right">List of upper limits for basin #<i></i></div></div>=pi,pi
  <div class="tooltip">BASIN_LL4<div class="right">List of lower limits for basin #<i></i></div></div>=2.6,-pi
  <div class="tooltip">BASIN_UL4<div class="right">List of upper limits for basin #<i></i></div></div>=pi,-2.6
  
<span style="color:blue">#C2 basin</span>
  <div class="tooltip">BASIN_LL5<div class="right">List of lower limits for basin #<i></i></div></div>=-2.7,-1.15
  <div class="tooltip">BASIN_UL5<div class="right">List of upper limits for basin #<i></i></div></div>=-1.8,-0.6

<span style="color:blue">#C3 basin</span>
   <div class="tooltip">BASIN_LL6<div class="right">List of lower limits for basin #<i></i></div></div>=-pi,0.6
   <div class="tooltip">BASIN_UL6<div class="right">List of upper limits for basin #<i></i></div></div>=-2.9,1.1
   <div class="tooltip">BASIN_LL7<div class="right">List of lower limits for basin #<i></i></div></div>=2.9,0.6
   <div class="tooltip">BASIN_UL7<div class="right">List of upper limits for basin #<i></i></div></div>=pi,1.1

... COMMITTOR

<br/><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/MFI_paper_scripts/Ibuprofen_patching/plumed_c4c5c6_escape.datt1">t1</b>,<b name="data/MFI_paper_scripts/Ibuprofen_patching/plumed_c4c5c6_escape.datt2">t2</b>,<b name="data/MFI_paper_scripts/Ibuprofen_patching/plumed_c4c5c6_escape.datmetad">metad.bias</b> <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=10 <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=COLVAR
</pre>
{% endraw %}
