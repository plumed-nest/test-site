**Project ID:** [plumID:20.025]({{ '/' | absolute_url }}eggs/20/025/)  
**Source:** OAMe_alone/plumed.dat  
**Originally used with PLUMED version:** 2.5-dev  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># --- (0) LOAD PYTORCH ---</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_a_d.html">LOAD</a> FILE=../code/PytorchModel.cpp

<span style="color:blue"># --- (1) ATOMS DEFINITIONS and ALIGNMENT ---</span>

HOST: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=1-196      <span style="color:blue">#host atoms</span>
WO: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=205-6504:3    <span style="color:blue">#water oxygen atoms</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=HOST
<a href="https://plumed.github.io/doc-master/user-doc/html/_f_i_t__t_o__t_e_m_p_l_a_t_e.html">FIT_TO_TEMPLATE</a> STRIDE=1 REFERENCE=conf_template.pdb TYPE=OPTIMAL <span style="color:blue">#coordinates alignment</span>

v1: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_i_x_e_d_a_t_o_m.html">FIXEDATOM</a> AT=2.0136,2.0136,2.0   <span style="color:blue">#virtual atoms</span>
v2: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_i_x_e_d_a_t_o_m.html">FIXEDATOM</a> AT=2.0136,2.0136,2.25
v3: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_i_x_e_d_a_t_o_m.html">FIXEDATOM</a> AT=2.0136,2.0136,2.5
v4: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_i_x_e_d_a_t_o_m.html">FIXEDATOM</a> AT=2.0136,2.0136,2.75
v5: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_i_x_e_d_a_t_o_m.html">FIXEDATOM</a> AT=2.0136,2.0136,3.0
v6: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_i_x_e_d_a_t_o_m.html">FIXEDATOM</a> AT=2.0136,2.0136,3.25
v7: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_i_x_e_d_a_t_o_m.html">FIXEDATOM</a> AT=2.0136,2.0136,3.5
v8: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_i_x_e_d_a_t_o_m.html">FIXEDATOM</a> AT=2.0136,2.0136,3.75

<span style="color:blue"># --- (2) DESCRIPTORS ---</span>

<span style="color:blue">#V1: COORDINATION GROUPA=v1 GROUPB=WO SWITCH={RATIONAL D_0=0.0 R_0=0.25 NN=2 MM=6} NLIST NL_CUTOFF=1.0 NL_STRIDE=5</span>
V2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=v2 GROUPB=WO SWITCH={RATIONAL D_0=0.0 R_0=0.25 NN=2 MM=6} NLIST NL_CUTOFF=1.0 NL_STRIDE=5
<span style="color:blue">#V3: COORDINATION GROUPA=v3 GROUPB=WO SWITCH={RATIONAL D_0=0.0 R_0=0.25 NN=2 MM=6} NLIST NL_CUTOFF=1.0 NL_STRIDE=5</span>
<span style="color:blue">#V4: COORDINATION GROUPA=v4 GROUPB=WO SWITCH={RATIONAL D_0=0.0 R_0=0.25 NN=2 MM=6} NLIST NL_CUTOFF=1.0 NL_STRIDE=5</span>
<span style="color:blue">#V5: COORDINATION GROUPA=v5 GROUPB=WO SWITCH={RATIONAL D_0=0.0 R_0=0.25 NN=2 MM=6} NLIST NL_CUTOFF=1.0 NL_STRIDE=5</span>
<span style="color:blue">#V6: COORDINATION GROUPA=v6 GROUPB=WO SWITCH={RATIONAL D_0=0.0 R_0=0.25 NN=2 MM=6} NLIST NL_CUTOFF=1.0 NL_STRIDE=5</span>
<span style="color:blue">#V7: COORDINATION GROUPA=v7 GROUPB=WO SWITCH={RATIONAL D_0=0.0 R_0=0.25 NN=2 MM=6} NLIST NL_CUTOFF=1.0 NL_STRIDE=5</span>
<span style="color:blue">#V8: COORDINATION GROUPA=v8 GROUPB=WO SWITCH={RATIONAL D_0=0.0 R_0=0.25 NN=2 MM=6} NLIST NL_CUTOFF=1.0 NL_STRIDE=5</span>

<span style="color:blue"># --- (3) DEEP-LDA CV and other quantities ---</span>

ene: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a>

<span style="color:blue"># --- (4) OPES  ---</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_e_s__m_e_t_a_d.html">OPES_METAD</a> ...
   LABEL=opes
   ARG=V2
   FILE=Kernels.data
   PACE=5000000
   BARRIER=30
   RESTART=YES
   STATE_WFILE=compressed_Kernels.data
   STATE_RFILE=compressed_Kernels.data
   STATE_WSTRIDE=50000
   <span style="color:blue">#WALKERS_MPI</span>
... <a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_e_s__m_e_t_a_d.html">OPES_METAD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=* STRIDE=250 FILE=COLVAR FMT=%8.4f

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
<span style="color:blue"></span>
<span style="color:blue"></span>
</pre>{% endraw %}
