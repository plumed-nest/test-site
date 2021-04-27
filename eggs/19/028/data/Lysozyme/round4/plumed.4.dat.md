**Project ID:** [plumID:19.028]({{ '/' | absolute_url }}eggs/19/028/)  
**Source:** Lysozyme/round4/plumed.4.dat  
**Originally used with PLUMED version:** 2.3  
**Stable:** [raw zipped stdout](plumed.4.dat.plumed.stdout.txt.zip) - [stderr](plumed.4.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.4.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.4.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=1-2881


lig: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=2870,2872,2874


d1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=lig,1533
d2: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=lig,1716
d3: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=lig,2285
d4: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=lig,2005
d5: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=lig,1905
d6: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=lig,2239 
d7: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=lig,2424
d8: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=lig,2523

helix1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=1416,1428,1452,1475,1501,1513,1533,1554,1566
helix2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=1964,1980,1994,2005,2028,2052,2071,2094,2111
helix3: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=2176,2200,2212,2227,2239,2251,2271,2285,2308
helix4: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=2535,2559,2583,2603,2626,2642,2658,2678,2702

hd12: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=helix1,helix2
hd23: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=helix2,helix3
hd34: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=helix3,helix4


<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> LABEL=rc1 ARG=d1,d2,d3,d4,d5,d6,d7,d8,hd12,hd23,hd34  POWERS=1,1,1,1,1,1,1,1,1,1,1 COEFFICIENTS=0.12284315062731374,-0.21259161972480697,0.35112111438584803,-0.29373342211839154,0.1787051946254787,0.5632845789531697,-0.23123865376681804,-0.37903689621901265,-0.3125239692750005,-0.015943454312690033,0.2930157522372512 PERIODIC=NO






<a href="https://plumed.github.io/doc-master/user-doc/html/_e_x_t_e_r_n_a_l.html">EXTERNAL</a> ARG=rc1 FILE=static_bias.4.txt LABEL=external1


<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=d1,d2,d3,d4,d5,d6,d7,d8,hd12,hd23,hd34,rc1,external1.bias STRIDE=1 FILE=benzene_Lyso_T298_4
</pre>{% endraw %}
