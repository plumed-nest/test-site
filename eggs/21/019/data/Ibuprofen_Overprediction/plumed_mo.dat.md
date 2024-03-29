**Project ID:** [plumID:21.019]({{ '/' | absolute_url }}eggs/21/019/)  
**Source:** Ibuprofen_Overprediction/plumed_mo.dat  
**Originally used with PLUMED version:** 2.5-mod  
**Stable:** [zipped raw stdout](plumed_mo.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_mo.dat.plumed.stderr.txt.zip) - [stderr](plumed_mo.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed_mo.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_mo.dat.plumed_master.stderr.txt.zip) - [stderr](plumed_mo.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/Ibuprofen_Overprediction/plumed_mo.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed_mo.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-failed-red.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed_mo.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-failed-red.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue"># Define orientational vectors and angles</span>
<div class="tooltip" style="color:green">DISTANCE<div class="right">Calculate the distance between a pair of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html" style="color:green">More details</a><i></i></div></div> ...
<div class="tooltip">ATOMS1<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=6,10
<div class="tooltip">ATOMS2<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=39,43
<div class="tooltip">ATOMS3<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=72,76
<div class="tooltip">ATOMS4<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=105,109
...
<div class="tooltip">ATOMS285<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=9378,9382
<div class="tooltip">ATOMS286<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=9411,9415
<div class="tooltip">ATOMS287<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=9444,9448
<div class="tooltip">ATOMS288<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=9477,9481
<div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/Ibuprofen_Overprediction/plumed_mo.datdd_mo1" onclick='showPath("data/Ibuprofen_Overprediction/plumed_mo.dat","data/Ibuprofen_Overprediction/plumed_mo.datdd_mo1")'>dd_mo1</b>
<span style="display:none;" id="data/Ibuprofen_Overprediction/plumed_mo.datdd_mo1">The DISTANCE action with label <b>dd_mo1</b> calculates a scalar quantity</span><div class="tooltip" style="color:green">COMPONENTS<div class="right">This action is not part of PLUMED and was included by using a LOAD command <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></div></div>
... DISTANCE

vv_mo1 NORMALIZE ARG1=<b name="data/Ibuprofen_Overprediction/plumed_mo.datdd_mo1">dd_mo1.x</b> ARG2=<b name="data/Ibuprofen_Overprediction/plumed_mo.datdd_mo1">dd_mo1.y</b> ARG3=<b name="data/Ibuprofen_Overprediction/plumed_mo.datdd_mo1">dd_mo1.z</b>
dp_mat_mo1 DOTPRODUCT_MATRIX GROUP1=vv_mo1.x GROUP2=vv_mo1.y GROUP3=vv_mo1.z
ang_mat_mo1 MATHEVAL ARG1=dp_mat_mo1 FUNC=acos(x PERIODIC=NO

DISTANCE ...
ATOMS1=18,20
ATOMS2=51,53
ATOMS3=84,86
ATOMS4=117,119
...
ATOMS285=9390,9392
ATOMS286=9423,9425
ATOMS287=9456,9458
ATOMS288=9489,9491
LABEL=<b name="data/Ibuprofen_Overprediction/plumed_mo.datdd_mo2" onclick='showPath("data/Ibuprofen_Overprediction/plumed_mo.dat","data/Ibuprofen_Overprediction/plumed_mo.datdd_mo2")'>dd_mo2</b>
COMPONENTS
... DISTANCE
<br/><b name="data/Ibuprofen_Overprediction/plumed_mo.datvv_mo2" onclick='showPath("data/Ibuprofen_Overprediction/plumed_mo.dat","data/Ibuprofen_Overprediction/plumed_mo.datvv_mo2")'>vv_mo2</b>: <div class="tooltip" style="color:green">NORMALIZE<div class="right">This action is not part of PLUMED and was included by using a LOAD command <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></div></div> ARG1=<b name="data/Ibuprofen_Overprediction/plumed_mo.datdd_mo2">dd_mo2.x</b> ARG2=<b name="data/Ibuprofen_Overprediction/plumed_mo.datdd_mo2">dd_mo2.y</b> ARG3=<b name="data/Ibuprofen_Overprediction/plumed_mo.datdd_mo2">dd_mo2.z</b>
<b name="data/Ibuprofen_Overprediction/plumed_mo.datdp_mat_mo2" onclick='showPath("data/Ibuprofen_Overprediction/plumed_mo.dat","data/Ibuprofen_Overprediction/plumed_mo.datdp_mat_mo2")'>dp_mat_mo2</b>: <div class="tooltip" style="color:green">DOTPRODUCT_MATRIX<div class="right">This action is not part of PLUMED and was included by using a LOAD command <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></div></div> GROUP1=<b name="data/Ibuprofen_Overprediction/plumed_mo.datvv_mo2">vv_mo2.x</b> GROUP2=<b name="data/Ibuprofen_Overprediction/plumed_mo.datvv_mo2">vv_mo2.y</b> GROUP3=<b name="data/Ibuprofen_Overprediction/plumed_mo.datvv_mo2">vv_mo2.z</b>
<b name="data/Ibuprofen_Overprediction/plumed_mo.datang_mat_mo2" onclick='showPath("data/Ibuprofen_Overprediction/plumed_mo.dat","data/Ibuprofen_Overprediction/plumed_mo.datang_mat_mo2")'>ang_mat_mo2</b>: <div class="tooltip" style="color:green">MATHEVAL<div class="right">An alias to the ef CUSTOM function. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG1<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/Ibuprofen_Overprediction/plumed_mo.datdp_mat_mo2">dp_mat_mo2</b> <div class="tooltip">FUNC<div class="right">the function you wish to evaluate<i></i></div></div>=acos(x <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO
<br/><span style="color:blue"># Plot Distribution</span>
<span style="display:none;" id="data/Ibuprofen_Overprediction/plumed_mo.datang_mat_mo2">The MATHEVAL action with label <b>ang_mat_mo2</b> calculates a scalar quantity</span><b name="data/Ibuprofen_Overprediction/plumed_mo.datvalg_mo" onclick='showPath("data/Ibuprofen_Overprediction/plumed_mo.dat","data/Ibuprofen_Overprediction/plumed_mo.datvalg_mo")'>valg_mo</b>: <div class="tooltip" style="color:green">KDE<div class="right">This action is not part of PLUMED and was included by using a LOAD command <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></div></div> ARG1=ang_mat_mo1 ARG2=<b name="data/Ibuprofen_Overprediction/plumed_mo.datang_mat_mo2">ang_mat_mo2</b>  GRID_MIN=0.000,0.000 GRID_MAX=3.142,3.142 GRID_BIN=37,37 BANDWIDTH=0.250,0.250 KERNEL=GAUSSIAN
<div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/Ibuprofen_Overprediction/plumed_mo.datvalg_mo">valg_mo</b> <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=plumed_md_mo.dat
</pre>
{% endraw %}
