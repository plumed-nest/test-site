**Project ID:** [plumID:19.028]({{ '/' | absolute_url }}eggs/19/028/)  
**Source:** Lysozyme/round9/plumed.9.2rc.dat  
**Originally used with PLUMED version:** 2.3  
**Stable:** [raw zipped stdout](plumed.9.2rc.dat.plumed.stdout.txt.zip) - [stderr](plumed.9.2rc.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.9.2rc.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.9.2rc.dat.plumed_master.stderr)  

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


<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> LABEL=rc1 ARG=d1,d2,d3,d4,d5,d6,d7,d8,hd12,hd23,hd34  POWERS=1,1,1,1,1,1,1,1,1,1,1 COEFFICIENTS=0.4930809380065504,0.5058593109729893,-0.4001714129673795,0.23349420293166986,0.030037136299780397,-0.40087790689897096,0.1229390189050703,0.23125338096805748,-0.20809724216770412,-0.11136820637118663,-0.02039729281248875 PERIODIC=NO


<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> LABEL=rc2 ARG=d1,d2,d3,d4,d5,d6,d7,d8,hd12,hd23,hd34  POWERS=1,1,1,1,1,1,1,1,1,1,1 COEFFICIENTS=0.47798774048355186,0.5938376978731852,-0.3911931737431559,-0.25477549844776715,-0.1867757539217771,-0.3460145457220869,0.01717439149939613,0.07070895480558717,-0.059124920936706925,-0.13513219665156984,-0.1388503646899041 PERIODIC=NO

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_x_t_e_r_n_a_l.html">EXTERNAL</a> ARG=rc1 FILE=static_bias.8.txt LABEL=external1

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_x_t_e_r_n_a_l.html">EXTERNAL</a> ARG=rc2 FILE=static_bias.9.rc2.txt LABEL=external2


<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=d1,d2,d3,d4,d5,d6,d7,d8,hd12,hd23,hd34,rc1,rc2,external1.bias,external2.bias STRIDE=1 FILE=benzene_Lyso_T298_9
</pre>{% endraw %}
