**Project ID:** [plumID:20.012]({{ '/' | absolute_url }}eggs/20/012/)  
**Source:** fun_SWISH/plumed.dat  
**Originally used with PLUMED version:** 2.4.2  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue">#####################################</span>
<span style="color:blue">#plumed.dat for Funnel MetaD + SWISH#</span>
<span style="color:blue">#####################################</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>


<span style="color:blue">###############################################</span>
<span style="color:blue">###DEFINE RADIUS + CALC PROT-LIG VECTOR COMP###</span>
<span style="color:blue">###############################################</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_a_d.html">LOAD</a> FILE=ProjectionOnAxis.cpp
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">MOLINFO</a> STRUCTURE=5akk_eqPR2_Ct_ALIGN.pdb
<a href="https://plumed.github.io/doc-master/user-doc/html/_i_n_c_l_u_d_e.html">INCLUDE</a> FILE=cmap.dat

<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> STRIDE=1 ENTITY0=1-5120 ENTITY1=5121-5137

<span style="color:blue">########################</span>
<span style="color:blue">###DEFINITION_OF_COMs###</span>
<span style="color:blue">########################</span>
lig: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=5121-5137		<span style="color:blue"># Ligand - 547 FRG</span>
p2_FS1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=3019,4303,4718	<span style="color:blue"># 196 SER@CA, 274 VAL@CA, 300 HIS(HIE)@CA</span>
p2_FS2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=2321,2160,4385,2411	<span style="color:blue"># 152 SER@CA, 141 ILE@CA, 279 MET@CA, 158 VAL@CA</span>
p1: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=3728			<span style="color:blue"># 241 TRP@CA</span>

<span style="color:blue">########################</span>
<span style="color:blue">###DEFINITION_OF_ARGs###</span>
<span style="color:blue">########################</span>
<span style="color:blue"># CV1: pp.proj = projection on the axis. The distance from the axis to the origin (along the axis)</span>
<span style="color:blue"># CV2: pp.ext = orthogonal distance between the ATOM(=lig) to the axis.</span>
<span style="color:blue"># CV3: ener = energy for the well-tempered ensemble. NOT for plain metaD.</span>
<span style="color:blue">##############################</span>
<span style="color:blue">###PoA_CV_for_Funnel_Side-1###</span>
<span style="color:blue">##############################</span>
<span style="color:blue">#pp: PROJECTION_ON_AXIS AXIS_ATOMS=p1,p2_FS1 ATOM=lig</span>

<span style="color:blue">##############################</span>
<span style="color:blue">###PoA_CV_for_Funnel_Side-2###</span>
<span style="color:blue">##############################</span>
pp: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_o_j_e_c_t_i_o_n__o_n__a_x_i_s.html">PROJECTION_ON_AXIS</a> AXIS_ATOMS=p1,p2_FS2 ATOM=lig



<span style="color:blue">#######################</span>
<span style="color:blue">###FUNNEL_PARAMETERS###</span>
<span style="color:blue">#######################</span>
s_cent: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html">CONSTANT</a> VALUES=3.0      	                              <span style="color:blue"># INFLEXION</span>
beta_cent: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html">CONSTANT</a> VALUES=1.5    	                              <span style="color:blue"># STEEPNESS</span>
wall_width: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html">CONSTANT</a> VALUES=1.2   	                              <span style="color:blue"># WIDTH (h)</span>
wall_buffer: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html">CONSTANT</a> VALUES=0.15  	                              <span style="color:blue"># BUFFER (f, total width = WIDTH + BUFFER)</span>
lwall: <a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=pp.proj AT=0.0 KAPPA=2000.0 EXP=2 EPS=1        <span style="color:blue"># Lower Wall (the starting point of the funnel)</span>
uwall: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=pp.proj,cmap AT=4.5,6.0 KAPPA=2000.0,3000.0 EXP=2,2 EPS=1,1 <span style="color:blue"># Upper Wall (the ending point of the funnel+restraint_4_swish)</span>


<span style="color:blue">##################################</span>
<span style="color:blue">###########CALCULATE FUNNEL#######</span>
<span style="color:blue"># Returns the radius of the funnel</span>
<span style="color:blue"># at the current value of the cv</span>
<span style="color:blue">##################################</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ...
	LABEL=wall_center
	ARG=pp.proj,s_cent,beta_cent,wall_width,wall_buffer
	VAR=s,sc,b,h,f
	FUNC=h*(1./(1.+exp(b*(s-sc))))+f
	PERIODIC=NO
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a>


<span style="color:blue">##############################</span>
<span style="color:blue">#####POTENTIAL_PARAMETERS#####</span>
<span style="color:blue">##############################</span>
scaling: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html">CONSTANT</a> VALUES=1.0
spring: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html">CONSTANT</a> VALUES=1000.0

<span style="color:blue">##############################</span>
<span style="color:blue">#######DEFINE_POTENTIAL#######</span>
<span style="color:blue">##############################</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ...
	LABEL=wall_bias
	ARG=pp.ext,spring,wall_center,scaling
	VAR=z,k,zc,sf
	FUNC=step(z-zc)*k*(z-zc)*(z-zc)/(sf*sf)
	PERIODIC=NO
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a>

finalbias: <a href="https://plumed.github.io/doc-master/user-doc/html/_b_i_a_s_v_a_l_u_e.html">BIASVALUE</a> ARG=wall_bias


<span style="color:blue">###############################</span>
<span style="color:blue">########DEFINE_METAD###########</span>
<span style="color:blue">###############################</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
	LABEL=meta ARG=pp.proj,pp.ext 
	SIGMA=0.025,0.03 HEIGHT=1.5 
	PACE=1000 FILE=HILLS 
        GRID_MIN=-0.5,0.0 GRID_MAX=5.0,2.0 GRID_SPACING=0.005,0.06
	BIASFACTOR=10.0 TEMP=300	
	
	REWEIGHTING_NGRID=1120,40
	REWEIGHTING_NHILLS=20
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>
<span style="color:blue">#GRID_MIN=0.0,0.0 GRID_MAX=2.0,2.0 GRID_BIN=160,133</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=* STRIDE=1000 FILE=COLVAR FMT=%8.4f

</pre>{% endraw %}
