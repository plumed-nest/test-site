**Project ID:** [plumID:19.048]({{ '/' | absolute_url }}eggs/19/048/)  
**Source:** A2a_LUF.dat  
**Originally used with PLUMED version:** 2.3.1  
**Stable:** [raw zipped stdout](A2a_LUF.dat.plumed.stdout.txt.zip) - [stderr](A2a_LUF.dat.plumed.stderr)  
**Master:** [raw zipped stdout](A2a_LUF.dat.plumed_master.stdout.txt.zip) - [stderr](A2a_LUF.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a> 
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> STRIDE=1000 ENTITY0=1-4827

lig: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=4842,4844
d1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=3803,lig COMPONENTS

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ...
  LABEL=dxy
  ARG=d1.x,d1.y
  VAR=ax,ay
  FUNC=(sqrt(ax*ax+ay*ay))
  PERIODIC=NO
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a>

<span style="color:blue">############################################################</span>
s_cent: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html">CONSTANT</a> VALUE=4            
beta_cent: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html">CONSTANT</a> VALUE=2
wall_width: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html">CONSTANT</a> VALUE=1.6     
wall_buffer: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html">CONSTANT</a> VALUE=0.15

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ...
 LABEL=wall_center
 ARG=d1.z,s_cent,beta_cent,wall_width,wall_buffer
 VAR=s,sc,b,h,f
 FUNC=h*(1./(1.+exp(b*(s-sc))))+f
 PERIODIC=NO
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a>


scaling: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html">CONSTANT</a> VALUES=1.0
spring: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html">CONSTANT</a> VALUES=3000.0

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ...
LABEL=wall_bias
ARG=dxy,spring,wall_center,scaling
VAR=z,k,zc,sf
FUNC=step(z-zc)*k*(z-zc)*(z-zc)/(sf*sf)
PERIODIC=NO
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a>

<span style="color:blue">############################################################</span>

meta: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=d1.z,dxy SIGMA=0.1,0.1 HEIGHT=1 PACE=500 FILE=HILLS GRID_MIN=-0.5,-0.5 GRID_MAX=5.5,5.5 GRID_SPACING=0.05,0.05 BIASFACTOR=15 TEMP=300
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=d1.z AT=5.0 KAPPA=1500.0 EXP=2 EPS=1 LABEL=uwall
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=d1.z AT=0.5 KAPPA=1500.0 EXP=2 EPS=1 LABEL=lwall

finalbias: <a href="https://plumed.github.io/doc-master/user-doc/html/_b_i_a_s_v_a_l_u_e.html">BIASVALUE</a> ARG=wall_bias

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=* STRIDE=500 FILE=COLVAR

</pre>{% endraw %}
