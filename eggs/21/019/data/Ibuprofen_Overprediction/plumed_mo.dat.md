**Project ID:** [plumID:21.019]({{ '/' | absolute_url }}eggs/21/019/)  
**Source:** Ibuprofen_Overprediction/plumed_mo.dat  
**Originally used with PLUMED version:** 2.5-mod  
**Stable:** [zipped raw stdout](plumed_mo.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_mo.dat.plumed.stderr.txt.zip) - [stderr](plumed_mo.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed_mo.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_mo.dat.plumed_master.stderr.txt.zip) - [stderr](plumed_mo.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/Ibuprofen_Overprediction/plumed_mo.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed_mo.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-failed-red.svg" alt="tested onv2.10" /></a></td></tr><tr><td style="padding:1px"><a href="plumed_mo.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-failed-red.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue" class="comment"># Define orientational vectors and angles</span>
<span class="plumedtooltip" style="color:green">DISTANCE<span class="right">Calculate the distance between a pair of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html" style="color:green">More details</a><i></i></span></span> ...
<span class="plumedtooltip">ATOMS1<span class="right">the pair of atom that we are calculating the distance between<i></i></span></span>=6,10
<span class="plumedtooltip">ATOMS2<span class="right">the pair of atom that we are calculating the distance between<i></i></span></span>=39,43
<span class="plumedtooltip">ATOMS3<span class="right">the pair of atom that we are calculating the distance between<i></i></span></span>=72,76
<span class="plumedtooltip">ATOMS4<span class="right">the pair of atom that we are calculating the distance between<i></i></span></span>=105,109
...
<span class="plumedtooltip">ATOMS285<span class="right">the pair of atom that we are calculating the distance between<i></i></span></span>=9378,9382
<span class="plumedtooltip">ATOMS286<span class="right">the pair of atom that we are calculating the distance between<i></i></span></span>=9411,9415
<span class="plumedtooltip">ATOMS287<span class="right">the pair of atom that we are calculating the distance between<i></i></span></span>=9444,9448
<span class="plumedtooltip">ATOMS288<span class="right">the pair of atom that we are calculating the distance between<i></i></span></span>=9477,9481
<span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/Ibuprofen_Overprediction/plumed_mo.datdd_mo1" onclick='showPath("data/Ibuprofen_Overprediction/plumed_mo.dat","data/Ibuprofen_Overprediction/plumed_mo.datdd_mo1","data/Ibuprofen_Overprediction/plumed_mo.datdd_mo1","brown")'>dd_mo1</b>
<span style="display:none;" id="data/Ibuprofen_Overprediction/plumed_mo.datdd_mo1">The DISTANCE action with label <b>dd_mo1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">dd_mo1.value</td><td>the DISTANCE between this pair of atoms</td></tr></table></span><span class="plumedtooltip" style="color:green">COMPONENTS<span class="right">This action is not part of PLUMED and was included by using a LOAD command <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></span></span>
... DISTANCE

vv_mo1 NORMALIZE ARG1=<b name="data/Ibuprofen_Overprediction/plumed_mo.datdd_mo1">dd_mo1.x</b> ARG2=<b name="data/Ibuprofen_Overprediction/plumed_mo.datdd_mo1">dd_mo1.y</b> ARG3=<b name="data/Ibuprofen_Overprediction/plumed_mo.datdd_mo1">dd_mo1.z</b>
dp_mat_mo1 DOTPRODUCT_MATRIX GROUP1=vv_mo1.x GROUP2=vv_mo1.y GROUP3=vv_mo1.z
ang_mat_mo1 MATHEVAL ARG1=dp_mat_mo1 FUNC=acos(x) PERIODIC=NO

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
LABEL=<b name="data/Ibuprofen_Overprediction/plumed_mo.datdd_mo2" onclick='showPath("data/Ibuprofen_Overprediction/plumed_mo.dat","data/Ibuprofen_Overprediction/plumed_mo.datdd_mo2","data/Ibuprofen_Overprediction/plumed_mo.datdd_mo2","brown")'>dd_mo2</b>
COMPONENTS
... DISTANCE
<br/><b name="data/Ibuprofen_Overprediction/plumed_mo.datvv_mo2" onclick='showPath("data/Ibuprofen_Overprediction/plumed_mo.dat","data/Ibuprofen_Overprediction/plumed_mo.datvv_mo2","data/Ibuprofen_Overprediction/plumed_mo.datvv_mo2","brown")'>vv_mo2</b>: <span class="plumedtooltip" style="color:green">NORMALIZE<span class="right">This action is not part of PLUMED and was included by using a LOAD command <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></span></span> ARG1=dd_mo2.x ARG2=dd_mo2.y ARG3=dd_mo2.z
<b name="data/Ibuprofen_Overprediction/plumed_mo.datdp_mat_mo2" onclick='showPath("data/Ibuprofen_Overprediction/plumed_mo.dat","data/Ibuprofen_Overprediction/plumed_mo.datdp_mat_mo2","data/Ibuprofen_Overprediction/plumed_mo.datdp_mat_mo2","brown")'>dp_mat_mo2</b>: <span class="plumedtooltip" style="color:green">DOTPRODUCT_MATRIX<span class="right">This action is not part of PLUMED and was included by using a LOAD command <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_a_d.html" style="color:green">More details</a><i></i></span></span> GROUP1=vv_mo2.x GROUP2=vv_mo2.y GROUP3=vv_mo2.z
<b name="data/Ibuprofen_Overprediction/plumed_mo.datang_mat_mo2" onclick='showPath("data/Ibuprofen_Overprediction/plumed_mo.dat","data/Ibuprofen_Overprediction/plumed_mo.datang_mat_mo2","data/Ibuprofen_Overprediction/plumed_mo.datang_mat_mo2","brown")'>ang_mat_mo2</b>: <span class="plumedtooltip" style="color:green">MATHEVAL<span class="right">An alias to the CUSTOM function that can also be used to calaculate combinations of variables using a custom expression. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html" style="color:green">More details</a><i></i></span></span> ARG1=dp_mat_mo2 <span class="plumedtooltip">FUNC<span class="right">the function you wish to evaluate<i></i></span></span>=acos(x) <span class="plumedtooltip">PERIODIC<span class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></span></span>=NO

<span style="color:blue" class="comment"># Plot Distribution</span>
<span style="display:none;" id="data/Ibuprofen_Overprediction/plumed_mo.datang_mat_mo2">The MATHEVAL action with label <b>ang_mat_mo2</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ang_mat_mo2.value</td><td>an arbitrary function</td></tr></table></span><b name="data/Ibuprofen_Overprediction/plumed_mo.datvalg_mo" onclick='showPath("data/Ibuprofen_Overprediction/plumed_mo.dat","data/Ibuprofen_Overprediction/plumed_mo.datvalg_mo","data/Ibuprofen_Overprediction/plumed_mo.datvalg_mo","brown")'>valg_mo</b>: <span class="plumedtooltip" style="color:green">KDE<span class="right">Create a histogram from the input scalar/vector/matrix using KDE <a href="https://www.plumed.org/doc-master/user-doc/html/_k_d_e.html" style="color:green">More details</a><i></i></span></span> ARG1=ang_mat_mo1 ARG2=<b name="data/Ibuprofen_Overprediction/plumed_mo.datang_mat_mo2">ang_mat_mo2</b>  <span class="plumedtooltip">GRID_MIN<span class="right"> the lower bounds for the grid<i></i></span></span>=0.000,0.000 <span class="plumedtooltip">GRID_MAX<span class="right"> the upper bounds for the grid<i></i></span></span>=3.142,3.142 <span class="plumedtooltip">GRID_BIN<span class="right">the number of bins for the grid<i></i></span></span>=37,37 <span class="plumedtooltip">BANDWIDTH<span class="right">the bandwidths for kernel density esimtation<i></i></span></span>=0.250,0.250 <span class="plumedtooltip">KERNEL<span class="right"> the kernel function you are using<i></i></span></span>=GAUSSIAN
<span style="display:none;" id="data/Ibuprofen_Overprediction/plumed_mo.datvalg_mo">The KDE action with label <b>valg_mo</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">valg_mo.value</td><td>a function on a grid that was obtained by doing a Kernel Density Estimation using the input arguments</td></tr></table></span><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=<b name="data/Ibuprofen_Overprediction/plumed_mo.datvalg_mo">valg_mo</b> <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=plumed_md_mo.dat
</pre>
{% endraw %}
