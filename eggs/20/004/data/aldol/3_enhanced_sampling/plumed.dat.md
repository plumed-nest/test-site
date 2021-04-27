**Project ID:** [plumID:20.004]({{ '/' | absolute_url }}eggs/20/004/)  
**Source:** aldol/3_enhanced_sampling/plumed.dat  
**Originally used with PLUMED version:** 2.5-dev  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>

<span style="color:blue">#UNITS</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> LENGTH=A  

<span style="color:blue">#LOAD FILES (or include them in PLUMED)</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_a_d.html">LOAD</a> FILE=../../code/PytorchModel.cpp
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_a_d.html">LOAD</a> FILE=Contacts.cpp

<span style="color:blue">#DEFINE GROUP OF ATOMS</span>
C: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=1,4,8
O: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6,11
H: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=2,3,5,7,9,10

<span style="color:blue">#DEFINE CONTACTS</span>
cc2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t_s.html">CONTACTS</a> GROUPA=C SWITCH={RATIONAL D_0=0.0 R_0=1.7 NN=6 MM=8} 
oo2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t_s.html">CONTACTS</a> GROUPA=O SWITCH={RATIONAL D_0=0.0 R_0=1.6 NN=6 MM=8} 
co2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t_s.html">CONTACTS</a> GROUPA=C GROUPB=O SWITCH={RATIONAL D_0=0.0 R_0=1.6 NN=6 MM=8} 
ch2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t_s.html">CONTACTS</a> GROUPA=C GROUPB=H SWITCH={RATIONAL D_0=0.0 R_0=1.2 NN=6 MM=8} 
oh2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t_s.html">CONTACTS</a> GROUPA=O GROUPB=H SWITCH={RATIONAL D_0=0.0 R_0=1.2 NN=6 MM=8} 

<span style="color:blue">#LOAD PYTHORCH MODEL</span>
auto: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_y_t_o_r_c_h__m_o_d_e_l.html">PYTORCH_MODEL</a> MODEL=../2_training_model/model.pt ARG=cc2.*,oo2.*,co2.*,ch2.*,oh2.*
NNcube: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=auto.node-0 FUNC=x+x^3 PERIODIC=NO

<span style="color:blue">#DEFINE WALLS WALLS</span>
com1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=1-7
com2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=8-11
dc1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=com1,com2 NOPBC
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=dc1  AT=+5.0 KAPPA=150.0 EXP=2 LABEL=uwall_1

nnuw: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=NNcube  AT=3.2 KAPPA=2000.0 EXP=2 
nnlw: <a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=NNcube  AT=-3.2 KAPPA=2000.0 EXP=2 

<span style="color:blue">#OPES CALCULATION</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_e_s__m_e_t_a_d.html">OPES_METAD</a> ...
  LABEL=opes
  ARG=NNcube
  PACE=500
  BARRIER=160
  SIGMA=0.10
  TEMP=300
... <a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_e_s__m_e_t_a_d.html">OPES_METAD</a>

<span style="color:blue">#MONITOR DISTANCES</span>
c1c8: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1,8 NOPBC
o6h7: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=6,7 NOPBC
o11h7: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=11,7 NOPBC

<span style="color:blue">#PRINT</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=20 FILE=COLVAR ARG=*
<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=1000
</pre>{% endraw %}
