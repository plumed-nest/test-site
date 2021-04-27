**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
**Source:** regtest/pycv/rt-f2/plumed.dat  
**Originally used with PLUMED version:** 2.5.2-mod  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># Copy of basic/rt13</span>

g1: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=1-10
c1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a>   ATOMS=g1

t1: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=1,6,10,15
t2: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=6,1 AXIS=6,10 VECTOR2=10,15
t3: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=6,1 AXIS=20,7 VECTOR2=10,c1

cc1: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_y_t_h_o_n_f_u_n_c_t_i_o_n.html">PYTHONFUNCTION</a> ARG=t1,t2,t3 IMPORT=pythonfunction FUNCTION=cc1 PERIODIC=NO
cc2: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_y_t_h_o_n_f_u_n_c_t_i_o_n.html">PYTHONFUNCTION</a> ARG=t1,t2,t3 IMPORT=pythonfunction FUNCTION=cc2 PERIODIC=NO
cc3: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_y_t_h_o_n_f_u_n_c_t_i_o_n.html">PYTHONFUNCTION</a> ARG=t1,t2    IMPORT=pythonfunction FUNCTION=cc3 PERIODIC=NO

<span style="color:blue"># cc1: MATHEVAL ARG=t1,t2,t3 FUNC=x^2+y+0*z+1 PERIODIC=NO</span>
<span style="color:blue"># cc2: MATHEVAL ARG=t1,t2,t3 FUNC=0*x^3+0*y^3+0*z^3 PERIODIC=NO</span>
<span style="color:blue"># cc3: MATHEVAL ARG=t1,t2 FUNC=x^2+y^2 PERIODIC=NO</span>

all: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=t1,t2,t3,cc1,cc2,cc3 VAR=a1,a2,a3,a4,a5,a6 FUNC={ (a1+a2+a3+a4+a5+a6) / 6.0 } PERIODIC=NO

<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=all AT=0 SLOPE=1.0

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ...
  STRIDE=2
  ARG=t1,t2,t3,cc1,cc2,cc3,all
  FILE=COLVAR FMT=%6.5f
... <a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
<span style="color:blue"></span>
</pre>{% endraw %}
