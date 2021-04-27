**Project ID:** [plumID:19.028]({{ '/' | absolute_url }}eggs/19/028/)  
**Source:** Lysozyme/round13/plumed.13.2rc.1.dat  
**Originally used with PLUMED version:** 2.3  
**Stable:** [raw zipped stdout](plumed.13.2rc.1.dat.plumed.stdout.txt.zip) - [stderr](plumed.13.2rc.1.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.13.2rc.1.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.13.2rc.1.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a> 
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


<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> LABEL=rc1 ARG=d1,d2,d3,d4,d5,d6,d7,d8,hd12,hd23,hd34  POWERS=1,1,1,1,1,1,1,1,1,1,1 COEFFICIENTS=0.4930809380065504,0.5058593109729893,-0.4001714129673795,0.23349420293166986,0.030037136299780397,-0.40087790689897096,0.1229390189050703,0.23125338096805748,-0.20809724216770412,-0.11136820637118663,-0.02039729281248875 PERIODIC=NO


<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> LABEL=rc2 ARG=d1,d2,d3,d4,d5,d6,d7,d8,hd12,hd23,hd34  POWERS=1,1,1,1,1,1,1,1,1,1,1 COEFFICIENTS=0.6523791027969725,0.39843894153595616,-0.48531942572099923,-0.07917807317470106,0.039850626498912835,-0.3037437511783076,-0.15437382551345147,-0.22403060705263078,-0.03784938171906625,-0.007286355646016722,0.06699856312142945 PERIODIC=NO

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_m_i_t_t_o_r.html">COMMITTOR</a> ...
 ARG=d1
 STRIDE=200
 BASIN_LL1=2.0
 BASIN_UL1=3.6
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_m_i_t_t_o_r.html">COMMITTOR</a>


<a href="https://plumed.github.io/doc-master/user-doc/html/_e_x_t_e_r_n_a_l.html">EXTERNAL</a> ARG=rc1 FILE=static_bias.8.test.txt LABEL=external1


<a href="https://plumed.github.io/doc-master/user-doc/html/_e_x_t_e_r_n_a_l.html">EXTERNAL</a> ARG=rc2 FILE=static_bias.13.rc2.1.txt LABEL=external2


<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=d1,d2,d3,d4,d5,d6,d7,d8,hd12,hd23,hd34,rc1,rc2,external1.bias,external2.bias STRIDE=1 FILE=benzene_Lyso_T298_13
</pre>{% endraw %}
