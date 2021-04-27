**Project ID:** [plumID:19.046]({{ '/' | absolute_url }}eggs/19/046/)  
**Source:** PLUMED_FM/plumed_FM.dat  
**Originally used with PLUMED version:** 2.5-mod  
**Stable:** [raw zipped stdout](plumed_FM.dat.plumed.stdout.txt.zip) - [stderr](plumed_FM.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_FM.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_FM.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">MOLINFO</a> MOLTYPE=protein STRUCTURE=protein.pdb
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=1-3232

lig: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=3233,3236,3237,3240,3241,3243,3245,3247,3249 <span style="color:blue"># you need the COM of your ligand/molecule</span>

fps: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_p_s.html">FPS</a> REFERENCE=Faidon_new_ref.pdb LIGAND=lig ANCHOR=2481 POINTS=-0.5910,0.3486,-1.6694,-0.6214,0.5475,-1.2516
<span style="color:blue">##############################################################################################</span>
<span style="color:blue"># This is the colvar that has inside linepos and linedist (fps.lp and fps.ld, respectively).</span>
<span style="color:blue"># Starting form the obvious, POINTS are the two points A and B to construct the funnel,</span>
<span style="color:blue"># REFERENCE is a pdb file to align the target protein with the frame used to construct</span>
<span style="color:blue"># the funnel. LIGAND must have the label of the COM of the ligand. ANCHOR is one of the</span>
<span style="color:blue"># closest atoms of the protein with respect to the ligand. It's necessary to avoid pbc</span>
<span style="color:blue"># problems.</span>
<span style="color:blue">##############################################################################################</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_f_u_n_n_e_l.html">FUNNEL</a> ARG=fps.lp,fps.ld MINS=-1.0 MAXS=3.5 NBINS=600 ZCC=1.8 ALPHA=0.55 KAPPA=35100 LABEL=funnel
<span style="color:blue">##############################################################################################</span>
<span style="color:blue"># This routine creates the external BIAS of the Funnel. ARG is already set and should</span>
<span style="color:blue"># not be changed. S is the direction along linepos and MINS and MAXS define the maximum</span>
<span style="color:blue"># values that fps.lp can take. ATTENTION: if fps.lp takes a value outside this interval</span>
<span style="color:blue"># during the simulation, the simulation will crash. NBINS and NBINZ (not used here) </span>
<span style="color:blue"># determine the binning of the external BIAS. ZCC and ALPHA regulate the shape and</span>
<span style="color:blue"># position of cone and cylinder. KAPPA is the constant used to evaluate the potential</span>
<span style="color:blue"># in each bin.</span>
<span style="color:blue">############################################################################################## </span>

<span style="color:blue">#METAD ARG=d1 SIGMA=0.01 HEIGHT=2.0 PACE=500 BIASFACTOR=12 TEMP=300 LABEL=metad # Not Funnel related</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=fps.lp AT=3.0 KAPPA=500000.0 EXP=3 OFFSET=0 LABEL=uwall
<span style="color:blue">##############################################################################################</span>
<span style="color:blue"># Here pick a value lower than MAXS, the ligand MUST NOT exit the grid</span>
<span style="color:blue">##############################################################################################</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=fps.lp AT=-0.3 KAPPA=500000.0 EXP=3 OFFSET=0 LABEL=lwall
<span style="color:blue">##############################################################################################</span>
<span style="color:blue"># Here pick a value greater than MINS, the ligand MUST NOT exit the grid</span>
<span style="color:blue">##############################################################################################</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_m_s_d.html">RMSD</a> REFERENCE=pocket.pdb TYPE=OPTIMAL LABEL=rmsd
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=rmsd AT=1.2 KAPPA=500000.0 EXP=3 OFFSET=0 LABEL=rmsdwall <span style="color:blue"># Not Funnel related</span>

rmsdINIT: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_m_s_d.html">RMSD</a> REFERENCE=my_start_meta.pdb TYPE=OPTIMAL
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=rmsdINIT AT=0.09 KAPPA=420000 EXP=2 OFFSET=0 LABEL=rmsdwallINIT 

<span style="color:blue">#####DESCRIPTORS#####</span>
OW: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=3251-47362:3
c1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=2473-2495,2913-2919
c2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=3240
dcm: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=c1,c2
c3: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=2480
c4: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=3236
dsb: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=c3,c4
t: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=2915,2780,3241,3247
w: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=2481,2482,2492,2949 GROUPB=OW  LESS_THAN={RATIONAL R_0=0.4 NN=6 MM=12 D_MAX=0.5}
<a href="https://plumed.github.io/doc-master/user-doc/html/_b_r_i_d_g_e.html">BRIDGE</a> BRIDGING_ATOMS=OW GROUPA=2805 GROUPB=2489 SWITCH={RATIONAL R_0=0.6 D_0=0.0 NN=6 MM=10 D_MAX=4.0} LABEL=wBpock
lig_OW_large: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=3233,3236,3237,3240,3241,3243,3245,3247,3249 GROUPB=OW  LESS_THAN={RATIONAL R_0=0.8 NN=6 MM=12 D_MAX=0.4}

<span style="color:blue">##NORMALIZE DESCRITOPRS##</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=wBpock COEFFICIENTS=0.1538 POWERS=1 LABEL=wBpock_norm PERIODIC=NO
<a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_b_e_t_a.html">ALPHABETA</a> ...
ATOMS1=2915,2780,3241,3247 REFERENCE=1.66
LABEL=ab_t
... <a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_b_e_t_a.html">ALPHABETA</a>
Prot:  <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=3233,3236,3237,3240,3241,3243,3245,3247,3249 GROUPB=1-3232 LESS_THAN={RATIONAL R_0=0.32 NN=6 MM=12}
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=Prot.lessthan COEFFICIENTS=0.012 POWERS=1 LABEL=Prot_norm PERIODIC=NO
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=lig_OW_large.lessthan COEFFICIENTS=0.01351 POWERS=1 LABEL=lig_OW_large_norm PERIODIC=NO
<span style="color:blue">########################</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
 LABEL=metad
 ARG=dsb SIGMA=0.005 HEIGHT=2.1  BIASFACTOR=15 TEMP=300 PACE=250
 GRID_MIN=0 GRID_MAX=5 GRID_BIN=2000
 REWEIGHTING_NGRID=2000
 REWEIGHTING_NHILLS=20
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

rw: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__m_e_t_a_d.html">REWEIGHT_METAD</a> TEMP=300

<span style="color:blue">##Here we some all the bias encountered in the system including restraints+bias on CV##</span>
tbias: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=metad.rbias,funnel.bias,uwall.bias,lwall.bias,rmsdwall.bias,rmsdwallINIT.bias PERIODIC=NO

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=* FILE=COLVAR_FM STRIDE=250
</pre>{% endraw %}
