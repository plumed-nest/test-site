**Project ID:** [plumID:19.018]({{ '/' | absolute_url }}eggs/19/018/)  
**Source:** plumed_excitedstates.dat  
**Originally used with PLUMED version:** 2.3  
**Stable:** [raw zipped stdout](plumed_excitedstates.dat.plumed.stdout.txt.zip) - [stderr](plumed_excitedstates.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_excitedstates.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_excitedstates.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> STRIDE=1 ENTITY0=1-107
T1:  <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=4,3,36,37
T2:  <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=58,57,25,26
T3:    <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=79,78,46,47


<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=T3 SIGMA=0.2 HEIGHT=1.2 PACE=500 FILE=HILLS_0.00 BIASFACTOR=25.0 TEMP=300.0 GRID_MIN=-pi GRID_MAX=pi

<span style="color:blue"># this the lambda value for current window</span>
lambda: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html">CONSTANT</a> VALUE=0.00

<span style="color:blue"># first we define V0</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ...
 LABEL=V0 ARG=T3 VAR=x
 FUNC=13.68-0.057*cos(x-pi)-48.06*(cos(x-pi))^2+0.17*(cos(x-pi))^3+42.2*(cos(x-pi))^4-0.0809*(cos(x-pi))^5
 PERIODIC=NO
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a>

<span style="color:blue"># then V1</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ...
 LABEL=V1 ARG=T3 VAR=x
 FUNC=341.-0.463*cos(x-pi)-92.73*(cos(x-pi))^2+1.23*(cos(x-pi))^3+55.6*(cos(x-pi))^4-0.803*(cos(x-pi))^5
 PERIODIC=NO
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a>

<span style="color:blue"># This is Vlambda for current window</span>
Vlambda: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=V0,V1,lambda VAR=x,y,z FUNC=(1.0-z)*x+z*y PERIODIC=NO

<span style="color:blue"># These are Vlambda for nearest neighbors</span>
Vlambdap: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=V0,V1,lambda VAR=x,y,z FUNC=(1.0-z-0.02)*x+(z+0.02)*y PERIODIC=NO
Vlambdam: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=V0,V1,lambda VAR=x,y,z FUNC=(1.0-z+0.02)*x+(z-0.02)*y PERIODIC=NO

<span style="color:blue"># activate Vlambda bias for current window</span>
Vlbias: <a href="https://plumed.github.io/doc-master/user-doc/html/_b_i_a_s_v_a_l_u_e.html">BIASVALUE</a> ARG=Vlambda

<span style="color:blue"># print out useful stuff</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=T3,Vlambdam,Vlambda,Vlambdap,T1,T2 STRIDE=500 FILE=COLVAR_0.00
</pre>{% endraw %}
