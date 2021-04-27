**Project ID:** [plumID:21.008]({{ '/' | absolute_url }}eggs/21/008/)  
**Source:** REM-FEP/replica033/plumed.dat  
**Originally used with PLUMED version:** 2.7  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> STRIDE=1 ENTITY0=1-347




<a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=4,3,84,85    LABEL=T1   
<a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=74,73,153,154  LABEL=T2
<a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=143,142,222,223 LABEL=T3
<a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=212,211,280,293  LABEL=T4     


<span style="color:blue"># this the lambda value for current window</span>
lambda1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html">CONSTANT</a> VALUE=1.00
lambda2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html">CONSTANT</a> VALUE=0.70



<span style="color:blue"># first we define V0 for T1</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ...
 LABEL=V0_1 ARG=T1 VAR=x
 FUNC=12.16-0.024*cos(x-pi)-43.32*(cos(x-pi))^2+0.12*(cos(x-pi))^3+38.8*(cos(x-pi))^4-0.0601*(cos(x-pi))^5
 PERIODIC=NO
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a>

<span style="color:blue"># then V1 for T1</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ...
 LABEL=V1_1 ARG=T1 VAR=x
 FUNC=301.3-0.1478*cos(x-pi)-48.16*(cos(x-pi))^2+0.9948*(cos(x-pi))^3+34.30*(cos(x-pi))^4-1.001*(cos(x-pi))^5
 PERIODIC=NO
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a>


<span style="color:blue"># then V2 for T1</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ...
 LABEL=V2_1 ARG=T1 VAR=x
 FUNC=348.8-0.1104*cos(x-pi)-54.71*(cos(x-pi))^2+0.7533*(cos(x-pi))^3+35.14*(cos(x-pi))^4-0.8068*(cos(x-pi))^5
 PERIODIC=NO
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a>


<span style="color:blue"># first we define V0 for T2</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ...
 LABEL=V0_2 ARG=T2 VAR=x
 FUNC=12.16-0.024*cos(x-pi)-43.32*(cos(x-pi))^2+0.12*(cos(x-pi))^3+38.8*(cos(x-pi))^4-0.0601*(cos(x-pi))^5
 PERIODIC=NO
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a>

<span style="color:blue"># then V1 for T2</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ...
 LABEL=V1_2 ARG=T2 VAR=x
 FUNC=313.9+0.3972*cos(x-pi)-72.12*(cos(x-pi))^2-0.9463*(cos(x-pi))^3+43.87*(cos(x-pi))^4+0.5858*(cos(x-pi))^5
 PERIODIC=NO
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a>


<span style="color:blue"># then V2 for T2</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ...
 LABEL=V2_2 ARG=T2 VAR=x
 FUNC=351.9-0.7135*cos(x-pi)-69.01*(cos(x-pi))^2+0.653*(cos(x-pi))^3+47.11*(cos(x-pi))^4+0.41*(cos(x-pi))^5
 PERIODIC=NO
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a>



<span style="color:blue"># first we define V0 for T3</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ...
 LABEL=V0_3 ARG=T3 VAR=x
 FUNC=12.16-0.024*cos(x-pi)-43.32*(cos(x-pi))^2+0.12*(cos(x-pi))^3+38.8*(cos(x-pi))^4-0.0601*(cos(x-pi))^5
 PERIODIC=NO
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a>

<span style="color:blue"># then V1 for T3</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ...
 LABEL=V1_3 ARG=T3 VAR=x
 FUNC=313.9+0.3972*cos(x-pi)-72.12*(cos(x-pi))^2-0.9463*(cos(x-pi))^3+43.87*(cos(x-pi))^4+0.5858*(cos(x-pi))^5
 PERIODIC=NO
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a>


<span style="color:blue"># then V2 for T3</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ...
 LABEL=V2_3 ARG=T3 VAR=x
 FUNC=351.9-0.7135*cos(x-pi)-69.01*(cos(x-pi))^2+0.653*(cos(x-pi))^3+47.11*(cos(x-pi))^4+0.41*(cos(x-pi))^5
 PERIODIC=NO
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a>



<span style="color:blue"># first we define V0 for T4</span>



<a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ...
 LABEL=V0_4 ARG=T4 VAR=x
 FUNC=12.16-0.024*cos(x-pi)-43.32*(cos(x-pi))^2+0.12*(cos(x-pi))^3+38.8*(cos(x-pi))^4-0.0601*(cos(x-pi))^5
 PERIODIC=NO
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a>

<span style="color:blue"># then V1 for T4</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ...
 LABEL=V1_4 ARG=T4 VAR=x
 FUNC=301.3-0.1478*cos(x-pi)-48.16*(cos(x-pi))^2+0.9948*(cos(x-pi))^3+34.30*(cos(x-pi))^4-1.001*(cos(x-pi))^5
 PERIODIC=NO
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a>


<span style="color:blue"># then V2 for T4</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ...
 LABEL=V2_4 ARG=T4 VAR=x
 FUNC=348.8-0.1104*cos(x-pi)-54.71*(cos(x-pi))^2+0.7533*(cos(x-pi))^3+35.14*(cos(x-pi))^4-0.8068*(cos(x-pi))^5
 PERIODIC=NO
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a>





<span style="color:blue"># This is Vlambda1 for current window</span>
Vlambda1: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=V0_1,V1_1,V2_1,lambda1,lambda2 VAR=x,y,z,l1,l2 FUNC=(1.0-l1)*x+l1*(1-l2)*y+l2*z PERIODIC=NO
Vlambdam1: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=V0_1,V1_1,V2_1,lambda1,lambda2 VAR=x,y,z,l1,l2 FUNC=(1.0-l1)*x+(l1)*(1-l2+0.1)*y+(l2-0.1)*z PERIODIC=NO
Vlambdap1: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=V0_1,V1_1,V2_1,lambda1,lambda2 VAR=x,y,z,l1,l2 FUNC=(1.0-l1)*x+(l1)*(1-l2-0.1)*y+(l2+0.1)*z PERIODIC=NO

Vlbias1: <a href="https://plumed.github.io/doc-master/user-doc/html/_b_i_a_s_v_a_l_u_e.html">BIASVALUE</a> ARG=Vlambda1


<span style="color:blue"># This is Vlambda2 for current window</span>
Vlambda2: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=V0_2,V1_2,V2_2,lambda1,lambda2 VAR=x,y,z,l1,l2 FUNC=(1.0-l1)*x+l1*(1-l2)*y+l2*z PERIODIC=NO
Vlambdam2: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=V0_2,V1_2,V2_2,lambda1,lambda2 VAR=x,y,z,l1,l2 FUNC=(1.0-l1)*x+(l1)*(1-l2+0.1)*y+(l2-0.1)*z PERIODIC=NO
Vlambdap2: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=V0_2,V1_2,V2_2,lambda1,lambda2 VAR=x,y,z,l1,l2 FUNC=(1.0-l1)*x+(l1)*(1-l2-0.1)*y+(l2+0.1)*z PERIODIC=NO

Vlbias2: <a href="https://plumed.github.io/doc-master/user-doc/html/_b_i_a_s_v_a_l_u_e.html">BIASVALUE</a> ARG=Vlambda2


<span style="color:blue"># This is Vlambda3 for current window</span>
Vlambda3: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=V0_3,V1_3,V2_3,lambda1,lambda2 VAR=x,y,z,l1,l2 FUNC=(1.0-l1)*x+l1*(1-l2)*y+l2*z PERIODIC=NO
Vlambdam3: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=V0_3,V1_3,V2_3,lambda1,lambda2 VAR=x,y,z,l1,l2 FUNC=(1.0-l1)*x+(l1)*(1-l2+0.1)*y+(l2-0.1)*z PERIODIC=NO
Vlambdap3: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=V0_3,V1_3,V2_3,lambda1,lambda2 VAR=x,y,z,l1,l2 FUNC=(1.0-l1)*x+(l1)*(1-l2-0.1)*y+(l2+0.1)*z PERIODIC=NO

Vlbias3: <a href="https://plumed.github.io/doc-master/user-doc/html/_b_i_a_s_v_a_l_u_e.html">BIASVALUE</a> ARG=Vlambda3


<span style="color:blue"># This is Vlambda4 for current window</span>
Vlambda4: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=V0_4,V1_4,V2_4,lambda1,lambda2 VAR=x,y,z,l1,l2 FUNC=(1.0-l1)*x+l1*(1-l2)*y+l2*z PERIODIC=NO
Vlambdam4: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=V0_4,V1_4,V2_4,lambda1,lambda2 VAR=x,y,z,l1,l2 FUNC=(1.0-l1)*x+(l1)*(1-l2+0.1)*y+(l2-0.1)*z PERIODIC=NO
Vlambdap4: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=V0_4,V1_4,V2_4,lambda1,lambda2 VAR=x,y,z,l1,l2 FUNC=(1.0-l1)*x+(l1)*(1-l2-0.1)*y+(l2+0.1)*z PERIODIC=NO

Vlbias4: <a href="https://plumed.github.io/doc-master/user-doc/html/_b_i_a_s_v_a_l_u_e.html">BIASVALUE</a> ARG=Vlambda4




<a href="https://plumed.github.io/doc-master/user-doc/html/_p_b_m_e_t_a_d.html">PBMETAD</a> ...
ARG=T1,T2,T3,T4 SIGMA=0.2,0.2,0.2,0.2  HEIGHT=1.2 PACE=500 BIASFACTOR=40 LABEL=pb
FILE=HILLS_T1,HILLS_T2,HILLS_T3,HILLS_T4
... <a href="https://plumed.github.io/doc-master/user-doc/html/_p_b_m_e_t_a_d.html">PBMETAD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=T1,T2,T3,T4,Vlambdam1,Vlambda1,Vlambdap1,Vlambdam2,Vlambda2,Vlambdap2,Vlambdam3,Vlambda3,Vlambdap3,Vlambdam4,Vlambda4,Vlambdap4,pb.bias  STRIDE=500 FILE=COLVAR

</pre>{% endraw %}
