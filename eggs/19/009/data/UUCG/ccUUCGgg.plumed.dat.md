**Project ID:** [plumID:19.009]({{ '/' | absolute_url }}eggs/19/009/)  
**Source:** UUCG/ccUUCGgg.plumed.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [zipped raw stdout](ccUUCGgg.plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](ccUUCGgg.plumed.dat.plumed.stderr.txt.zip) - [stderr](ccUUCGgg.plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](ccUUCGgg.plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](ccUUCGgg.plumed.dat.plumed_master.stderr.txt.zip) - [stderr](ccUUCGgg.plumed.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/UUCG/ccUUCGgg.plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="ccUUCGgg.plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="ccUUCGgg.plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue"># RESTART</span>
<div class="tooltip" style="color:green">MOLINFO<div class="right">This command is used to provide information on the molecules that are present in your system. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">STRUCTURE<div class="right">a file in pdb format containing a reference structure<i></i></div></div>=UUCG_8_L.pdb
<div class="tooltip" style="color:green">WHOLEMOLECULES<div class="right">This action is used to rebuild molecules that can become split by the periodic boundary conditions. <a href="https://www.plumed.org/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ENTITY0<div class="right">the atoms that make up a molecule that you wish to align<i></i></div></div>=1-254
<br/><b name="data/UUCG/ccUUCGgg.plumed.date0" onclick='showPath("data/UUCG/ccUUCGgg.plumed.dat","data/UUCG/ccUUCGgg.plumed.date0")'>e0</b>: <div class="tooltip" style="color:green">ERMSD<div class="right">Calculate eRMSD with respect to a reference structure. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_r_m_s_d.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the list of atoms (use lcs)<i></i></div></div>=<div class="tooltip">@lcs-1<div class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 1. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></div></div>,<div class="tooltip">@lcs-2<div class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 2. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></div></div>,<div class="tooltip">@lcs-3<div class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 3. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></div></div>,<div class="tooltip">@lcs-4<div class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 4. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></div></div>,<div class="tooltip">@lcs-5<div class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 5. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></div></div>,<div class="tooltip">@lcs-6<div class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 6. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></div></div>,<div class="tooltip">@lcs-7<div class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 7. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></div></div>,<div class="tooltip">@lcs-8<div class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 8. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></div></div> <div class="tooltip">REFERENCE<div class="right">a file in pdb format containing the reference structure and the atoms involved in the CV<i></i></div></div>=UUCG_8_H.pdb
<span style="display:none;" id="data/UUCG/ccUUCGgg.plumed.date0">The ERMSD action with label <b>e0</b> calculates a scalar quantity</span><b name="data/UUCG/ccUUCGgg.plumed.date3" onclick='showPath("data/UUCG/ccUUCGgg.plumed.dat","data/UUCG/ccUUCGgg.plumed.date3")'>e3</b>: <div class="tooltip" style="color:green">ERMSD<div class="right">Calculate eRMSD with respect to a reference structure. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_r_m_s_d.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the list of atoms (use lcs)<i></i></div></div>=<div class="tooltip">@lcs-1<div class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 1. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></div></div>,<div class="tooltip">@lcs-2<div class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 2. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></div></div>,<div class="tooltip">@lcs-3<div class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 3. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></div></div>,<div class="tooltip">@lcs-4<div class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 4. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></div></div>,<div class="tooltip">@lcs-5<div class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 5. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></div></div>,<div class="tooltip">@lcs-6<div class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 6. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></div></div>,<div class="tooltip">@lcs-7<div class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 7. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></div></div>,<div class="tooltip">@lcs-8<div class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 8. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></div></div> <div class="tooltip">REFERENCE<div class="right">a file in pdb format containing the reference structure and the atoms involved in the CV<i></i></div></div>=UUCG_8_L.pdb
<br/><span style="display:none;" id="data/UUCG/ccUUCGgg.plumed.date3">The ERMSD action with label <b>e3</b> calculates a scalar quantity</span><b name="data/UUCG/ccUUCGgg.plumed.datee3" onclick='showPath("data/UUCG/ccUUCGgg.plumed.dat","data/UUCG/ccUUCGgg.plumed.datee3")'>ee3</b>: <div class="tooltip" style="color:green">ERMSD<div class="right">Calculate eRMSD with respect to a reference structure. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_r_m_s_d.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the list of atoms (use lcs)<i></i></div></div>=<div class="tooltip">@lcs-1<div class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 1. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></div></div>,<div class="tooltip">@lcs-2<div class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 2. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></div></div>,<div class="tooltip">@lcs-3<div class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 3. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></div></div>,<div class="tooltip">@lcs-4<div class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 4. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></div></div>,<div class="tooltip">@lcs-5<div class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 5. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></div></div>,<div class="tooltip">@lcs-6<div class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 6. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></div></div>,<div class="tooltip">@lcs-7<div class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 7. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></div></div>,<div class="tooltip">@lcs-8<div class="right">an ordered triplet of atoms on the 6-membered ring of the nucleobase in residue 8. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">Click here</a> for more information. <i></i></div></div> <div class="tooltip">REFERENCE<div class="right">a file in pdb format containing the reference structure and the atoms involved in the CV<i></i></div></div>=UUCG_8_L.pdb <div class="tooltip">CUTOFF<div class="right"> only pairs of atoms closer than CUTOFF are considered in the calculation<i></i></div></div>=3.2
<br/><span style="display:none;" id="data/UUCG/ccUUCGgg.plumed.datee3">The ERMSD action with label <b>ee3</b> calculates a scalar quantity</span><b name="data/UUCG/ccUUCGgg.plumed.datr0" onclick='showPath("data/UUCG/ccUUCGgg.plumed.dat","data/UUCG/ccUUCGgg.plumed.datr0")'>r0</b>: <div class="tooltip" style="color:green">RMSD<div class="right">Calculate the RMSD with respect to a reference structure. <a href="https://www.plumed.org/doc-master/user-doc/html/_r_m_s_d.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">REFERENCE<div class="right">a file in pdb format containing the reference structure and the atoms involved in the CV<i></i></div></div>=UUCG_8_H.pdb <div class="tooltip">TYPE<div class="right"> the manner in which RMSD alignment is performed<i></i></div></div>=OPTIMAL
<span style="display:none;" id="data/UUCG/ccUUCGgg.plumed.datr0">The RMSD action with label <b>r0</b> calculates a scalar quantity</span><b name="data/UUCG/ccUUCGgg.plumed.datr3" onclick='showPath("data/UUCG/ccUUCGgg.plumed.dat","data/UUCG/ccUUCGgg.plumed.datr3")'>r3</b>: <div class="tooltip" style="color:green">RMSD<div class="right">Calculate the RMSD with respect to a reference structure. <a href="https://www.plumed.org/doc-master/user-doc/html/_r_m_s_d.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">REFERENCE<div class="right">a file in pdb format containing the reference structure and the atoms involved in the CV<i></i></div></div>=UUCG_8_L.pdb <div class="tooltip">TYPE<div class="right"> the manner in which RMSD alignment is performed<i></i></div></div>=OPTIMAL

<br/><span style="display:none;" id="data/UUCG/ccUUCGgg.plumed.datr3">The RMSD action with label <b>r3</b> calculates a scalar quantity</span><b name="data/UUCG/ccUUCGgg.plumed.datmetad" onclick='showPath("data/UUCG/ccUUCGgg.plumed.dat","data/UUCG/ccUUCGgg.plumed.datmetad")'>metad</b>: <div class="tooltip" style="color:green">METAD<div class="right">Used to performed metadynamics on one or more collective variables. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_e_t_a_d.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/UUCG/ccUUCGgg.plumed.datee3">ee3</b> <div class="tooltip">PACE<div class="right">the frequency for hill addition<i></i></div></div>=500000001 <div class="tooltip">HEIGHT<div class="right">the heights of the Gaussian hills<i></i></div></div>=0.0 <div class="tooltip">SIGMA<div class="right">the widths of the Gaussian hills<i></i></div></div>=0.1 <div class="tooltip">FILE<div class="right"> a file in which the list of added hills is stored<i></i></div></div>=HILLS_avg_5 <div class="tooltip">TEMP<div class="right">the system temperature - this is only needed if you are doing well-tempered metadynamics<i></i></div></div>=300.882 <div class="tooltip">BIASFACTOR<div class="right">use well tempered metadynamics and use this bias factor<i></i></div></div>=15 <div class="tooltip">GRID_MIN<div class="right">the lower bounds for the grid<i></i></div></div>=0.0 <div class="tooltip">GRID_MAX<div class="right">the upper bounds for the grid<i></i></div></div>=5.0 <div class="tooltip">GRID_BIN<div class="right">the number of bins for the grid<i></i></div></div>=250
<br/><span style="display:none;" id="data/UUCG/ccUUCGgg.plumed.datmetad">The METAD action with label <b>metad</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">metad.bias</td><td>the instantaneous value of the bias potential</td></tr></table></span><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/UUCG/ccUUCGgg.plumed.date3">e3</b>,<b name="data/UUCG/ccUUCGgg.plumed.datee3">ee3</b>,<b name="data/UUCG/ccUUCGgg.plumed.date0">e0</b>,<b name="data/UUCG/ccUUCGgg.plumed.datr3">r3</b>,<b name="data/UUCG/ccUUCGgg.plumed.datr0">r0</b>,<b name="data/UUCG/ccUUCGgg.plumed.datmetad">metad.bias</b> <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=colvar_5 <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=1
<br/><div class="tooltip" style="color:green">ENDPLUMED<div class="right">Terminate plumed input. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html" style="color:green">More details</a><i></i></div></div><span style="color:blue">

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

ENDPLUMED
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
