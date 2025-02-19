**Project ID:** [plumID:19.009]({{ '/' | absolute_url }}eggs/19/009/)  
**Source:** GAGA/ccGAGAgg.plumed.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [zipped raw stdout](ccGAGAgg.plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](ccGAGAgg.plumed.dat.plumed.stderr.txt.zip) - [stderr](ccGAGAgg.plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](ccGAGAgg.plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](ccGAGAgg.plumed.dat.plumed_master.stderr.txt.zip) - [stderr](ccGAGAgg.plumed.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/GAGA/ccGAGAgg.plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="ccGAGAgg.plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-passing-green.svg" alt="tested onv2.10" /></a></td></tr><tr><td style="padding:1px"><a href="ccGAGAgg.plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue" class="comment"># RESTART</span>
<span class="plumedtooltip" style="color:green">MOLINFO<span class="right">This command is used to provide information on the molecules that are present in your system. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">STRUCTURE<span class="right">a file in pdb format containing a reference structure<i></i></span></span>=GAGA_8_H.pdb
<span style="display:none;" id="data/GAGA/ccGAGAgg.plumed.dat">The MOLINFO action with label <b></b> calculates something</span><span class="plumedtooltip" style="color:green">WHOLEMOLECULES<span class="right">This action is used to rebuild molecules that can become split by the periodic boundary conditions. <a href="https://www.plumed.org/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ENTITY0<span class="right">the atoms that make up a molecule that you wish to align<i></i></span></span>=1-263

<span id="data/GAGA/ccGAGAgg.plumed.datdefe0_short"><b name="data/GAGA/ccGAGAgg.plumed.date0" onclick='showPath("data/GAGA/ccGAGAgg.plumed.dat","data/GAGA/ccGAGAgg.plumed.date0","data/GAGA/ccGAGAgg.plumed.date0","black")'>e0</b><span style="display:none;" id="data/GAGA/ccGAGAgg.plumed.date0">The ERMSD action with label <b>e0</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">e0</td><td width="5%"><font color="black">scalar</font></td><td>the eRMSD between the instantaneous structure and the reference structure that was input</td></tr></table></span>: <span class="plumedtooltip" style="color:green">ERMSD<span class="right">Calculate eRMSD with respect to a reference structure. This action has <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/GAGA/ccGAGAgg.plumed.datdefe0");'>hidden defaults</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_r_m_s_d.html">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS<span class="right">the list of atoms (use lcs)<i></i></span></span>=<span class="plumedtooltip">@lcs-1<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 1. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span>,<span class="plumedtooltip">@lcs-2<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 2. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span>,<span class="plumedtooltip">@lcs-3<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 3. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span>,<span class="plumedtooltip">@lcs-4<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 4. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span>,<span class="plumedtooltip">@lcs-5<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 5. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span>,<span class="plumedtooltip">@lcs-6<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 6. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span>,<span class="plumedtooltip">@lcs-7<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 7. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span>,<span class="plumedtooltip">@lcs-8<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 8. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span> <span class="plumedtooltip">REFERENCE<span class="right">a file in pdb format containing the reference structure and the atoms involved in the CV<i></i></span></span>=GAGA_8_H.pdb
</span><span id="data/GAGA/ccGAGAgg.plumed.datdefe0_long" style="display:none;"><b name="data/GAGA/ccGAGAgg.plumed.date0" onclick='showPath("data/GAGA/ccGAGAgg.plumed.dat","data/GAGA/ccGAGAgg.plumed.date0","data/GAGA/ccGAGAgg.plumed.date0","black")'>e0</b>: <span class="plumedtooltip" style="color:green">ERMSD<span class="right">Calculate eRMSD with respect to a reference structure. This action uses the <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/GAGA/ccGAGAgg.plumed.datdefe0");'>defaults shown here</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_r_m_s_d.html">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS<span class="right">the list of atoms (use lcs)<i></i></span></span>=<span class="plumedtooltip">@lcs-1<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 1. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span>,<span class="plumedtooltip">@lcs-2<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 2. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span>,<span class="plumedtooltip">@lcs-3<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 3. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span>,<span class="plumedtooltip">@lcs-4<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 4. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span>,<span class="plumedtooltip">@lcs-5<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 5. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span>,<span class="plumedtooltip">@lcs-6<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 6. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span>,<span class="plumedtooltip">@lcs-7<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 7. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span>,<span class="plumedtooltip">@lcs-8<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 8. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span> <span class="plumedtooltip">REFERENCE<span class="right">a file in pdb format containing the reference structure and the atoms involved in the CV<i></i></span></span>=GAGA_8_H.pdb  <span class="plumedtooltip">CUTOFF<span class="right"> only pairs of atoms closer than CUTOFF are considered in the calculation<i></i></span></span>=2.4
</span><span id="data/GAGA/ccGAGAgg.plumed.datdefe3_short"><b name="data/GAGA/ccGAGAgg.plumed.date3" onclick='showPath("data/GAGA/ccGAGAgg.plumed.dat","data/GAGA/ccGAGAgg.plumed.date3","data/GAGA/ccGAGAgg.plumed.date3","black")'>e3</b><span style="display:none;" id="data/GAGA/ccGAGAgg.plumed.date3">The ERMSD action with label <b>e3</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">e3</td><td width="5%"><font color="black">scalar</font></td><td>the eRMSD between the instantaneous structure and the reference structure that was input</td></tr></table></span>: <span class="plumedtooltip" style="color:green">ERMSD<span class="right">Calculate eRMSD with respect to a reference structure. This action has <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/GAGA/ccGAGAgg.plumed.datdefe3");'>hidden defaults</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_r_m_s_d.html">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS<span class="right">the list of atoms (use lcs)<i></i></span></span>=<span class="plumedtooltip">@lcs-1<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 1. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span>,<span class="plumedtooltip">@lcs-2<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 2. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span>,<span class="plumedtooltip">@lcs-3<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 3. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span>,<span class="plumedtooltip">@lcs-4<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 4. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span>,<span class="plumedtooltip">@lcs-5<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 5. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span>,<span class="plumedtooltip">@lcs-6<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 6. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span>,<span class="plumedtooltip">@lcs-7<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 7. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span>,<span class="plumedtooltip">@lcs-8<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 8. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span> <span class="plumedtooltip">REFERENCE<span class="right">a file in pdb format containing the reference structure and the atoms involved in the CV<i></i></span></span>=GAGA_8_L.pdb
</span><span id="data/GAGA/ccGAGAgg.plumed.datdefe3_long" style="display:none;"><b name="data/GAGA/ccGAGAgg.plumed.date3" onclick='showPath("data/GAGA/ccGAGAgg.plumed.dat","data/GAGA/ccGAGAgg.plumed.date3","data/GAGA/ccGAGAgg.plumed.date3","black")'>e3</b>: <span class="plumedtooltip" style="color:green">ERMSD<span class="right">Calculate eRMSD with respect to a reference structure. This action uses the <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/GAGA/ccGAGAgg.plumed.datdefe3");'>defaults shown here</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_r_m_s_d.html">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS<span class="right">the list of atoms (use lcs)<i></i></span></span>=<span class="plumedtooltip">@lcs-1<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 1. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span>,<span class="plumedtooltip">@lcs-2<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 2. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span>,<span class="plumedtooltip">@lcs-3<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 3. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span>,<span class="plumedtooltip">@lcs-4<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 4. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span>,<span class="plumedtooltip">@lcs-5<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 5. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span>,<span class="plumedtooltip">@lcs-6<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 6. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span>,<span class="plumedtooltip">@lcs-7<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 7. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span>,<span class="plumedtooltip">@lcs-8<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 8. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span> <span class="plumedtooltip">REFERENCE<span class="right">a file in pdb format containing the reference structure and the atoms involved in the CV<i></i></span></span>=GAGA_8_L.pdb  <span class="plumedtooltip">CUTOFF<span class="right"> only pairs of atoms closer than CUTOFF are considered in the calculation<i></i></span></span>=2.4
</span><br/><b name="data/GAGA/ccGAGAgg.plumed.datee3" onclick='showPath("data/GAGA/ccGAGAgg.plumed.dat","data/GAGA/ccGAGAgg.plumed.datee3","data/GAGA/ccGAGAgg.plumed.datee3","black")'>ee3</b><span style="display:none;" id="data/GAGA/ccGAGAgg.plumed.datee3">The ERMSD action with label <b>ee3</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ee3</td><td width="5%"><font color="black">scalar</font></td><td>the eRMSD between the instantaneous structure and the reference structure that was input</td></tr></table></span>: <span class="plumedtooltip" style="color:green">ERMSD<span class="right">Calculate eRMSD with respect to a reference structure. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_r_m_s_d.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS<span class="right">the list of atoms (use lcs)<i></i></span></span>=<span class="plumedtooltip">@lcs-1<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 1. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span>,<span class="plumedtooltip">@lcs-2<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 2. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span>,<span class="plumedtooltip">@lcs-3<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 3. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span>,<span class="plumedtooltip">@lcs-4<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 4. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span>,<span class="plumedtooltip">@lcs-5<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 5. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span>,<span class="plumedtooltip">@lcs-6<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 6. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span>,<span class="plumedtooltip">@lcs-7<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 7. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span>,<span class="plumedtooltip">@lcs-8<span class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 8. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></span></span> <span class="plumedtooltip">REFERENCE<span class="right">a file in pdb format containing the reference structure and the atoms involved in the CV<i></i></span></span>=GAGA_8_L.pdb <span class="plumedtooltip">CUTOFF<span class="right"> only pairs of atoms closer than CUTOFF are considered in the calculation<i></i></span></span>=3.2

<span id="data/GAGA/ccGAGAgg.plumed.datdefr0_short"><b name="data/GAGA/ccGAGAgg.plumed.datr0" onclick='showPath("data/GAGA/ccGAGAgg.plumed.dat","data/GAGA/ccGAGAgg.plumed.datr0","data/GAGA/ccGAGAgg.plumed.datr0","black")'>r0</b><span style="display:none;" id="data/GAGA/ccGAGAgg.plumed.datr0">The RMSD action with label <b>r0</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">r0</td><td width="5%"><font color="black">scalar</font></td><td>the RMSD between the instantaneous structure and the reference structure that was input</td></tr></table></span>: <span class="plumedtooltip" style="color:green">RMSD<span class="right">Calculate the RMSD with respect to a reference structure. This action has <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/GAGA/ccGAGAgg.plumed.datdefr0");'>hidden defaults</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_r_m_s_d.html">More details</a><i></i></span></span> <span class="plumedtooltip">REFERENCE<span class="right">a file in pdb format containing the reference structure and the atoms involved in the CV<i></i></span></span>=GAGA_8_H.pdb <span class="plumedtooltip">TYPE<span class="right"> the manner in which RMSD alignment is performed<i></i></span></span>=OPTIMAL
</span><span id="data/GAGA/ccGAGAgg.plumed.datdefr0_long" style="display:none;"><b name="data/GAGA/ccGAGAgg.plumed.datr0" onclick='showPath("data/GAGA/ccGAGAgg.plumed.dat","data/GAGA/ccGAGAgg.plumed.datr0","data/GAGA/ccGAGAgg.plumed.datr0","black")'>r0</b>: <span class="plumedtooltip" style="color:green">RMSD<span class="right">Calculate the RMSD with respect to a reference structure. This action uses the <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/GAGA/ccGAGAgg.plumed.datdefr0");'>defaults shown here</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_r_m_s_d.html">More details</a><i></i></span></span> <span class="plumedtooltip">REFERENCE<span class="right">a file in pdb format containing the reference structure and the atoms involved in the CV<i></i></span></span>=GAGA_8_H.pdb <span class="plumedtooltip">TYPE<span class="right"> the manner in which RMSD alignment is performed<i></i></span></span>=OPTIMAL  <span class="plumedtooltip">NUMBER<span class="right"> if there are multiple structures in the pdb file you can specify that you want the RMSD from a specific structure by specifying its place in the file here<i></i></span></span>=0
</span><span id="data/GAGA/ccGAGAgg.plumed.datdefr3_short"><b name="data/GAGA/ccGAGAgg.plumed.datr3" onclick='showPath("data/GAGA/ccGAGAgg.plumed.dat","data/GAGA/ccGAGAgg.plumed.datr3","data/GAGA/ccGAGAgg.plumed.datr3","black")'>r3</b><span style="display:none;" id="data/GAGA/ccGAGAgg.plumed.datr3">The RMSD action with label <b>r3</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">r3</td><td width="5%"><font color="black">scalar</font></td><td>the RMSD between the instantaneous structure and the reference structure that was input</td></tr></table></span>: <span class="plumedtooltip" style="color:green">RMSD<span class="right">Calculate the RMSD with respect to a reference structure. This action has <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/GAGA/ccGAGAgg.plumed.datdefr3");'>hidden defaults</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_r_m_s_d.html">More details</a><i></i></span></span> <span class="plumedtooltip">REFERENCE<span class="right">a file in pdb format containing the reference structure and the atoms involved in the CV<i></i></span></span>=GAGA_8_L.pdb <span class="plumedtooltip">TYPE<span class="right"> the manner in which RMSD alignment is performed<i></i></span></span>=OPTIMAL
</span><span id="data/GAGA/ccGAGAgg.plumed.datdefr3_long" style="display:none;"><b name="data/GAGA/ccGAGAgg.plumed.datr3" onclick='showPath("data/GAGA/ccGAGAgg.plumed.dat","data/GAGA/ccGAGAgg.plumed.datr3","data/GAGA/ccGAGAgg.plumed.datr3","black")'>r3</b>: <span class="plumedtooltip" style="color:green">RMSD<span class="right">Calculate the RMSD with respect to a reference structure. This action uses the <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/GAGA/ccGAGAgg.plumed.datdefr3");'>defaults shown here</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_r_m_s_d.html">More details</a><i></i></span></span> <span class="plumedtooltip">REFERENCE<span class="right">a file in pdb format containing the reference structure and the atoms involved in the CV<i></i></span></span>=GAGA_8_L.pdb <span class="plumedtooltip">TYPE<span class="right"> the manner in which RMSD alignment is performed<i></i></span></span>=OPTIMAL  <span class="plumedtooltip">NUMBER<span class="right"> if there are multiple structures in the pdb file you can specify that you want the RMSD from a specific structure by specifying its place in the file here<i></i></span></span>=0
</span><br/><br/><b name="data/GAGA/ccGAGAgg.plumed.datmetad" onclick='showPath("data/GAGA/ccGAGAgg.plumed.dat","data/GAGA/ccGAGAgg.plumed.datmetad","data/GAGA/ccGAGAgg.plumed.datmetad","black")'>metad</b><span style="display:none;" id="data/GAGA/ccGAGAgg.plumed.datmetad">The METAD action with label <b>metad</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">metad.bias</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the bias potential</td></tr></table></span>: <span class="plumedtooltip" style="color:green">METAD<span class="right">Used to performed metadynamics on one or more collective variables. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_e_t_a_d.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the labels of the scalars on which the bias will act<i></i></span></span>=<b name="data/GAGA/ccGAGAgg.plumed.datee3">ee3</b> <span class="plumedtooltip">PACE<span class="right">the frequency for hill addition<i></i></span></span>=500000001 <span class="plumedtooltip">HEIGHT<span class="right">the heights of the Gaussian hills<i></i></span></span>=0.0 <span class="plumedtooltip">SIGMA<span class="right">the widths of the Gaussian hills<i></i></span></span>=0.1 <span class="plumedtooltip">FILE<span class="right"> a file in which the list of added hills is stored<i></i></span></span>=HILLS_avg_5 <span class="plumedtooltip">TEMP<span class="right">the system temperature - this is only needed if you are doing well-tempered metadynamics<i></i></span></span>=300.882 <span class="plumedtooltip">BIASFACTOR<span class="right">use well tempered metadynamics and use this bias factor<i></i></span></span>=15 <span class="plumedtooltip">GRID_MIN<span class="right">the lower bounds for the grid<i></i></span></span>=0.0 <span class="plumedtooltip">GRID_MAX<span class="right">the upper bounds for the grid<i></i></span></span>=5.0 <span class="plumedtooltip">GRID_BIN<span class="right">the number of bins for the grid<i></i></span></span>=250

<span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=<b name="data/GAGA/ccGAGAgg.plumed.date3">e3</b>,<b name="data/GAGA/ccGAGAgg.plumed.datee3">ee3</b>,<b name="data/GAGA/ccGAGAgg.plumed.date0">e0</b>,<b name="data/GAGA/ccGAGAgg.plumed.datr3">r3</b>,<b name="data/GAGA/ccGAGAgg.plumed.datr0">r0</b>,<b name="data/GAGA/ccGAGAgg.plumed.datmetad">metad.bias</b> <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=colvar_5 <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=1

<span class="plumedtooltip" style="color:green">ENDPLUMED<span class="right">Terminate plumed input. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html" style="color:green">More details</a><i></i></span></span><span style="color:blue" class="comment">

# histograms below are computed using PLUMED 2.3 syntax

HISTOGRAM ...
REWEIGHT_BIAS
ARG=e3
TEMP=300.882
USE_ALL_DATA
UNNORMALIZED
GRID_MIN=0
GRID_MAX=3
GRID_BIN=250
RESTART=NO
BANDWIDTH=0.0075
GRID_WFILE=fes_ermsd_5_0
UPDATE_FROM=200000
UPDATE_UNTIL=400000
... HISTOGRAM

HISTOGRAM ...
REWEIGHT_BIAS
ARG=e3
TEMP=300.882
USE_ALL_DATA
UNNORMALIZED
GRID_MIN=0
GRID_MAX=3
GRID_BIN=250
RESTART=NO
BANDWIDTH=0.0075
GRID_WFILE=fes_ermsd_5_1
UPDATE_FROM=400000
UPDATE_UNTIL=600000
... HISTOGRAM


HISTOGRAM ...
REWEIGHT_BIAS
ARG=e3
TEMP=300.882
USE_ALL_DATA
UNNORMALIZED
GRID_MIN=0
GRID_MAX=3
GRID_BIN=250
RESTART=NO
BANDWIDTH=0.0075
GRID_WFILE=fes_ermsd_5_2
UPDATE_FROM=600000
UPDATE_UNTIL=800000
... HISTOGRAM


HISTOGRAM ...
REWEIGHT_BIAS
ARG=e3
TEMP=300.882
USE_ALL_DATA
UNNORMALIZED
GRID_MIN=0
GRID_MAX=3
GRID_BIN=250
RESTART=NO
BANDWIDTH=0.0075
GRID_WFILE=fes_ermsd_5_3
UPDATE_FROM=800000
UPDATE_UNTIL=1000000
... HISTOGRAM

################################

HISTOGRAM ...
REWEIGHT_BIAS
ARG=r3
TEMP=300.882
USE_ALL_DATA
UNNORMALIZED
GRID_MIN=0
GRID_MAX=1
GRID_BIN=250
RESTART=NO
BANDWIDTH=0.0025
GRID_WFILE=fes_rmsd_5_0
UPDATE_FROM=0
UPDATE_UNTIL=250000
... HISTOGRAM

HISTOGRAM ...
REWEIGHT_BIAS
ARG=r3
TEMP=300.882
USE_ALL_DATA
UNNORMALIZED
GRID_MIN=0
GRID_MAX=1
GRID_BIN=250
RESTART=NO
BANDWIDTH=0.0025
GRID_WFILE=fes_rmsd_5_1
UPDATE_FROM=250000
UPDATE_UNTIL=500000
... HISTOGRAM


HISTOGRAM ...
REWEIGHT_BIAS
ARG=r3
TEMP=300.882
USE_ALL_DATA
UNNORMALIZED
GRID_MIN=0
GRID_MAX=1
GRID_BIN=250
RESTART=NO
BANDWIDTH=0.0025
GRID_WFILE=fes_rmsd_5_2
UPDATE_FROM=500000
UPDATE_UNTIL=750000
... HISTOGRAM


HISTOGRAM ...
REWEIGHT_BIAS
ARG=r3
TEMP=300.882
USE_ALL_DATA
UNNORMALIZED
GRID_MIN=0
GRID_MAX=1
GRID_BIN=250
RESTART=NO
BANDWIDTH=0.0025
GRID_WFILE=fes_rmsd_5_3
UPDATE_FROM=750000
UPDATE_UNTIL=1000000
... HISTOGRAM
</span></pre>
{% endraw %}
