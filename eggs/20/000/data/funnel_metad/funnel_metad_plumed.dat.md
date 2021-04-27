**Project ID:** [plumID:20.000]({{ '/' | absolute_url }}eggs/20/000/)  
**Source:** funnel_metad/funnel_metad_plumed.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [raw zipped stdout](funnel_metad_plumed.dat.plumed.stdout.txt.zip) - [stderr](funnel_metad_plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](funnel_metad_plumed.dat.plumed_master.stdout.txt.zip) - [stderr](funnel_metad_plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue">#</span>
<span style="color:blue"># This is the input file needed to perform funnel metadynamics simulation</span>
<span style="color:blue"># based on the MC-HLDA CVs </span>
<span style="color:blue">#</span>
<span style="color:blue"># This input file can be used with all the PLUMED versions >=2.3</span>
<span style="color:blue">#</span>

<span style="color:blue"># Definition of the center of mass of the ligand, considering only its heavy atoms</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=1,5,6,10,14,17,18,19,22,23,24,25,26,29  LABEL=ixo

<span style="color:blue"># Definition of the center of mass of the pocket</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=1396,1398,1400,1403,1404,1406,1408,1409,1411,1413,1415,1416,1449,1451,1453,1456,1458,1459,1495,1497,1499,1501,1505,1509,1510,2838,2840,2842,2845,2846,2848,2850,2852,2854,2856,2857,3605,3607,3609,3612,3613,3615,3617,3618,3620,3622,3624,3625 LABEL=pkt

<span style="color:blue"># Definition of the distance between the ligand and the pocket as a 3d vector xyz</span>
<span style="color:blue"># (the membrane is in the plane xy)</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=ixo,pkt LABEL=d1 COMPONENTS NOPBC

<span style="color:blue"># Definition of the periodicity of the components of the distance </span>
<span style="color:blue"># (to avoid jumps in the variable during the simulation due to the </span>
<span style="color:blue"># rototranslation of the system)</span>
d1x: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1.x PERIODIC=-4.7,4.7
d1y: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1.y PERIODIC=-4.7,4.7
d1z: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1.z PERIODIC=-8.2,8.2

<span style="color:blue"># We define the radius of the funnel potential on the xy plane (the same of the membrane) </span>
radius: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=d1x,d1y VAR=x,y FUNC=sqrt(x*x+y*y) PERIODIC=NO
<span style="color:blue"># We define the conical and the cylindrical part of the funnel potential</span>
funnel: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=radius,d1z VAR=r,z FUNC=(r-(z+1.8))*step(z+1.7)+(r-0.1)*step(-1.7-z) PERIODIC=NO
<span style="color:blue"># We define the funnel potential</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> AT=0 ARG=funnel KAPPA=2000.0 LABEL=funnelwall


<span style="color:blue"># Wall on distance to prevent the ligand exit to the solvent</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> AT=-4.0 ARG=d1.z KAPPA=2000.0 LABEL=topwall
<span style="color:blue"># Wall on distance to prevent the ligand entering the intracellular part</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> AT=0.3 ARG=d1.z KAPPA=2000.0 LABEL=bottomwall

<span style="color:blue"># Contact related to the nonbonded interactions in bound state</span>
bound_d1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=25,3637
bound_d2: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=24,3637
bound_d3: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=25,2842
bound_d4: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=26,2837
bound_d5: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=24,3620
bound_d6: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=26,1505
bound_d7: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=17,1398

<span style="color:blue"># Contact related to the nonbonded interactions in state A </span>
cl2_d1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=25,1409
cl2_d2: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=24,1409
cl2_d3: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=14,1456
cl2_d4: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=14,1411
cl2_d5: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=19,3622
cl2_d6: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=14,1408

<span style="color:blue"># Contact related to the nonbonded interactions in state B</span>
cl3_d1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=14,1404
cl3_d2: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=14,3975
cl3_d3: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=10,1413
cl3_d4: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=24,3613

<span style="color:blue"># Contact related to the nonbonded interactions in state C</span>
cl5_d1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=24,3618
cl5_d2: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=25,3618
cl5_d3: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=23,3615
cl5_d4: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=29,2791

<span style="color:blue"># Salt bridges</span>
sb_d1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=5,1392
sb_d2: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=5,1393

<span style="color:blue"># Eigenvectors from the MC-HLDA analysis on the contacts</span>
eig1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=bound_d1,bound_d2,bound_d3,bound_d4,bound_d5,bound_d6,bound_d7,cl2_d1,cl2_d2,cl2_d3,cl2_d4,cl2_d5,cl2_d6,cl3_d1,cl3_d2,cl3_d3,cl3_d4,cl5_d1,cl5_d2,cl5_d3,cl5_d4,sb_d1,sb_d2 COEFFICIENTS=0.312,-0.262,0.116,0.021,0.411,0.020,0.073,0.484,-0.490,0.004,0.007,-0.008,-0.002,-0.037,-0.009,-0.001,0.085,-0.054,-0.347,-0.153,0.124,-0.022,-0.012 PERIODIC=NO
eig2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=bound_d1,bound_d2,bound_d3,bound_d4,bound_d5,bound_d6,bound_d7,cl2_d1,cl2_d2,cl2_d3,cl2_d4,cl2_d5,cl2_d6,cl3_d1,cl3_d2,cl3_d3,cl3_d4,cl5_d1,cl5_d2,cl5_d3,cl5_d4,sb_d1,sb_d2 COEFFICIENTS=-0.509,0.468,0.025,0.031,-0.211,-0.003,-0.008,0.239,-0.218,-0.002,-0.004,-0.227,-0.019,0.005,0.006,-0.006,-0.173,0.106,0.430,0.090,0.289,0.015,0.029 PERIODIC=NO
eig3: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=bound_d1,bound_d2,bound_d3,bound_d4,bound_d5,bound_d6,bound_d7,cl2_d1,cl2_d2,cl2_d3,cl2_d4,cl2_d5,cl2_d6,cl3_d1,cl3_d2,cl3_d3,cl3_d4,cl5_d1,cl5_d2,cl5_d3,cl5_d4,sb_d1,sb_d2 COEFFICIENTS=-0.367,0.354,-0.078,-0.003,0.104,-0.008,-0.118,0.424,-0.307,-0.011,0.063,0.077,-0.059,0.119,0.014,0.004,0.175,-0.558,0.237,0.089,0.013,0.021,0.022 PERIODIC=NO

<span style="color:blue"># Multiple-walkers well-tempered metadynamics on the MC-HLDA eigenvectors</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
LABEL=metad
ARG=eig1,eig2
PACE=500 HEIGHT=1.2 
BIASFACTOR=24.
TEMP=310.15
SIGMA=0.015,0.015
FILE=../HILLS 
GRID_MIN=-0.1,-0.2
GRID_MAX=2.,2.
WALKERS_MPI
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<span style="color:blue"># Here we print all the data regarding metadynamics</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=metad.* STRIDE=500 FILE=metaD_data
<span style="color:blue"># Here we print all the data regarding barriers</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=d1.z,topwall.*,bottomwall.* STRIDE=500 FILE=IXO_dist.dat
<span style="color:blue"># Here we print all the data regarding ligand position and funnel potential</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=d1.x,d1.y,d1.z,d1x,d1y,d1z,radius,funnel,funnelwall.* STRIDE=500 FILE=funnel_dist.dat
<span style="color:blue"># Here we print all the data regarding the MC-HLDA eigenvectors </span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=eig1,eig2,eig3 STRIDE=500 FILE=eigenvectors.dat
<span style="color:blue"># Here we print all the distances for the contacts </span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=bound_d1,bound_d2,bound_d3,bound_d4,bound_d5,bound_d6,bound_d7,cl2_d1,cl2_d2,cl2_d3,cl2_d4,cl2_d5,cl2_d6,cl3_d1,cl3_d2,cl3_d3,cl3_d4,cl5_d1,cl5_d2,cl5_d3,cl5_d4,sb_d1,sb_d2 STRIDE=500 FILE=contacts.dat

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
