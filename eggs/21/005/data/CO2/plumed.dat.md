**Project ID:** [plumID:21.005]({{ '/' | absolute_url }}eggs/21/005/)  
**Source:** CO2/plumed.dat  
**Originally used with PLUMED version:** 2.7-mod  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_a_d.html">LOAD</a> FILE=../codes/StructureFactor_descriptor.test.cpp
<span style="color:blue">#RESTART</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=1-324:3 LABEL=C
<a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=2-324:3,3-324:3 LABEL=O

so: <a href="https://plumed.github.io/doc-master/user-doc/html/_s_t_r_u_c_t_u_r_e__f_a_c_t_o_r__d_e_s_c_r_i_p_t_o_r__t_e_s_t.html">STRUCTURE_FACTOR_DESCRIPTOR_TEST</a> ACTIVE_SHELLS=27,45,54,117,126,144 ATOMS=O 

auto1: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_y_t_o_r_c_h__m_o_d_e_l.html">PYTORCH_MODEL</a> MODEL=co2_333_sfO_tc1.pt ARG=so.Sk3_-3_-3,so.Sk3_-3_3,so.Sk3_3_-3,so.Sk3_3_3,so.Sk0_3_-6,so.Sk0_3_6,so.Sk0_6_-3,so.Sk0_6_3,so.Sk3_-6_0,so.Sk3_0_-6,so.Sk3_0_6,so.Sk3_6_0,so.Sk6_-3_0,so.Sk6_0_-3,so.Sk6_0_3,so.Sk6_3_0,so.Sk3_-6_-3,so.Sk3_-6_3,so.Sk3_-3_-6,so.Sk3_-3_6,so.Sk3_3_-6,so.Sk3_3_6,so.Sk3_6_-3,so.Sk3_6_3,so.Sk6_-3_-3,so.Sk6_-3_3,so.Sk6_3_-3,so.Sk6_3_3,so.Sk0_6_-9,so.Sk0_6_9,so.Sk0_9_-6,so.Sk0_9_6,so.Sk6_-9_0,so.Sk6_0_-9,so.Sk6_0_9,so.Sk6_9_0,so.Sk9_-6_0,so.Sk9_0_-6,so.Sk9_0_6,so.Sk9_6_0,so.Sk3_-9_-6,so.Sk3_-9_6,so.Sk3_-6_-9,so.Sk3_-6_9,so.Sk3_6_-9,so.Sk3_6_9,so.Sk3_9_-6,so.Sk3_9_6,so.Sk6_-9_-3,so.Sk6_-9_3,so.Sk6_-3_-9,so.Sk6_-3_9,so.Sk6_3_-9,so.Sk6_3_9,so.Sk6_9_-3,so.Sk6_9_3,so.Sk9_-6_-3,so.Sk9_-6_3,so.Sk9_-3_-6,so.Sk9_-3_6,so.Sk9_3_-6,so.Sk9_3_6,so.Sk9_6_-3,so.Sk9_6_3,so.Sk0_0_12,so.Sk0_12_0,so.Sk12_0_0
NNcube1: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=auto1.node-0 FUNC=x+x^3 PERIODIC=NO

<a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_e_s__m_e_t_a_d.html">OPES_METAD</a> ...
  LABEL=opes
  ARG=NNcube1
  PACE=500
  BARRIER=200
  FILE=Kernels.data
  STATE_RFILE=compressed_KernelsR.data
  STATE_WFILE=compressed_KernelsW.data
  STATE_WSTRIDE=10000 
  NLIST
...


uwall: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=NNcube1 AT=2.9 KAPPA=10000
lwall: <a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=NNcube1 AT=-2.9 KAPPA=10000

<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=500
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FMT=%g STRIDE=500 FILE=COLVAR-comps ARG=so.Sk3_-3_-3,so.Sk3_-3_3,so.Sk3_3_-3,so.Sk3_3_3,so.Sk0_3_-6,so.Sk0_3_6,so.Sk0_6_-3,so.Sk0_6_3,so.Sk3_-6_0,so.Sk3_0_-6,so.Sk3_0_6,so.Sk3_6_0,so.Sk6_-3_0,so.Sk6_0_-3,so.Sk6_0_3,so.Sk6_3_0,so.Sk3_-6_-3,so.Sk3_-6_3,so.Sk3_-3_-6,so.Sk3_-3_6,so.Sk3_3_-6,so.Sk3_3_6,so.Sk3_6_-3,so.Sk3_6_3,so.Sk6_-3_-3,so.Sk6_-3_3,so.Sk6_3_-3,so.Sk6_3_3,so.Sk0_6_-9,so.Sk0_6_9,so.Sk0_9_-6,so.Sk0_9_6,so.Sk6_-9_0,so.Sk6_0_-9,so.Sk6_0_9,so.Sk6_9_0,so.Sk9_-6_0,so.Sk9_0_-6,so.Sk9_0_6,so.Sk9_6_0,so.Sk3_-9_-6,so.Sk3_-9_6,so.Sk3_-6_-9,so.Sk3_-6_9,so.Sk3_6_-9,so.Sk3_6_9,so.Sk3_9_-6,so.Sk3_9_6,so.Sk6_-9_-3,so.Sk6_-9_3,so.Sk6_-3_-9,so.Sk6_-3_9,so.Sk6_3_-9,so.Sk6_3_9,so.Sk6_9_-3,so.Sk6_9_3,so.Sk9_-6_-3,so.Sk9_-6_3,so.Sk9_-3_-6,so.Sk9_-3_6,so.Sk9_3_-6,so.Sk9_3_6,so.Sk9_6_-3,so.Sk9_6_3,so.Sk0_0_12,so.Sk0_12_0,so.Sk12_0_0
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FMT=%g STRIDE=500 FILE=COLVAR ARG=NNcube1,opes.*,uwall.*,lwall.*

</pre>{% endraw %}
