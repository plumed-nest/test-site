**Project ID:** [plumID:20.012]({{ '/' | absolute_url }}eggs/20/012/)  
**Source:** COMet_Path/cv_definitions.dat  
{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_a_d.html">LOAD</a> FILE=ProjectionOnAxis.cpp
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_a_d.html">LOAD</a> FILE=BridgeSimple.cpp

<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> STRIDE=1 ENTITY0=1-5120 ENTITY1=5121-5137

water_o: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=5138-74478:4
bs_noh: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=2390-2392,2489-2492,1842,1843
lig_noh: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=5121,5123,5129

<span style="color:blue">#bridge: BRIDGE_SIMPLE GROUPA=bs_noh GROUPB=lig_noh BRIDGING_ATOMS=water_o SWITCH={RATIONAL R_0=0.3 NN=8 MM=12 D_MAX=1.0} #NLIST NL_STRIDE=20 NL_CUTOFF=1.1</span>

lig: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=5121-5137		<span style="color:blue"># Ligand - 547 FRG</span>
p2_FS1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=3019,4303,4718	<span style="color:blue"># 196 SER@CA, 276 VAL@CA, 302 HIS(HIE)@CA</span>
p2_FS2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=2321,2160,4385,2411	<span style="color:blue"># 152 SER@CA, 141 ILE@CA, 281 MET@CA, 158 VAL@CA</span>
p1: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=3728			<span style="color:blue"># 243 TRP@CA</span>

pp: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_o_j_e_c_t_i_o_n__o_n__a_x_i_s.html">PROJECTION_ON_AXIS</a> AXIS_ATOMS=p1,p2_FS2 ATOM=lig

<span style="color:blue">#INCLUDE FILE=cmap_i0_m0_1.dat</span>
<span style="color:blue">#INCLUDE FILE=cmap_lp_m0_1.dat</span>
<span style="color:blue">#INCLUDE FILE=cmap_lx_m0_1.dat</span>

lig_1: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=5122
lig_2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=5126,5136

d1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=p1,lig_1
d2: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=p1,lig_2
d3: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=p2_FS2,lig_1
d4: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=p2_FS2,lig_2
</pre>{% endraw %}
