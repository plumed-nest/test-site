**Project ID:** [plumID:22.022]({{ '/' | absolute_url }}eggs/22/022/)  
**Source:** Arend_Grothaus_2022_PLUMED/plumed_rmsd_GSH.dat  
**Originally used with PLUMED version:** 2.7  
**Stable:** [zipped raw stdout](plumed_rmsd_GSH.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_rmsd_GSH.dat.plumed.stderr.txt.zip) - [stderr](plumed_rmsd_GSH.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed_rmsd_GSH.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_rmsd_GSH.dat.plumed_master.stderr.txt.zip) - [stderr](plumed_rmsd_GSH.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/Arend_Grothaus_2022_PLUMED/plumed_rmsd_GSH.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed_rmsd_GSH.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed_rmsd_GSH.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue"># RMSD of GSH with alignment on backbone of Mrp1</span>
<b name="data/Arend_Grothaus_2022_PLUMED/plumed_rmsd_GSH.datrmsd" onclick='showPath("data/Arend_Grothaus_2022_PLUMED/plumed_rmsd_GSH.dat","data/Arend_Grothaus_2022_PLUMED/plumed_rmsd_GSH.datrmsd")'>rmsd</b>: <div class="tooltip" style="color:green">RMSD<div class="right">Calculate the RMSD with respect to a reference structure. <a href="https://www.plumed.org/doc-master/user-doc/html/_r_m_s_d.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">REFERENCE<div class="right">a file in pdb format containing the reference structure and the atoms involved in the CV<i></i></div></div>=ref-GSH.pdb <div class="tooltip">TYPE<div class="right"> the manner in which RMSD alignment is performed<i></i></div></div>=OPTIMAL
<br/><span style="color:blue"># Print the RMSD CV on COLVAR file every step</span>
<span style="display:none;" id="data/Arend_Grothaus_2022_PLUMED/plumed_rmsd_GSH.datrmsd">The RMSD action with label <b>rmsd</b> calculates a scalar quantity</span><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/Arend_Grothaus_2022_PLUMED/plumed_rmsd_GSH.datrmsd">rmsd</b> <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=COLVAR_RMSD_GSH <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=1
</pre>
{% endraw %}
