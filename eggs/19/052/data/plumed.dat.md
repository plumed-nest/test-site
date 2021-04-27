**Project ID:** [plumID:19.052]({{ '/' | absolute_url }}eggs/19/052/)  
**Source:** plumed.dat  
**Originally used with PLUMED version:** not specified  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> NATURAL 
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>
<span style="color:blue"># Record the volume of the simulation cell.</span>
cell: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_l_l.html">CELL</a>
<span style="color:blue"># We first compute the local order parameter for each atom using the cubic harmonic function “FCCUBIC”. The sigmoid switching function “SMAP” is used to transform these quantities with a non-linear mapping on. </span>
<span style="color:blue"># We compute the sum of these transformed order parameters using the keyword “MORE THAN”. The value of “cub.morethan” is thus proportional to the number of atoms in the fcc crystal.</span>
<span style="color:blue"># The system contains a total of 23328 real atoms, The first atom is a “ghost” atom that stays stationary at the center of the supercell. This ghost atom is only used as a reference point</span>
cub: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_c_c_u_b_i_c.html">FCCUBIC</a> SPECIES=2-23329 SWITCH={CUBIC D_0=1.2 D_MAX=1.5} ALPHA=27 MEAN MORE_THAN1={SMAP R_0=0.45 D_0=0.0 A=8 B=8}

<span style="color:blue"># Perform a metadynamics simulation</span>
metad: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
ARG=cub.morethan-1
PACE=1000 HEIGHT=0.3 SIGMA=600 FILE=HILLS TEMP=0.58 BIASFACTOR=400
ADAPTIVE=DIFF SIGMA_MAX=300 SIGMA_MIN=0.1 
... 

fixmax: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=cub.morethan-1 AT=2500 KAPPA=0.1
<span style="color:blue"># monitor the two variables and the metadynamics bias potential </span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=10 ARG=cell.ax,cub.*,metad.bias,fixmax.bias FILE=COLVAR
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
