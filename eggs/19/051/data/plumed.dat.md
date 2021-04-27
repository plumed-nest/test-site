**Project ID:** [plumID:19.051]({{ '/' | absolute_url }}eggs/19/051/)  
**Source:** plumed.dat  
**Originally used with PLUMED version:** not specified  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># This input was used to compute the surface free energy excess for the 111 surface. </span>
<span style="color:blue"># In addition to returning the metadynamics bias potential that promotes the solid-liquid transitions, </span>
<span style="color:blue"># this PLUMED input also defines a number of restraint potentials that ensure that the central region </span>
<span style="color:blue"># of the supercell remains in the solid, fcc structure.</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> NATURAL
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>
<span style="color:blue"># Record the shape of the simulation cell.</span>
cell: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_l_l.html">CELL</a>
<span style="color:blue"># We compute the local order parameter for each atom using the cubic harmonic function “FCCUBIC”. </span>
<span style="color:blue"># By specifying these Euler angles we ensure that the CV only identifies atoms as being in an fcc crystals if the 111 lattice direction is along the x axis of the system. </span>
<span style="color:blue"># The sigmoid switching function “SMAP” is used to do a non-linear mapping of these symmetry function values. </span>
<span style="color:blue"># We collect the sum of the transforced FCCCUBIC parameters for all of the atoms so the value of “cub.morethan” is proportional to the number of atoms in the fcc crystal with the specified lattice direction.</span>
<span style="color:blue"># The system contains a total of 1152 real atoms, The 1153th atom is a “ghost” atom that stays stationary at the center of the supercell. </span>
<span style="color:blue"># This ghost atom is only used as a reference point and allows us to indicate the relative positions of the atoms in some CVs.</span>
cub: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_c_c_u_b_i_c.html">FCCUBIC</a> ...
SPECIES=1-1152 SWITCH={CUBIC D_0=1.2 D_MAX=1.5}
MEAN
MORE_THAN={SMAP R_0=0.45 D_0=0.0 A=8 B=8}
ALPHA=27 PHI=-1.5708 THETA=-0.61548 PSI=0.785389
... 
<span style="color:blue"># At undercooled conditions, the system has a strong tendency to form solids. Although the central region of the supercell is constrained to remain as an fcc crystal with the 111 lattice direction along the x axis of the system, </span>
<span style="color:blue"># the peripheral region is likely to form twinned crystals or mis-oriented crystals with grain boundaries. As the local order parameter is not rotational-invariant, any atoms in wrongly orientated crystals usually adopt values </span>
<span style="color:blue"># intermediate between those obtained for bulk solid and liquid. These crystals with unwanted orientations will be misidentified as partially liquid, and will be included in the computed free energy profile. When this happens, </span>
<span style="color:blue"># the free energy profile shows bumps, which hinders the determination of the chemical potnetial and surface excess free energy. For this reason, “cub2”, “cub3”, “cub4” and “cub5” are used to identify fcc crystals with unwanted </span>
<span style="color:blue"># orientations. Constraints are added on these CVs to prevent the formation of solid phase with an orientation incompatible with the simulation box.</span>
cub2: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_c_c_u_b_i_c.html">FCCUBIC</a> ...
SPECIES=1-1152 SWITCH={CUBIC D_0=1.2 D_MAX=1.5}
MORE_THAN={SMAP R_0=0.05 D_0=0.4 A=16 B=8}
ALPHA=27 PHI=-1.5708 THETA=0.61548 PSI=2.35619
... 
cub3: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_c_c_u_b_i_c.html">FCCUBIC</a> ...
SPECIES=1-1152 SWITCH={CUBIC D_0=1.2 D_MAX=1.5}
MORE_THAN={SMAP R_0=0.05 D_0=0.4 A=16 B=8}
ALPHA=27 PHI=1.5708 THETA=-1.29515 PSI=0.785389
... 
cub4: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_c_c_u_b_i_c.html">FCCUBIC</a> ...
SPECIES=1-1152 SWITCH={CUBIC D_0=1.2 D_MAX=1.5}
MORE_THAN={SMAP R_0=0.05 D_0=0.4 A=16 B=8}
ALPHA=27 PHI=-0.2014 THETA=1.84644 PSI=1.71269
... 
cub5: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_c_c_u_b_i_c.html">FCCUBIC</a> ...
SPECIES=1-1152 SWITCH={CUBIC D_0=1.2 D_MAX=1.5}
MORE_THAN={SMAP R_0=0.05 D_0=0.4 A=16 B=8}
ALPHA=27 PHI=-0.61548 THETA=-1.5708 PSI=-0.785398
... 
<span style="color:blue"># The 1153th ghost atom is used as a landmark. These commands allow us to calculate the value of the order parameter in the central slice of the box, in the side regions and in the border slice of the supercell. </span>
<span style="color:blue"># Notice that the sigmoid switching function “SMAP” is tuned in order to facilitate the biasing procedures.</span>
centercub: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_r_o_u_n_d.html">AROUND</a> DATA=cub ATOM=1153 XLOWER=-1.2 XUPPER=1.2 SIGMA=0.5 MORE_THAN={SMAP R_0=0.5 D_0=0.0 A=8 B=8}
sidecub: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_r_o_u_n_d.html">AROUND</a> DATA=cub ATOM=1153 XLOWER=-2.3 XUPPER=2.3 SIGMA=0.5 OUTSIDE LESS_THAN={SMAP R_0=0.5 D_0=-0.1 A=8 B=2}
bordercub: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_r_o_u_n_d.html">AROUND</a> DATA=cub ATOM=1153 XLOWER=-7.0 XUPPER=7.0 SIGMA=0.5 OUTSIDE LESS_THAN={SMAP R_0=0.5 D_0=-0.45 A=8 B=8}
<span style="color:blue"># Well-tempered metadynamics is used to induce transitions between the liquid and the fcc crystal for the region on the side of the supercell. An external history-dependent bias potential is gradually accumulated in the space of the CV </span>
<span style="color:blue"># “sidecub.lessthan”. A Gaussian that should cover the space of 600 timesteps in the CV space is deposited every 1600 time steps, with the maximum height equal to 0.15 Lennard-Jones energy unit. The well-tempered option is activated with </span>
<span style="color:blue"># the biasfactor set to 90. </span>
metad: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
ARG=sidecub.lessthan
PACE=1600 HEIGHT=0.15 SIGMA=600 FILE=HILLS
TEMP=0.60 BIASFACTOR=90
ADAPTIVE=DIFF SIGMA_MAX=50 SIGMA_MIN=0.1
... 
<span style="color:blue"># A restraint is used to keep the central slice of the simulation cell, near to the ghost atom, crystalline.</span>
wall: <a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=centercub.morethan AT=140 KAPPA=2.0
<span style="color:blue"># Several restraints are added to prevent nucleation of crystals with unwanted crystal orientations.</span>
notwin2: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=cub2.morethan AT=14 KAPPA=0.4
notwin3: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=cub3.morethan AT=14 KAPPA=0.2
notwin4: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=cub4.morethan AT=14 KAPPA=0.2
notwin5: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=cub5.morethan AT=14 KAPPA=0.1
<span style="color:blue"># A further bias is added on the atoms at the border of the simulation box far away from the ghost atom, in order to facilitate the nucleation of the melt starting from the edge of the supercell.</span>
softliquid: <a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=bordercub.lessthan AT=30 KAPPA=0.005
<span style="color:blue"># Finally the instantaneous values of the CV and the biases are recorded. These are used in the re-weighting processes to construct the FES</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=10 ARG=cell.ax,cub.*,metad.bias,wall.bias,notwin2.bias,notwin3.bias,notwin4.bias,notwin5.bias,softliquid.bias FILE=FES
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=10 ARG=cub2.*,cub3.*,cub4.*,cub5.*,centercub.*,sidecub.*,sidecub.*,bordercub.*  FILE=COLVAR
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
<span style="color:blue"></span>
</pre>{% endraw %}
