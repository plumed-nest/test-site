**Project ID:** [plumID:19.034]({{ '/' | absolute_url }}eggs/19/034/)  
**Source:** ptcv_plumednest/plumed.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue">#RESTART</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_a_d.html">LOAD</a> FILE=Proton.cpp
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_a_d.html">LOAD</a> FILE=PathCV.cpp
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> LENGTH=A TIME=ps ENERGY=kcal/mol

<span style="color:blue"># definition of CVs</span>

c1: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_o_t_o_n.html">PROTON</a> ALLATOMS=1-192 NN=12 MM=24 GAMMA=8 NO=64 NH=128 R_0=1.30 OFFSET_DEFAULT=2.0 OFFSET_INDEX=1,2 OFFSET_VALUE=0,0 
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_a_t_o_m_s.html">DUMPATOMS</a> STRIDE=10 FILE=proton.xyz ATOMS=c1 

distance: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=c1,194

c: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=1,2 GROUPB=65-192 R_0=1.3 NN=14 MM=28 
d: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=1,2 GROUPB=3-64 R_0=2.5 NN=14 MM=28 

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_a_t_h_c_v.html">PATHCV</a> LABEL=pcv ARG=c,distance,d GENPATH=0,2,0,1,1,1,2,2,2  STRIDE=1000 PACE=1000 HALFLIFE=1000 OUTFILE=PATH1
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=c,distance,d,pcv.s STRIDE=1  FILE=colvar

<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=distance AT=6.0 KAPPA=20 LABEL=uwall
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=uwall.bias STRIDE=1000 FILE=uwall

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=pcv.s SIGMA=0.045 HEIGHT=0.05 PACE=100 LABEL=restraint
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=pcv.s,restraint.bias STRIDE=50  FILE=colvar.out
</pre>{% endraw %}
