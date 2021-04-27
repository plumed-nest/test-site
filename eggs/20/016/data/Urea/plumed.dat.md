**Project ID:** [plumID:20.016]({{ '/' | absolute_url }}eggs/20/016/)  
**Source:** Urea/plumed.dat  
**Originally used with PLUMED version:** 2.6-dev  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># Restart simulation. This command will append results of new simulations to the same output files, e.g. COLVAR.</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_a_d.html">LOAD</a> FILE=PairOrientationalEntropy.cpp

<span style="color:blue"># Define groups for the CV</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_i_n_c_l_u_d_e.html">INCLUDE</a> FILE=<a href="centers.dat.html">centers.dat</a>
C: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=1-864:8
O: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=2-864:8
N1: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=3-864:8
N2: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6-864:8
 
<span style="color:blue"># Define the CV</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_a_i_r__o_r_i_e_n_t_a_t_i_o_n_a_l__e_n_t_r_o_p_y.html">PAIR_ORIENTATIONAL_ENTROPY</a> ...
 LABEL=s1
 CENTER=C
 START=Ncenter
 END=O
 MAXR=0.6
 SIGMA=0.05,0.25
... <a href="https://plumed.github.io/doc-master/user-doc/html/_p_a_i_r__o_r_i_e_n_t_a_t_i_o_n_a_l__e_n_t_r_o_p_y.html">PAIR_ORIENTATIONAL_ENTROPY</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_a_i_r__o_r_i_e_n_t_a_t_i_o_n_a_l__e_n_t_r_o_p_y.html">PAIR_ORIENTATIONAL_ENTROPY</a> ...
 LABEL=s2
 CENTER=C
 START=N1
 END=N2
 MAXR=0.6
 SIGMA=0.05,0.125
 UP_DOWN_SYMMETRY
... <a href="https://plumed.github.io/doc-master/user-doc/html/_p_a_i_r__o_r_i_e_n_t_a_t_i_o_n_a_l__e_n_t_r_o_p_y.html">PAIR_ORIENTATIONAL_ENTROPY</a>

<span style="color:blue"># Construct a bias potential using metadynamics</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
 LABEL=metad
 ARG=s1,s2   <span style="color:blue"># Label of the CV</span>
 PACE=500   <span style="color:blue"># Pace in the deposition of the gaussians</span>
 HEIGHT=18.705   <span style="color:blue"># Height of the gaussians in energy units kJ/mol. This is 5 kT.</span>
 SIGMA=0.1,0.1   <span style="color:blue"># Width of the gaussian in CV units</span>
 FILE=HILLS   <span style="color:blue"># File where the information of the gaussians is printed</span>
 BIASFACTOR=200.0   <span style="color:blue"># Bias factor in well tempered simulations</span>
 TEMP=450.0   <span style="color:blue"># Temperature in Kelvin. Only needed for well tempered simulations</span>
 GRID_MIN=-14.0,-14.0   <span style="color:blue"># The following three lines define a grid for the calculation of the bias potential. Use it **always**.</span>
 GRID_MAX=0.,0.
 GRID_BIN=600,600
 CALC_RCT
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<span style="color:blue"># Print value of the CV and bias to a file named COLVAR</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=500  ARG=* FILE=COLVAR   




</pre>{% endraw %}
