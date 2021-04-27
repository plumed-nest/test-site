**Project ID:** [plumID:19.017]({{ '/' | absolute_url }}eggs/19/017/)  
**Source:** plumed_metad/metad_24ang.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [raw zipped stdout](metad_24ang.dat.plumed.stdout.txt.zip) - [stderr](metad_24ang.dat.plumed.stderr)  
**Master:** [raw zipped stdout](metad_24ang.dat.plumed_master.stdout.txt.zip) - [stderr](metad_24ang.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=1-2593 ENTITY1=2594-2605
<a href="https://plumed.github.io/doc-master/user-doc/html/_f_i_t__t_o__t_e_m_p_l_a_t_e.html">FIT_TO_TEMPLATE</a> REFERENCE=../input/heavy_atoms.pdb TYPE=OPTIMAL

<span style="color:blue"># Group definition</span>
prot_noh: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> NDX_FILE=../input/index.ndx NDX_GROUP=Protein-H
sph: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> NDX_FILE=../input/index.ndx NDX_GROUP=sphere
bnz: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> NDX_FILE=../input/index.ndx NDX_GROUP=BNZ_noH

<a href="https://plumed.github.io/doc-master/user-doc/html/_w_r_a_p_a_r_o_u_n_d.html">WRAPAROUND</a> ATOMS=bnz AROUND=sph

sph_center: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=sph
bnz_center: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=bnz

sph_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_o_s_i_t_i_o_n.html">POSITION</a> ATOM=sph_center NOPBC
bnz_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_o_s_i_t_i_o_n.html">POSITION</a> ATOM=bnz_center NOPBC

abs_x: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=bnz_coord.x,sph_coord.x FUNC=x-y PERIODIC=NO
abs_y: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=bnz_coord.y,sph_coord.y FUNC=x-y PERIODIC=NO
abs_z: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=bnz_coord.z,sph_coord.z FUNC=x-y PERIODIC=NO

rho: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=abs_x,abs_y,abs_z FUNC=sqrt(x*x+y*y+z*z) PERIODIC=NO
theta: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=abs_z,rho FUNC=acos(x/y) PERIODIC=0.,pi
phi: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=abs_x,abs_y FUNC=atan2(y,x) PERIODIC=-pi,pi

<span style="color:blue"># Restraining potential of the sphere</span>
restr: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=rho AT=2.4 KAPPA=10000

<span style="color:blue"># Coordination number</span>
c: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=bnz GROUPB=prot_noh R_0=0.45

<span style="color:blue"># Metadynamics</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
ARG=rho,theta,phi
GRID_MIN=0,0.,-pi
GRID_MAX=2.8,pi,pi
SIGMA=0.1,pi/16.,pi/8.
HEIGHT=1.2
PACE=500
BIASFACTOR=20
TEMP=300.
LABEL=metad
CALC_RCT
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>


<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=rho FILE=distance.dat STRIDE=500
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=metad.* FILE=metad_data.dat STRIDE=500
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=restr.* FILE=sphere_restraint.dat STRIDE=500
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=abs_x,abs_y,abs_z FILE=xyz_coord.dat STRIDE=500
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=rho,theta,phi FILE=rtp_coord.dat STRIDE=500
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=c FILE=all_coordination_45.dat STRIDE=500

<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=500
</pre>{% endraw %}
