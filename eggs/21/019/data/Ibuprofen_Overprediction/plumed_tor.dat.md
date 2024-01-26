**Project ID:** [plumID:21.019]({{ '/' | absolute_url }}eggs/21/019/)  
**Source:** Ibuprofen_Overprediction/plumed_tor.dat  
**Originally used with PLUMED version:** 2.5-mod  
**Stable:** [zipped raw stdout](plumed_tor.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_tor.dat.plumed.stderr.txt.zip) - [stderr](plumed_tor.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed_tor.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_tor.dat.plumed_master.stderr.txt.zip) - [stderr](plumed_tor.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/Ibuprofen_Overprediction/plumed_tor.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed_tor.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-failed-red.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed_tor.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-failed-red.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue"># Define Torsional angles</span>
<div class="tooltip" style="color:green">TORSIONS<div class="right">Calculate whether or not a set of torsional angles are within a particular range. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n_s.html" style="color:green">More details</a><i></i></div></div> ...
<div class="tooltip">ATOMS1<div class="right">the atoms involved in each of the torsion angles you wish to calculate<i></i></div></div>=74,79,70,73
<div class="tooltip">ATOMS2<div class="right">the atoms involved in each of the torsion angles you wish to calculate<i></i></div></div>=107,112,103,106
<div class="tooltip">ATOMS3<div class="right">the atoms involved in each of the torsion angles you wish to calculate<i></i></div></div>=206,211,202,205
<div class="tooltip">ATOMS4<div class="right">the atoms involved in each of the torsion angles you wish to calculate<i></i></div></div>=239,244,235,238
...
<div class="tooltip">ATOMS141<div class="right">the atoms involved in each of the torsion angles you wish to calculate<i></i></div></div>=9314,9319,9310,9313
<div class="tooltip">ATOMS142<div class="right">the atoms involved in each of the torsion angles you wish to calculate<i></i></div></div>=9347,9352,9343,9346
<div class="tooltip">ATOMS143<div class="right">the atoms involved in each of the torsion angles you wish to calculate<i></i></div></div>=9446,9451,9442,9445
<div class="tooltip">ATOMS144<div class="right">the atoms involved in each of the torsion angles you wish to calculate<i></i></div></div>=9479,9484,9475,9478
<div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/Ibuprofen_Overprediction/plumed_tor.datGlobal" onclick='showPath("data/Ibuprofen_Overprediction/plumed_tor.dat","data/Ibuprofen_Overprediction/plumed_tor.datGlobal")'>Global</b>
... TORSIONS

TORSIONS ...
<div class="tooltip">ATOMS1<div class="right">the atoms involved in each of the torsion angles you wish to calculate<i></i></div></div>=76,79,74,75
<div class="tooltip">ATOMS2<div class="right">the atoms involved in each of the torsion angles you wish to calculate<i></i></div></div>=109,112,107,108
<div class="tooltip">ATOMS3<div class="right">the atoms involved in each of the torsion angles you wish to calculate<i></i></div></div>=208,211,206,207
<div class="tooltip">ATOMS4<div class="right">the atoms involved in each of the torsion angles you wish to calculate<i></i></div></div>=241,244,239,240
...
<div class="tooltip">ATOMS141<div class="right">the atoms involved in each of the torsion angles you wish to calculate<i></i></div></div>=9316,9319,9314,9315
<div class="tooltip">ATOMS142<div class="right">the atoms involved in each of the torsion angles you wish to calculate<i></i></div></div>=9349,9352,9347,9348
<div class="tooltip">ATOMS143<div class="right">the atoms involved in each of the torsion angles you wish to calculate<i></i></div></div>=9448,9451,9446,9447
<div class="tooltip">ATOMS144<div class="right">the atoms involved in each of the torsion angles you wish to calculate<i></i></div></div>=9481,9484,9479,9480
<div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/Ibuprofen_Overprediction/plumed_tor.datGlobal" onclick='showPath("data/Ibuprofen_Overprediction/plumed_tor.dat","data/Ibuprofen_Overprediction/plumed_tor.datGlobal")'>Local</b>
... TORSIONS
<br/><span style="color:blue"># Plot 2D distribution</span>
<span style="display:none;" id="data/Ibuprofen_Overprediction/plumed_tor.datGlobal">The TORSIONS action with label <b>Global</b> calculates a scalar quantity</span><b name="data/Ibuprofen_Overprediction/plumed_tor.datkde_Stor" onclick='showPath("data/Ibuprofen_Overprediction/plumed_tor.dat","data/Ibuprofen_Overprediction/plumed_tor.datkde_Stor")'>kde_Stor</b>: <div class="tooltip" style="color:green">KDE<div class="right">This action is not part of PLUMED and was included by using a LOAD command <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></div></div> ARG1=<b name="data/Ibuprofen_Overprediction/plumed_tor.datGlobal">Global</b> ARG2=Local  GRID_MIN=-3.142,-3.142 GRID_MAX=3.142,3.142 GRID_BIN=73,73 BANDWIDTH=0.250,0.250 KERNEL=GAUSSIAN
<br/><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/Ibuprofen_Overprediction/plumed_tor.datkde_Stor">kde_Stor</b> <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=plumed_md_tor.dat
</pre>
{% endraw %}
