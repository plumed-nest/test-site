**Project ID:** [plumID:19.033]({{ '/' | absolute_url }}eggs/19/033/)  
**Source:** pmd_plumednest/plumed.0.dat  
**Originally used with PLUMED version:** 2.3  
**Stable:** [raw zipped stdout](plumed.0.dat.plumed.stdout.txt.zip) - [stderr](plumed.0.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.0.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.0.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_a_d.html">LOAD</a> FILE=PathCV.cpp
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> LENGTH=A TIME=ps ENERGY=kcal/mol

<span style="color:blue">#original omega torsion angles </span>
ow1: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=17,19,21,31
ow2: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=31,33,35,45
ow3: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=45,47,49,59

<span style="color:blue">#shift</span>
cw: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html">CONSTANT</a> VALUE=pi

<span style="color:blue">#shifted omega torsion angles</span>
w1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=ow1,cw COEFFICIENTS=1.0,0.5 PERIODIC=-pi,pi
w2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=ow2,cw COEFFICIENTS=1.0,0.5 PERIODIC=-pi,pi
w3: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=ow3,cw COEFFICIENTS=1.0,0.5 PERIODIC=-pi,pi

<span style="color:blue">#non-periodic shifted omega torsion angles (for restraining)</span>
r1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=w1 COEFFICIENTS=1.0 PERIODIC=NO
r2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=w2 COEFFICIENTS=1.0 PERIODIC=NO
r3: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=w3 COEFFICIENTS=1.0 PERIODIC=NO

<span style="color:blue">#cosines of original omega torsion angles </span>
c1: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=17,19,21,31 COSINE
c2: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=31,33,35,45 COSINE
c3: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=45,47,49,59 COSINE

<span style="color:blue">#sum of cosines of original omega torsion angles</span>
W: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=c1,c2,c3 PERIODIC=NO

<span style="color:blue">#path-CV in the space of w1,w2,w3</span>
<span style="color:blue">#WALKERS_ID=${ID} must be changed for each walker, as well as the name of the plumed.${ID}.dat file</span>
pcv: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_a_t_h_c_v.html">PATHCV</a> ARG=w1,w2,w3 GENPATH=20,60,20,1.57,1.57,1.57,-1.57,-1.57,-1.57 FIXED=21,80 HALFLIFE=2000 PACE=500 STRIDE=500 WALKERS_RSTRIDE=500 WALKERS_ID=0 WALKERS_N=8 WALKERS_DIR=.

<span style="color:blue">#metadynamics on path progress parameter pcv.s</span>
metad: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=pcv.s SIGMA=0.05 HEIGHT=0.02 PACE=500 INTERVAL=-0.1,1.1 GRID_MIN=-1.0 GRID_MAX=2.0 WALKERS_MPI FILE=HILLS

<span style="color:blue">#tube potential to restrain all walkers near the path</span>
tube: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=pcv.z AT=0.0 KAPPA=50.0

<span style="color:blue">#walls to keep walkers near the relevant interval pcv.s=[0,1]</span>
lwall: <a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=pcv.s AT=-0.1 KAPPA=1000.0 EXP=2 EPS=1 OFFSET=0
uwall: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=pcv.s AT=1.1  KAPPA=1000.0 EXP=2 EPS=1 OFFSET=0

<span style="color:blue">#walls to avoid periodic crossings in the space of w1,w2,w3</span>
lwwall: <a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=r1,r2,r3 AT=-3.0,-3.0,-3.0 KAPPA=1000.0,1000.0,1000.0 EXP=2,2,2 EPS=1,1,1 OFFSET=0,0,0
uwwall: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=r1,r2,r3 AT=3.0,3.0,3.0 KAPPA=1000.0,1000.0,1000.0 EXP=2,2,2 EPS=1,1,1 OFFSET=0,0,0

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=*  STRIDE=50 FILE=COLVAR


</pre>{% endraw %}
