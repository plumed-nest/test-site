**Project ID:** [plumID:20.016]({{ '/' | absolute_url }}eggs/20/016/)  
**Source:** Naphthalene/plumed.dat  
**Originally used with PLUMED version:** 2.6-dev  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># Restart simulation. This command will append results of new simulations to the same output files, e.g. COLVAR.</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_a_d.html">LOAD</a> FILE=PairOrientationalEntropy.cpp
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_a_d.html">LOAD</a> FILE=PairOrientationalEntropyPerpendicular.cpp

<span style="color:blue"># Define groups for the CV</span>
C8: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=8-648:18 <span style="color:blue"># Head</span>
C9: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=9-648:18 <span style="color:blue"># Head</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_i_n_c_l_u_d_e.html">INCLUDE</a> FILE=<a href="centers.dat.html">centers.dat</a>

<span style="color:blue"># Define the CV</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_a_i_r__o_r_i_e_n_t_a_t_i_o_n_a_l__e_n_t_r_o_p_y.html">PAIR_ORIENTATIONAL_ENTROPY</a> ...
 LABEL=s1
 CENTER=CENTERS
 START=STARTS
 END=ENDS
 MAXR=0.7
 SIGMA=0.05,0.125
 <span style="color:blue">#REFERENCE_DENSITY=4.5</span>
 UP_DOWN_SYMMETRY
 LOW_COMM
... <a href="https://plumed.github.io/doc-master/user-doc/html/_p_a_i_r__o_r_i_e_n_t_a_t_i_o_n_a_l__e_n_t_r_o_p_y.html">PAIR_ORIENTATIONAL_ENTROPY</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_a_i_r__o_r_i_e_n_t_a_t_i_o_n_a_l__e_n_t_r_o_p_y__p_e_r_p_e_n_d_i_c_u_l_a_r.html">PAIR_ORIENTATIONAL_ENTROPY_PERPENDICULAR</a> ...
 LABEL=s2
 CENTER=CENTERS
 START1=STARTS
 END1=ENDS
 START2=C8
 END2=C9
 MAXR=0.7
 SIGMA=0.05,0.125
 <span style="color:blue">#REFERENCE_DENSITY=4.5</span>
 UP_DOWN_SYMMETRY
 LOW_COMM
... <a href="https://plumed.github.io/doc-master/user-doc/html/_p_a_i_r__o_r_i_e_n_t_a_t_i_o_n_a_l__e_n_t_r_o_p_y__p_e_r_p_e_n_d_i_c_u_l_a_r.html">PAIR_ORIENTATIONAL_ENTROPY_PERPENDICULAR</a>

<span style="color:blue"># Construct a bias potential using metadynamics</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
 LABEL=metad
 ARG=s1,s2   <span style="color:blue"># Label of the CV</span>
 PACE=500   <span style="color:blue"># Pace in the deposition of the gaussians</span>
 HEIGHT=12.25   <span style="color:blue"># Height of the gaussians in energy units kJ/mol. This is 2 kT.</span>
 SIGMA=0.2,0.2    <span style="color:blue"># Width of the gaussian in CV units</span>
 FILE=HILLS   <span style="color:blue"># File where the information of the gaussians is printed</span>
 BIASFACTOR=200.0   <span style="color:blue"># Bias factor in well tempered simulations</span>
 TEMP=300.0   <span style="color:blue"># Temperature in Kelvin. Only needed for well tempered simulations</span>
 GRID_MIN=-20.0,-20.0   <span style="color:blue"># The following three lines define a grid for the calculation of the bias potential. Use it **always**.</span>
 GRID_MAX=0.,0.
 GRID_BIN=1000,1000
 CALC_RCT
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<span style="color:blue"># Restraint the volume</span>
vol: <a href="https://plumed.github.io/doc-master/user-doc/html/_v_o_l_u_m_e.html">VOLUME</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=vol AT=12.0 KAPPA=1000.0 EXP=1 LABEL=uwall

<span style="color:blue"># Print value of the CV and bias to a file named COLVAR</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=500  ARG=* FILE=COLVAR   

</pre>{% endraw %}
