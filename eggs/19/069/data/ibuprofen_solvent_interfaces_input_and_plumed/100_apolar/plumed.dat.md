**Project ID:** [plumID:19.069]({{ '/' | absolute_url }}eggs/19/069/)  
**Source:** ibuprofen_solvent_interfaces_input_and_plumed/100_apolar/plumed.dat  
**Originally used with PLUMED version:** 2.3  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue">#center of mass of all bulk ibuprofen molecules using carbons on the benzene ring C4 - C9</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_i_n_c_l_u_d_e.html">INCLUDE</a> FILE=<a href="COM_bulk.dat.html">COM_bulk.dat</a>
<span style="color:blue"># celnter of mass of all solvent molecules</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_i_n_c_l_u_d_e.html">INCLUDE</a> FILE=<a href="COM_solvent.dat.html">COM_solvent.dat</a>
<span style="color:blue"># solvent group and pseudobulk groups</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_i_n_c_l_u_d_e.html">INCLUDE</a> FILE=<a href="groups.dat.html">groups.dat</a> 
<span style="color:blue"># defining distance e.g d1: DISTANCE ATOMS=s1,pseudobulk</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_i_n_c_l_u_d_e.html">INCLUDE</a> FILE=<a href="distance.dat.html">distance.dat</a>
<span style="color:blue">#printing all d.z </span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_i_n_c_l_u_d_e.html">INCLUDE</a> FILE=<a href="print.dat.html">print.dat</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
<span style="color:blue"></span>
</pre>{% endraw %}
