**Project ID:** [plumID:20.031]({{ '/' | absolute_url }}eggs/20/031/)  
**Source:** nanoshuttle_simulations/m08/plumed.dat  
**Originally used with PLUMED version:** 2.7  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue">#m08</span>
<span style="color:blue">#RESTART</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> STRIDE=1 ENTITY0=1-3342 ENTITY1=3343-5783 ENTITY2=5784-8224 ENTITY3=8225-10665 ENTITY4=10666-13106 ENTITY5=13107-15547 ENTITY6=15548-17988 ENTITY7=17989-20429 ENTITY8=20430-22870 ENTITY9=22871-25311

c1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=2602,2600,2599,2605,2604
c2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=6223,6222,6221,6220,6219,6224
<span style="color:blue">#d1: DISTANCE ATOMS=c1,c2</span>

c3: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=2604,2605,2606,2608,2612,2610
c4: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=6216,6214,6213,6224,6219,6217
<span style="color:blue">#d2: DISTANCE ATOMS=c3,c4</span>

c5: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=2602,2600,2599,2605,2604
c6: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=14948,14950,14951,14953,14958,14947
<span style="color:blue">#d3: DISTANCE ATOMS=c5,c6</span>
<span style="color:blue">#</span>
c7: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=2604,2605,2606,2608,2612,2610
c8: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=14958,14953,14954,14955,14956,14957
<span style="color:blue">#d1: DISTANCE ATOMS=c7,c8</span>


t1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=1182,1183,1183,1182,2654,2654,1588,1527,2056,1182,1183,1183,1182,2654,2654,1588,1527,2056 GROUPB=6213,6213,6215,6215,6216,6218,6218,6218,6220,14947,14947,14949,14949,14950,14952,14952,14952,14954 R_0=0.50 PAIR
t3: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=c1,c3,c5,c7  GROUPB=c2,c4,c6,c8 R_0=0.60 PAIR

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_b_m_e_t_a_d.html">PBMETAD</a> ...
LABEL=pb ARG=t1,t3 SIGMA=0.35,0.35 HEIGHT=1.2 PACE=500 FILE=HILLS_t1,HILLS_t3 BIASFACTOR=25 TEMP=300
WALKERS_N=6
WALKERS_ID=0
WALKERS_DIR=../
WALKERS_RSTRIDE=500
... <a href="https://plumed.github.io/doc-master/user-doc/html/_p_b_m_e_t_a_d.html">PBMETAD</a>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=t1,t3,pb.bias  STRIDE=500   FILE=COLVAR
</pre>{% endraw %}
