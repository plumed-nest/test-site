**Project ID:** [plumID:21.019]({{ '/' | absolute_url }}eggs/21/019/)  
**Source:** Ibuprofen_Overprediction/plumed_tor.dat  
**Originally used with PLUMED version:** 2.5-mod  
**Stable:** [zipped raw stdout](plumed_tor.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_tor.dat.plumed.stderr.txt.zip) - [stderr](plumed_tor.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed_tor.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_tor.dat.plumed_master.stderr.txt.zip) - [stderr](plumed_tor.dat.plumed_master.stderr)  

{% raw %}
<div class="plumedInputContainer">
<div class="plumedpreheader">
<div class="headerInfo" id="value_details_data/Ibuprofen_Overprediction/plumed_tor.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div class="containerBadge">
<div class="headerBadge"><a href="plumed_tor.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-failed-red.svg" alt="tested onv2.10" /></a></div>
<div class="headerBadge"><a href="plumed_tor.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-failed-red.svg" alt="tested onmaster" /></a></div>
</div>
</div>
<pre class="plumedlisting">
<span style="color:blue" class="comment"># Define Torsional angles</span>
<span class="plumedtooltip" style="color:green">TORSIONS<span class="right">Calculate whether or not a set of torsional angles are within a particular range. <a href="https://www.plumed.org/doc-master/user-doc/html/TORSIONS" style="color:green">More details</a><i></i></span></span> ...
<span class="plumedtooltip">ATOMS1<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=74,79,70,73
<span class="plumedtooltip">ATOMS2<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=107,112,103,106
<span class="plumedtooltip">ATOMS3<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=206,211,202,205
<span class="plumedtooltip">ATOMS4<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=239,244,235,238
...
<span class="plumedtooltip">ATOMS141<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=9314,9319,9310,9313
<span class="plumedtooltip">ATOMS142<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=9347,9352,9343,9346
<span class="plumedtooltip">ATOMS143<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=9446,9451,9442,9445
<span class="plumedtooltip">ATOMS144<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=9479,9484,9475,9478
<span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/Ibuprofen_Overprediction/plumed_tor.datGlobal" onclick='showPath("data/Ibuprofen_Overprediction/plumed_tor.dat","data/Ibuprofen_Overprediction/plumed_tor.datGlobal","data/Ibuprofen_Overprediction/plumed_tor.datGlobal","brown")'>Global</b>
... TORSIONS

TORSIONS ...
<span class="plumedtooltip">ATOMS1<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=76,79,74,75
<span class="plumedtooltip">ATOMS2<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=109,112,107,108
<span class="plumedtooltip">ATOMS3<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=208,211,206,207
<span class="plumedtooltip">ATOMS4<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=241,244,239,240
...
<span class="plumedtooltip">ATOMS141<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=9316,9319,9314,9315
<span class="plumedtooltip">ATOMS142<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=9349,9352,9347,9348
<span class="plumedtooltip">ATOMS143<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=9448,9451,9446,9447
<span class="plumedtooltip">ATOMS144<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=9481,9484,9479,9480
<span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/Ibuprofen_Overprediction/plumed_tor.datGlobal" onclick='showPath("data/Ibuprofen_Overprediction/plumed_tor.dat","data/Ibuprofen_Overprediction/plumed_tor.datGlobal","data/Ibuprofen_Overprediction/plumed_tor.datGlobal","brown")'>Local</b>
... TORSIONS
<br/><span style="color:blue" class="comment"># Plot 2D distribution</span>
<span style="display:none;" id="data/Ibuprofen_Overprediction/plumed_tor.datGlobal">The TORSIONS action with label <b>Global</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">Global.value</td><td>the TORSION for each set of three atoms that were specified</td></tr></table></span><b name="data/Ibuprofen_Overprediction/plumed_tor.datkde_Stor" onclick='showPath("data/Ibuprofen_Overprediction/plumed_tor.dat","data/Ibuprofen_Overprediction/plumed_tor.datkde_Stor","data/Ibuprofen_Overprediction/plumed_tor.datkde_Stor","brown")'>kde_Stor</b>: <span class="plumedtooltip" style="color:green">KDE<span class="right">Create a histogram from the input scalar/vector/matrix using KDE <a href="https://www.plumed.org/doc-master/user-doc/html/KDE" style="color:green">More details</a><i></i></span></span> ARG1=<b name="data/Ibuprofen_Overprediction/plumed_tor.datGlobal">Global</b> ARG2=Local  <span class="plumedtooltip">GRID_MIN<span class="right"> the lower bounds for the grid<i></i></span></span>=-3.142,-3.142 <span class="plumedtooltip">GRID_MAX<span class="right"> the upper bounds for the grid<i></i></span></span>=3.142,3.142 <span class="plumedtooltip">GRID_BIN<span class="right">the number of bins for the grid<i></i></span></span>=73,73 <span class="plumedtooltip">BANDWIDTH<span class="right">the bandwidths for kernel density esimtation<i></i></span></span>=0.250,0.250 <span class="plumedtooltip">KERNEL<span class="right"> the kernel function you are using<i></i></span></span>=GAUSSIAN

<span style="display:none;" id="data/Ibuprofen_Overprediction/plumed_tor.datkde_Stor">The KDE action with label <b>kde_Stor</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">kde_Stor.value</td><td>a function on a grid that was obtained by doing a Kernel Density Estimation using the input arguments</td></tr></table></span><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/PRINT" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=<b name="data/Ibuprofen_Overprediction/plumed_tor.datkde_Stor">kde_Stor</b> <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=plumed_md_tor.dat
</pre></div>

{% endraw %}
