**Project ID:** [plumID:23.003]({{ '/' | absolute_url }}eggs/23/003/)  
**Source:** Case_2/Prep/short_MD/MD/plumed_dihedral.dat  
**Originally used with PLUMED version:** 2.8  
**Stable:** [zipped raw stdout](plumed_dihedral.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_dihedral.dat.plumed.stderr.txt.zip) - [stderr](plumed_dihedral.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed_dihedral.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_dihedral.dat.plumed_master.stderr.txt.zip) - [stderr](plumed_dihedral.dat.plumed_master.stderr)  

{% raw %}
<div class="plumedInputContainer">
<div class="plumedpreheader">
<div class="headerInfo" id="value_details_data/Case_2/Prep/short_MD/MD/plumed_dihedral.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div class="containerBadge">
<div class="headerBadge"><a href="plumed_dihedral.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-passing-green.svg" alt="tested onv2.10" /></a></div>
<div class="headerBadge"><a href="plumed_dihedral.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></div>
</div>
</div>
<pre class="plumedlisting">
<b name="data/Case_2/Prep/short_MD/MD/plumed_dihedral.dattheta" onclick='showPath("data/Case_2/Prep/short_MD/MD/plumed_dihedral.dat","data/Case_2/Prep/short_MD/MD/plumed_dihedral.dattheta","data/Case_2/Prep/short_MD/MD/plumed_dihedral.dattheta","brown")'>theta</b>: <span class="plumedtooltip" style="color:green">TORSION<span class="right">Calculate one or multiple torsional angles. <a href="https://www.plumed.org/doc-master/user-doc/html/TORSION" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=1,2,3,4

<span style="display:none;" id="data/Case_2/Prep/short_MD/MD/plumed_dihedral.dattheta">The TORSION action with label <b>theta</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">theta.value</td><td>the TORSION involving these atoms</td></tr></table></span><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/PRINT" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=1 <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=<b name="data/Case_2/Prep/short_MD/MD/plumed_dihedral.dattheta">theta</b> <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=analysis.dat
</pre></div>

{% endraw %}
