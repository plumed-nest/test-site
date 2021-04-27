**Project ID:** [plumID:21.001]({{ '/' | absolute_url }}eggs/21/001/)  
**Source:** HS2ST/plumed.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>

<span style="color:blue">##########################################################################################</span>
<span style="color:blue">#DO NOT LOOK AT Plucker right now, theta and phi can only see one boat conformation</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_u_c_k_e_r_i_n_g.html">PUCKERING</a> ATOMS=14614,14612,14626,14622,14620,14615  LABEL=puck

<span style="color:blue">##########################################################################################</span>

<span style="color:blue">#set up distance iduo2-papsS</span>
O2: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=14628
S: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=14727
dP:   <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=O2,S
<span style="color:blue">##########################################################################################</span>

metad: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=dP,puck.qx,puck.qy,puck.qz PACE=500 HEIGHT=2.0 SIGMA=0.1,0.2,0.2,0.2 FILE=HILLS3 BIASFACTOR=50.0 GRID_MIN=0,-pi,-pi,-pi GRID_MAX=1.2,2pi,2pi,2pi TEMP=300.0 GRID_BIN=100,100,100,100

<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=dP AT=1 KAPPA=35100 EXP=2 OFFSET=0 LABEL=uwall
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=dP,puck.qz AT=0.3,0.05 KAPPA=35100,1000.0 EXP=2,2 OFFSET=0,0 LABEL=lwall


<span style="color:blue"># monitor the two variables and the metadynamics bias potential</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=10 ARG=*  FILE=COLVAR

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=10 ARG=puck.phi,puck.theta,metad.bias  FILE=COLVAR2
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=10 ARG=puck.phi,puck.amplitude,metad.bias  FILE=COLVAR3
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=10 ARG=puck.amplitude,puck.theta,metad.bias  FILE=COLVAR4


<span style="color:blue">##########################################################################################</span>

</pre>{% endraw %}
