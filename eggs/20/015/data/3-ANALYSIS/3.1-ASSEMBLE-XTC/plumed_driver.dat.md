**Project ID:** [plumID:20.015]({{ '/' | absolute_url }}eggs/20/015/)  
**Source:** 3-ANALYSIS/3.1-ASSEMBLE-XTC/plumed_driver.dat  
**Originally used with PLUMED version:** 2.6-dev  
**Stable:** [zipped raw stdout](plumed_driver.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_driver.dat.plumed.stderr.txt.zip) - [stderr](plumed_driver.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed_driver.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_driver.dat.plumed_master.stderr.txt.zip) - [stderr](plumed_driver.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/3-ANALYSIS/3.1-ASSEMBLE-XTC/plumed_driver.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed_driver.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed_driver.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue"># include topology info</span>
<div class="tooltip" style="color:green">MOLINFO<div class="right">This command is used to provide information on the molecules that are present in your system. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_o_l_i_n_f_o.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">STRUCTURE<div class="right">a file in pdb format containing a reference structure<i></i></div></div>=../../0-TOPO/step5_charmm2gmx.pdb <div class="tooltip">WHOLE<div class="right"> The reference structure is whole, i<i></i></div></div>
<br/><span style="color:blue"># define all atoms</span>
<b name="data/3-ANALYSIS/3.1-ASSEMBLE-XTC/plumed_driver.datprot" onclick='showPath("data/3-ANALYSIS/3.1-ASSEMBLE-XTC/plumed_driver.dat","data/3-ANALYSIS/3.1-ASSEMBLE-XTC/plumed_driver.datprot")'>prot</b>: <div class="tooltip" style="color:green">GROUP<div class="right">Define a group of atoms so that a particular list of atoms can be referenced with a single label in definitions of CVs or virtual atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_g_r_o_u_p.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">NDX_FILE<div class="right">the name of index file (gromacs syntax)<i></i></div></div>=../../0-TOPO/index.ndx <div class="tooltip">NDX_GROUP<div class="right">the name of the group to be imported (gromacs syntax) - first group found is used by default<i></i></div></div>=PROT
<br/><span style="color:blue"># make protein whole</span>
<div class="tooltip" style="color:green">WHOLEMOLECULES<div class="right">This action is used to rebuild molecules that can become split by the periodic boundary conditions. <a href="https://www.plumed.org/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html" style="color:green">More details</a><i></i></div></div> ...
<div class="tooltip">ADDREFERENCE<div class="right"> Define the reference position of the first atom of each entity using a PDB file<i></i></div></div>
<div class="tooltip">EMST<div class="right"> Define atoms sequence in entities using an Euclidean minimum spanning tree<i></i></div></div>
<div class="tooltip">ENTITY0<div class="right">the atoms that make up a molecule that you wish to align<i></i></div></div>=1-6701
<div class="tooltip">ENTITY1<div class="right">the atoms that make up a molecule that you wish to align<i></i></div></div>=6702-6741
... WHOLEMOLECULES
<br/><span style="color:blue"># PRINT ATOM POSITIONS</span>
<div class="tooltip" style="color:green">DUMPATOMS<div class="right">Dump selected atoms on a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_d_u_m_p_a_t_o_m_s.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">STRIDE<div class="right"> the frequency with which the atoms should be output<i></i></div></div>=1 <div class="tooltip">FILE<div class="right">file on which to output coordinates; extension is automatically detected<i></i></div></div>=traj.gro <div class="tooltip">ATOMS<div class="right">the atom indices whose positions you would like to print out<i></i></div></div>=<b name="data/3-ANALYSIS/3.1-ASSEMBLE-XTC/plumed_driver.datprot">prot</b>
</pre>
{% endraw %}
