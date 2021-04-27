**Project ID:** [plumID:21.015]({{ '/' | absolute_url }}eggs/21/015/)  
**Source:** US/CBM73/plumed19.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [raw zipped stdout](plumed19.dat.plumed.stdout.txt.zip) - [stderr](plumed19.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed19.dat.plumed_master.stdout.txt.zip) - [stderr](plumed19.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=721-882

a1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=793-797 
a2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=809-812 
a3: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=828-832 
achi: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1-720 

p1: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_o_s_i_t_i_o_n.html">POSITION</a> ATOM=a1 NOPBC
p2: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_o_s_i_t_i_o_n.html">POSITION</a> ATOM=a2 NOPBC
p3: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_o_s_i_t_i_o_n.html">POSITION</a> ATOM=a3 NOPBC
pchi: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_o_s_i_t_i_o_n.html">POSITION</a> ATOM=achi NOPBC

distx: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=p1.x,p2.x,p3.x,pchi.x VAR=a,b,c,y FUNC=((y-a)^2+(y-b)^2+(y-c)^2)^0.5 PERIODIC=NO

restraint-bnd: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=distx KAPPA=100.0 AT=0.6

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=distx,restraint-bnd.bias STRIDE=5000 FILE=COLVAR19

</pre>{% endraw %}
