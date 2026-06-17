**Project ID:** [plumID:24.036]({{ '/' | absolute_url }}eggs/24/036/)  
**Source:** PLIT/plumed_water.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [zipped raw stdout](plumed_water.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_water.dat.plumed.stderr.txt.zip) - [stderr](plumed_water.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed_water.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_water.dat.plumed_master.stderr.txt.zip) - [stderr](plumed_water.dat.plumed_master.stderr)  

{% raw %}
<div class="plumedInputContainer">
<div class="plumedpreheader">
<div class="headerInfo" id="value_details_data/PLIT/plumed_water.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div class="containerBadge">
<div class="headerBadge"><a href="plumed_water.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-passing-green.svg" alt="tested onv2.10" /></a></div>
<div class="headerBadge"><a href="plumed_water.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></div>
</div>
</div>
<pre class="plumedlisting">
<span class="plumedtooltip" style="color:green">WHOLEMOLECULES<span class="right">This action is used to rebuild molecules that can become split by the periodic boundary conditions. <a href="https://www.plumed.org/doc-master/user-doc/html/WHOLEMOLECULES" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ENTITY0<span class="right">the atoms that make up a molecule that you wish to align<i></i></span></span>=1-6951

<span style="display:none;" id="data/PLIT/plumed_water.dat">The WHOLEMOLECULES action with label <b></b> calculates something</span><b name="data/PLIT/plumed_water.datd0" onclick='showPath("data/PLIT/plumed_water.dat","data/PLIT/plumed_water.datd0","data/PLIT/plumed_water.datd0","brown")'>d0</b>:  <span class="plumedtooltip" style="color:green">DISTANCE<span class="right">Calculate the distance/s between pairs of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/DISTANCE" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS<span class="right">the pair of atom that we are calculating the distance between<i></i></span></span>=5825,6817

<span style="display:none;" id="data/PLIT/plumed_water.datd0">The DISTANCE action with label <b>d0</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">d0.value</td><td>the DISTANCE between this pair of atoms</td></tr></table></span><b name="data/PLIT/plumed_water.datwater" onclick='showPath("data/PLIT/plumed_water.dat","data/PLIT/plumed_water.datwater","data/PLIT/plumed_water.datwater","brown")'>water</b>: <span class="plumedtooltip" style="color:green">GROUP<span class="right">Define a group of atoms so that a particular list of atoms can be referenced with a single label in definitions of CVs or virtual atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/GROUP" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS<span class="right">the numerical indexes for the set of atoms in the group<i></i></span></span>=7011-62733:3

<span style="display:none;" id="data/PLIT/plumed_water.datwater">The GROUP action with label <b>water</b> calculates something</span><span class="plumedtooltip" style="color:green">COORDINATION<span class="right">Calculate coordination numbers. <a href="https://www.plumed.org/doc-master/user-doc/html/COORDINATION" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">GROUPA<span class="right">First list of atoms<i></i></span></span>=5825 <span class="plumedtooltip">GROUPB<span class="right">Second list of atoms (if empty, N*(N-1)/2 pairs in GROUPA are counted)<i></i></span></span>=<b name="data/PLIT/plumed_water.datwater">water</b> <span class="plumedtooltip">R_0<span class="right">The r_0 parameter of the switching function<i></i></span></span>=0.33
<span class="plumedtooltip" style="color:green">COORDINATION<span class="right">Calculate coordination numbers. <a href="https://www.plumed.org/doc-master/user-doc/html/COORDINATION" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">GROUPA<span class="right">First list of atoms<i></i></span></span>=6817 <span class="plumedtooltip">GROUPB<span class="right">Second list of atoms (if empty, N*(N-1)/2 pairs in GROUPA are counted)<i></i></span></span>=<b name="data/PLIT/plumed_water.datwater">water</b> <span class="plumedtooltip">R_0<span class="right">The r_0 parameter of the switching function<i></i></span></span>=0.33

<span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/PRINT" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=*   <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=1   <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=COLVAR 
</pre></div>

{% endraw %}
