**Project ID:** [plumID:19.037]({{ '/' | absolute_url }}eggs/19/037/)  
**Source:** Walker_1/plumed.mtd.inp  
**Originally used with PLUMED version:** 2.3  
**Stable:** [raw zipped stdout](plumed.mtd.inp.plumed.stdout.txt.zip) - [stderr](plumed.mtd.inp.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.mtd.inp.plumed_master.stdout.txt.zip) - [stderr](plumed.mtd.inp.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>

<span style="color:blue"># Units</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> ENERGY=eV LENGTH=A TIME=ps

<span style="color:blue"># CV(s)</span>

d1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=9,52
d2: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=24,67

v1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=8,16 COMPONENTS
v2: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=21,16 COMPONENTS
v3: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=51,59 COMPONENTS
v4: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=64,59 COMPONENTS

fx: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=v1.y,v1.z,v2.y,v2.z VAR=ay,az,by,bz FUNC=ay*bz-az*by PERIODIC=-24.9215,24.9215
fy: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=v1.x,v1.z,v2.x,v2.z VAR=ax,az,bx,bz FUNC=az*bx-ax*bz PERIODIC=-24.9215,24.9215
fz: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=v1.x,v1.y,v2.x,v2.y VAR=ax,ay,bx,by FUNC=ax*by-ay*bx PERIODIC=-24.9215,24.9215

gx: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=v3.y,v3.z,v4.y,v4.z VAR=ay,az,by,bz FUNC=ay*bz-az*by PERIODIC=-24.9215,24.9215
gy: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=v3.x,v3.z,v4.x,v4.z VAR=ax,az,bx,bz FUNC=az*bx-ax*bz PERIODIC=-24.9215,24.9215
gz: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=v3.x,v3.y,v4.x,v4.y VAR=ax,ay,bx,by FUNC=ax*by-ay*bx PERIODIC=-24.9215,24.9215

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ...
LABEL=theta
ARG=fx,fy,fz,gx,gy,gz
VAR=ax,ay,az,bx,by,bz
FUNC=(ax*bx+ay*by+az*bz)/sqrt((ax*ax+ay*ay+az*az)*(bx*bx+by*by+bz*bz))
PERIODIC=-2,2
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a>

<span style="color:blue"># Walls</span>
uwall1: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=d1 AT=22.0 KAPPA=1000 EXP=2 EPS=1 OFFSET=0
uwall2: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=d2 AT=22.0 KAPPA=1000 EXP=2 EPS=1 OFFSET=0

<span style="color:blue"># Metadynamics</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
  LABEL=mtd
  ARG=d1,d2,theta
  SIGMA=0.2,0.2,0.05
  PACE=1000
  HEIGHT=0.026
  BIASFACTOR=5 TEMP=300
  WALKERS_DIR=../HILLS_DIR 
  WALKERS_RSTRIDE=500 
  WALKERS_N=2
  WALKERS_ID=1
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<span style="color:blue"># Print CV</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=d1,d2,theta,uwall1.bias,uwall2.bias FILE=COLVAR STRIDE=1
<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=1000
</pre>{% endraw %}
