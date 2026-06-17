**Project ID:** [plumID:22.022]({{ '/' | absolute_url }}eggs/22/022/)  
**Source:** Arend_Grothaus_2022_PLUMED/plumed_rmsd_GSH+rito.dat  
**Originally used with PLUMED version:** 2.7  
**Stable:** [zipped raw stdout](plumed_rmsd_GSH+rito.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_rmsd_GSH+rito.dat.plumed.stderr.txt.zip) - [stderr](plumed_rmsd_GSH+rito.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed_rmsd_GSH+rito.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_rmsd_GSH+rito.dat.plumed_master.stderr.txt.zip) - [stderr](plumed_rmsd_GSH+rito.dat.plumed_master.stderr)  

{% raw %}
<div class="plumedInputContainer">
<div class="plumedpreheader">
<div class="headerInfo" id="value_details_data/Arend_Grothaus_2022_PLUMED/plumed_rmsd_GSH+rito.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div class="containerBadge">
<div class="headerBadge"><a href="plumed_rmsd_GSH+rito.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-passing-green.svg" alt="tested onv2.10" /></a></div>
<div class="headerBadge"><a href="plumed_rmsd_GSH+rito.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></div>
</div>
</div>
<pre class="plumedlisting">
<span style="color:blue" class="comment"># RMSD of GSH (+rito) with alignment on backbone of Mrp1</span>
<br/><span style="color:blue" class="comment"># for creation of a ref.pdb file, do the following to the occupancy and tempfactor column:</span>
<span style="color:blue" class="comment"># occupancy column (1st column after x,y,z): label atoms for alignment as 1, all others as 0 </span>
<span style="color:blue" class="comment"># tempfactor column (2nd column after x,y,z): label atoms for rmsd measurement as 1, all others as 0 </span>
<br/><b name="data/Arend_Grothaus_2022_PLUMED/plumed_rmsd_GSH+rito.datrmsd" onclick='showPath("data/Arend_Grothaus_2022_PLUMED/plumed_rmsd_GSH+rito.dat","data/Arend_Grothaus_2022_PLUMED/plumed_rmsd_GSH+rito.datrmsd","data/Arend_Grothaus_2022_PLUMED/plumed_rmsd_GSH+rito.datrmsd","brown")'>rmsd</b>: <span class="plumedtooltip" style="color:green">RMSD<span class="right">Calculate the RMSD with respect to a reference structure. <a href="https://www.plumed.org/doc-master/user-doc/html/RMSD" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">REFERENCE<span class="right">a file in pdb format containing the reference structure and the atoms involved in the CV<i></i></span></span>=ref_GSH+rito.pdb <span class="plumedtooltip">TYPE<span class="right"> the manner in which RMSD alignment is performed<i></i></span></span>=OPTIMAL

<span style="color:blue" class="comment"># Print the RMSD CV on COLVAR file every step</span>
<span style="display:none;" id="data/Arend_Grothaus_2022_PLUMED/plumed_rmsd_GSH+rito.datrmsd">The RMSD action with label <b>rmsd</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">rmsd.value</td><td>the RMSD distance between the instaneous structure and the reference structure/s that were input</td></tr></table></span><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/PRINT" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=<b name="data/Arend_Grothaus_2022_PLUMED/plumed_rmsd_GSH+rito.datrmsd">rmsd</b> <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=COLVAR_RMSD_GSH <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=1
</pre></div>

{% endraw %}
