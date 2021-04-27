**Project ID:** [plumID:20.015]({{ '/' | absolute_url }}eggs/20/015/)  
**Source:** EMMI-ASCT2/3-ANALYSIS/3.1-ASSEMBLE-XTC/plumed_driver.dat  
**Originally used with PLUMED version:** 2.6-dev  
**Stable:** [raw zipped stdout](plumed_driver.dat.plumed.stdout.txt.zip) - [stderr](plumed_driver.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_driver.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_driver.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># include topology info</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">MOLINFO</a> STRUCTURE=../../0-TOPO/step5_charmm2gmx.pdb

<span style="color:blue"># define all atoms</span>
prot: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> NDX_FILE=../../0-TOPO/index.ndx NDX_GROUP=PROT

<span style="color:blue"># make protein whole</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ...
ADDREFERENCE 
ENTITY0=1-6701         REF0=5.3607,4.5911,3.1497
ENTITY1=6702-6741      REF1=3.2439,3.3684,6.0308
... <a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a>

<span style="color:blue"># PRINT ATOM POSITIONS</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_a_t_o_m_s.html">DUMPATOMS</a> STRIDE=1 FILE=traj.gro ATOMS=prot
</pre>{% endraw %}
