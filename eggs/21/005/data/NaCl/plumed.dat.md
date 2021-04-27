**Project ID:** [plumID:21.005]({{ '/' | absolute_url }}eggs/21/005/)  
**Source:** NaCl/plumed.dat  
**Originally used with PLUMED version:** 2.7-mod  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_a_d.html">LOAD</a> FILE=../codes/StructureFactor_descriptor.test.cpp
<span style="color:blue">#RESTART</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=1-108 LABEL=na
<a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=109-216 LABEL=cl
<a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=1-216 LABEL=nacl


s1: <a href="https://plumed.github.io/doc-master/user-doc/html/_s_t_r_u_c_t_u_r_e__f_a_c_t_o_r__d_e_s_c_r_i_p_t_o_r__t_e_s_t.html">STRUCTURE_FACTOR_DESCRIPTOR_TEST</a> ACTIVE_SHELLS=27,36,72,99 ATOMS=na
s2: <a href="https://plumed.github.io/doc-master/user-doc/html/_s_t_r_u_c_t_u_r_e__f_a_c_t_o_r__d_e_s_c_r_i_p_t_o_r__t_e_s_t.html">STRUCTURE_FACTOR_DESCRIPTOR_TEST</a> ACTIVE_SHELLS=27,36,72,99 ATOMS=cl

auto1: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_y_t_o_r_c_h__m_o_d_e_l.html">PYTORCH_MODEL</a> MODEL=nacl_sfNa_ct1.pt ARG=s1.Sk3_-3_-3,s1.Sk3_-3_3,s1.Sk3_3_-3,s1.Sk3_3_3,s1.Sk6_0_0,s1.Sk0_6_-6,s1.Sk0_6_6,s1.Sk6_-6_0,s1.Sk6_0_-6,s1.Sk6_0_6,s1.Sk6_6_0,s1.Sk9_-3_-3,s1.Sk9_-3_3,s1.Sk9_3_-3,s1.Sk9_3_3
NNcube1: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=auto1.node-0 FUNC=x+x^3 PERIODIC=NO

auto2: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_y_t_o_r_c_h__m_o_d_e_l.html">PYTORCH_MODEL</a> MODEL=nacl_sfCl_ct1.pt ARG=s2.Sk3_-3_-3,s2.Sk3_-3_3,s2.Sk3_3_-3,s2.Sk3_3_3,s2.Sk6_0_0,s2.Sk0_6_-6,s2.Sk0_6_6,s2.Sk6_-6_0,s2.Sk6_0_-6,s2.Sk6_0_6,s2.Sk6_6_0,s1.Sk9_-3_-3,s2.Sk9_-3_3,s2.Sk9_3_-3,s2.Sk9_3_3
NNcube2: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=auto2.node-0 FUNC=x+x^3 PERIODIC=NO

s12: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=NNcube1,NNcube2 FUNC=0.5*(x+y) PERIODIC=NO


<a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_e_s__m_e_t_a_d.html">OPES_METAD</a> ...
  LABEL=opes
  ARG=s12
  PACE=1000
  BARRIER=600
  FILE=Kernels.data
  STATE_RFILE=compressed_KernelsR.data
  STATE_WFILE=compressed_KernelsW.data
  STATE_WSTRIDE=5000 
...

uwall1: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=NNcube1 AT=2.9 KAPPA=5000
lwall1: <a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=NNcube1 AT=-2.9 KAPPA=5000

<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=500
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=500 FILE=COLVAR-na ARG=s1.Sk3_-3_-3,s1.Sk3_-3_3,s1.Sk3_3_-3,s1.Sk3_3_3,s1.Sk6_0_0,s1.Sk0_6_-6,s1.Sk0_6_6,s1.Sk6_-6_0,s1.Sk6_0_-6,s1.Sk6_0_6,s1.Sk6_6_0,s1.Sk9_-3_-3,s1.Sk9_-3_3,s1.Sk9_3_-3,s1.Sk9_3_3 
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=500 FILE=COLVAR-cl ARG=s2.Sk3_-3_-3,s2.Sk3_-3_3,s2.Sk3_3_-3,s2.Sk3_3_3,s2.Sk6_0_0,s2.Sk0_6_-6,s2.Sk0_6_6,s2.Sk6_-6_0,s2.Sk6_0_-6,s2.Sk6_0_6,s2.Sk6_6_0,s1.Sk9_-3_-3,s2.Sk9_-3_3,s2.Sk9_3_-3,s2.Sk9_3_3
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FMT=%g STRIDE=500 FILE=COLVAR-nn ARG=NNcube1,NNcube2
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FMT=%g STRIDE=500 FILE=COLVAR ARG=s12,opes.*,uwall1.*,lwall1.*

</pre>{% endraw %}
