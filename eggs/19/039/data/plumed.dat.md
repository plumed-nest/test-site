**Project ID:** [plumID:19.039]({{ '/' | absolute_url }}eggs/19/039/)  
**Source:** plumed.dat  
**Originally used with PLUMED version:** 2.6-dev  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue">#RESTART</span>

<span style="color:blue"># To be used to force reconstruction of periodic boundary conditions</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=54,75,212,228,239,258,311,328,348,372,383,402,421,463,487,503,519,657,674,690,714,897,914,934,953,964,974,985,1007,1018,1037,1247,1264,1283,1302,1324,1689,1708,1727,1738,1962,1984,1994,2312,2329,2349,2467,2490,2500,2517,2524,2536,2547,2554,2569,2575,2591,2607,2635,2657,2676,2693,2700,2719,2735,2746,2770,2777,2788,2795,2805,2815,2832,2854,2868,2898,2904,2911,2927,2948,2962,2472,3221,3224,3225,3228,3229,3231,3233,3235,3237

d1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=2472,3224
lig: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=3221,3224,3225,3228,3229,3231,3233,3235,3237

<span style="color:blue"># This collective variable has the information of the position of the ligand with respect to the funnel-shape restraint potential. The reference file specified in REFERENCE should contain only the target molecule (no ligand, solvent, ecc.)</span>
fps: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_u_n_n_e_l__p_s.html">FUNNEL_PS</a> LIGAND=lig REFERENCE=start.pdb ANCHOR=2472 POINTS=4.724,5.369,4.069,4.597,5.721,4.343

rmsd: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_m_s_d.html">RMSD</a> REFERENCE=start.pdb TYPE=OPTIMAL

<span style="color:blue"># If not already present, FUNNEL will create the funnel potential and write it to the file specified in FILE</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_f_u_n_n_e_l.html">FUNNEL</a> ARG=fps.lp,fps.ld ZCC=1.8 ALPHA=0.55 RCYL=0.1 MINS=-0.5 MAXS=3.7 KAPPA=35100 NBINS=500 NBINZ=500 FILE=BIAS LABEL=funnel

<span style="color:blue"># remove BIASFACTOR if you want to perform standard metadynamics</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=d1 SIGMA=0.01 HEIGHT=2.0 PACE=500 TEMP=300 BIASFACTOR=20 LABEL=metad GRID_MIN=0.0 GRID_MAX=4.0 GRID_WFILE=grid_w.dat GRID_WSTRIDE=250000

<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=fps.lp AT=-0.3 KAPPA=500000 EXP=2 OFFSET=0 LABEL=lwall
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=rmsd AT=0.09 KAPPA=500000 EXP=2 OFFSET=0 LABEL=uwall-rmsd
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=fps.lp AT=3.4 KAPPA=500000 EXP=2 OFFSET=0 LABEL=uwall
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=d1 AT=3.8 KAPPA=500000 EXP=2 OFFSET=0 LABEL=distwall

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=500 ARG=* FILE=COLVAR
</pre>{% endraw %}
