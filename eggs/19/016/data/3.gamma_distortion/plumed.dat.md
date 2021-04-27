**Project ID:** [plumID:19.016]({{ '/' | absolute_url }}eggs/19/016/)  
**Source:** 3.gamma_distortion/plumed.dat  
**Originally used with PLUMED version:** 2.3  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue">#RESTART</span>

ene: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a>
vol: <a href="https://plumed.github.io/doc-master/user-doc/html/_v_o_l_u_m_e.html">VOLUME</a>

cell: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_l_l.html">CELL</a>

aaa:    <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=cell.ax,cell.ay,cell.az POWERS=2,2,2 PERIODIC=NO
bbb:    <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=cell.bx,cell.by,cell.bz POWERS=2,2,2 PERIODIC=NO
ccc:    <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=cell.cx,cell.cy,cell.cz POWERS=2,2,2 PERIODIC=NO

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ...
ARG=cell.ax,cell.ay,cell.az,cell.bx,cell.by,cell.bz
VAR=ax,ay,az,bx,by,bz
FUNC=acos((ax*bx+ay*by+az*bz)/sqrt((ax*ax+ay*ay+az*az)*(bx*bx+by*by+bz*bz)))
PERIODIC=NO
LABEL=alpha
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ...
ARG=cell.ax,cell.ay,cell.az,cell.cx,cell.cy,cell.cz
VAR=ax,ay,az,bx,by,bz
FUNC=acos((ax*bx+ay*by+az*bz)/sqrt((ax*ax+ay*ay+az*az)*(bx*bx+by*by+bz*bz)))
PERIODIC=NO
LABEL=beta
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a>


<a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ...
ARG=cell.bx,cell.by,cell.bz,cell.cx,cell.cy,cell.cz
VAR=ax,ay,az,bx,by,bz
FUNC=acos((ax*bx+ay*by+az*bz)/sqrt((ax*ax+ay*ay+az*az)*(bx*bx+by*by+bz*bz)))
PERIODIC=NO
LABEL=gamma
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=alpha,beta,gamma AT=1.7,2.0,1.7 KAPPA=1000000,1000000,1000000 LABEL=uwall
<span style="color:blue">#LOWER_WALLS ARG=alpha,gamma AT=1.5,1.5 KAPPA=1000000,1000000  LABEL=lwall</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=alpha,beta,gamma AT=1.5,1.3,1.5 KAPPA=1000000,1000000,1000000 LABEL=lwall
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=beta SIGMA=0.005 HEIGHT=2.5 PACE=500 LABEL=metad TEMP=300 BIASFACTOR=150	 

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=alpha,beta,gamma,aaa,bbb,ccc,ene,vol,metad.bias STRIDE=100 FILE=COLVAR

</pre>{% endraw %}
