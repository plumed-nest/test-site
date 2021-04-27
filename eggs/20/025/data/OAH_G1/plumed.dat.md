**Project ID:** [plumID:20.025]({{ '/' | absolute_url }}eggs/20/025/)  
**Source:** OAH_G1/plumed.dat  
**Originally used with PLUMED version:** 2.5-dev  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># --- (0) LOAD PYTORCH ---</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_a_d.html">LOAD</a> FILE=../code/PytorchModel.cpp

<span style="color:blue"># --- (1) ATOMS DEFINITIONS and ALIGNMENT ---</span>

HOST: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=16-199      <span style="color:blue">#host atoms</span>
LIGC: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=1-6  <span style="color:blue">#carbon atoms in the ligand</span>
l1: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=1             <span style="color:blue">#ligand selected atoms</span>
l2: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=3
l3: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=4
l4: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6
WO: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=209-6508:3    <span style="color:blue">#water oxygen atoms</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=HOST
<a href="https://plumed.github.io/doc-master/user-doc/html/_f_i_t__t_o__t_e_m_p_l_a_t_e.html">FIT_TO_TEMPLATE</a> STRIDE=1 REFERENCE=conf_template.pdb TYPE=OPTIMAL <span style="color:blue">#coordinates alignment</span>
lig: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=LIGC

v1: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_i_x_e_d_a_t_o_m.html">FIXEDATOM</a> AT=2.0136,2.0136,2.0   <span style="color:blue">#virtual atoms</span>
v2: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_i_x_e_d_a_t_o_m.html">FIXEDATOM</a> AT=2.0136,2.0136,2.25
v3: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_i_x_e_d_a_t_o_m.html">FIXEDATOM</a> AT=2.0136,2.0136,2.5
v4: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_i_x_e_d_a_t_o_m.html">FIXEDATOM</a> AT=2.0136,2.0136,2.75
v5: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_i_x_e_d_a_t_o_m.html">FIXEDATOM</a> AT=2.0136,2.0136,3.0
v6: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_i_x_e_d_a_t_o_m.html">FIXEDATOM</a> AT=2.0136,2.0136,3.25
v7: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_i_x_e_d_a_t_o_m.html">FIXEDATOM</a> AT=2.0136,2.0136,3.5
v8: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_i_x_e_d_a_t_o_m.html">FIXEDATOM</a> AT=2.0136,2.0136,3.75

cyl: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=v1,lig COMPONENTS
radius: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=cyl.x,cyl.y FUNC=sqrt(x*x+y*y) PERIODIC=NO

<span style="color:blue"># --- (2) DESCRIPTORS ---</span>

L1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=l1 GROUPB=WO SWITCH={RATIONAL D_0=0.0 R_0=0.25 NN=6 MM=10} NLIST NL_CUTOFF=1.0 NL_STRIDE=5
L2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=l2 GROUPB=WO SWITCH={RATIONAL D_0=0.0 R_0=0.25 NN=6 MM=10} NLIST NL_CUTOFF=1.0 NL_STRIDE=5
L3: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=l3 GROUPB=WO SWITCH={RATIONAL D_0=0.0 R_0=0.25 NN=6 MM=10} NLIST NL_CUTOFF=1.0 NL_STRIDE=5
L4: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=l4 GROUPB=WO SWITCH={RATIONAL D_0=0.0 R_0=0.25 NN=6 MM=10} NLIST NL_CUTOFF=1.0 NL_STRIDE=5
V1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=v1 GROUPB=WO SWITCH={RATIONAL D_0=0.0 R_0=0.25 NN=2 MM=6} NLIST NL_CUTOFF=1.0 NL_STRIDE=5
V2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=v2 GROUPB=WO SWITCH={RATIONAL D_0=0.0 R_0=0.25 NN=2 MM=6} NLIST NL_CUTOFF=1.0 NL_STRIDE=5
V3: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=v3 GROUPB=WO SWITCH={RATIONAL D_0=0.0 R_0=0.25 NN=2 MM=6} NLIST NL_CUTOFF=1.0 NL_STRIDE=5
V4: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=v4 GROUPB=WO SWITCH={RATIONAL D_0=0.0 R_0=0.25 NN=2 MM=6} NLIST NL_CUTOFF=1.0 NL_STRIDE=5
V5: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=v5 GROUPB=WO SWITCH={RATIONAL D_0=0.0 R_0=0.25 NN=2 MM=6} NLIST NL_CUTOFF=1.0 NL_STRIDE=5
V6: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=v6 GROUPB=WO SWITCH={RATIONAL D_0=0.0 R_0=0.25 NN=2 MM=6} NLIST NL_CUTOFF=1.0 NL_STRIDE=5
V7: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=v7 GROUPB=WO SWITCH={RATIONAL D_0=0.0 R_0=0.25 NN=2 MM=6} NLIST NL_CUTOFF=1.0 NL_STRIDE=5
V8: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=v8 GROUPB=WO SWITCH={RATIONAL D_0=0.0 R_0=0.25 NN=2 MM=6} NLIST NL_CUTOFF=1.0 NL_STRIDE=5

d1: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=L1 FUNC=(x/2.5)-1.0 PERIODIC=NO  <span style="color:blue">#normalized descriptors</span>
d2: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=L2 FUNC=(x/2.5)-1.0 PERIODIC=NO
d3: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=L3 FUNC=(x/2.5)-1.0 PERIODIC=NO
d4: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=L4 FUNC=(x/2.5)-1.0 PERIODIC=NO
d5: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=V1 FUNC=(x/2.8)-1.0 PERIODIC=NO
d6: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=V2 FUNC=(x/2.8)-1.0 PERIODIC=NO
d7: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=V3 FUNC=(x/2.8)-1.0 PERIODIC=NO
d8: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=V4 FUNC=(x/2.8)-1.0 PERIODIC=NO
d9: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=V5 FUNC=(x/2.8)-1.0 PERIODIC=NO
d10: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=V6 FUNC=(x/2.8)-1.0 PERIODIC=NO
d11: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=V7 FUNC=(x/2.8)-1.0 PERIODIC=NO
d12: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=V8 FUNC=(x/2.8)-1.0 PERIODIC=NO

<span style="color:blue"># --- (3) DEEP-LDA CV and other quantities ---</span>

s: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_y_t_o_r_c_h__m_o_d_e_l.html">PYTORCH_MODEL</a> MODEL=modelG1_OAH_a.pt ARG=d1,d2,d3,d4,d5,d6,d7,d8,d9,d10,d11,d12  <span style="color:blue">#NN output</span>
sw: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=s.node-0 FUNC=x+x^3 PERIODIC=NO   <span style="color:blue">#Deep-LDA CV</span>

funnel: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=radius,cyl.z VAR=r,z FUNC=(r+1.0*(-1.2+z))*step(-z+1.)+(r-0.2)*step(z-1.) PERIODIC=NO
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> AT=0 ARG=funnel KAPPA=2000.0 LABEL=funnelwall  <span style="color:blue">#funnel restraint</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> AT=1.8 ARG=cyl.z KAPPA=4000.0 EXP=2 LABEL=upper_wall  <span style="color:blue">#upper limit of cyl.z</span>

ang: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_n_g_l_e.html">ANGLE</a> ATOMS=v3,v5,8,6   <span style="color:blue">#angle of a ligand's axis with z</span>
cosang: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=ang FUNC=cos(x) PERIODIC=NO

ene: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a>

<span style="color:blue"># --- (4) OPES  ---</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_e_s__m_e_t_a_d.html">OPES_METAD</a> ...
   LABEL=opes
   ARG=cyl.z,sw
   FILE=Kernels.data
   PACE=500
   FILE=../Kernels.data
   RESTART=NO
   STATE_RFILE=../compressed_Kernels.data
   STATE_WFILE=../compressed_Kernels.data
   STATE_WSTRIDE=50000
   WALKERS_MPI
... <a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_e_s__m_e_t_a_d.html">OPES_METAD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=* STRIDE=250 FILE=COLVAR FMT=%8.4f

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
<span style="color:blue"></span>
<span style="color:blue"></span>
</pre>{% endraw %}
