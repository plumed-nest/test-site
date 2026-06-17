**Project ID:** [plumID:26.005]({{ '/' | absolute_url }}eggs/26/005/)  
**Source:** plumed_S4_CD2AP_SH3-2.dat  
**Originally used with PLUMED version:** 2.9  
**Stable:** [zipped raw stdout](plumed_S4_CD2AP_SH3-2.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_S4_CD2AP_SH3-2.dat.plumed.stderr.txt.zip) - [stderr](plumed_S4_CD2AP_SH3-2.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed_S4_CD2AP_SH3-2.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_S4_CD2AP_SH3-2.dat.plumed_master.stderr.txt.zip) - [stderr](plumed_S4_CD2AP_SH3-2.dat.plumed_master.stderr)  

{% raw %}
<div class="plumedInputContainer">
<div class="plumedpreheader">
<div class="headerInfo" id="value_details_data/plumed_S4_CD2AP_SH3-2.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div class="containerBadge">
<div class="headerBadge"><a href="plumed_S4_CD2AP_SH3-2.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-passing-green.svg" alt="tested onv2.10" /></a></div>
<div class="headerBadge"><a href="plumed_S4_CD2AP_SH3-2.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></div>
</div>
</div>
<pre class="plumedlisting">
<span style="color:blue" class="comment"># plumed_S4_CD2AP_SH3-2.dat  —  CRYPTAD</span>
<span style="color:blue" class="comment"># WTMetaD for CD2AP SH3-2 domain (S4)</span>
<span style="color:blue" class="comment"># 2 CVs: RT-loop flank (Site1) and groove (Site2) jaw distances</span>
<span style="color:blue" class="comment">#</span>
<span style="color:blue" class="comment"># Confirmed GROMACS atom indices (1-based, Cα):</span>
<span style="color:blue" class="comment">#   cv_site1:  GLU-124 = 238  |  LEU-129 = 314   (ref dist = 1.347 nm)</span>
<span style="color:blue" class="comment">#   cv_site2:  LYS-114 =  61  |  TYR-119 = 153   (ref dist = 1.267 nm)</span>
<span style="color:blue" class="comment">#</span>
<span style="color:blue" class="comment"># Note on residue numbering: residues 114–129 use the CD2AP full-protein</span>
<span style="color:blue" class="comment"># sequence numbers. The construct starts at ~residue 109; atom indices are</span>
<span style="color:blue" class="comment"># low (61, 153, 238, 314) because the construct is short (~62 residues).</span>
<span style="color:blue" class="comment">#</span>
<span style="color:blue" class="comment"># BEFORE RUNNING:</span>
<span style="color:blue" class="comment">#   1. Verify WHOLEMOLECULES atom range (estimate: SH3-2 construct ~62 residues</span>
<span style="color:blue" class="comment">#      × ~15 atoms/res ≈ 930 atoms; adjust ENTITY0 upper bound accordingly).</span>
<span style="color:blue" class="comment">#   2. Compute nc_threshold from last 50 ns of production MD.</span>
<br/><span style="color:blue" class="comment"># ── PBC molecule reconstruction ───────────────────────────────────────────────</span>
<span style="color:blue" class="comment"># CD2AP SH3-2 domain construct: ~62 residues × ~15 atoms/res ≈ 930 protein atoms.</span>
<span class="plumedtooltip" style="color:green">WHOLEMOLECULES<span class="right">This action is used to rebuild molecules that can become split by the periodic boundary conditions. <a href="https://www.plumed.org/doc-master/user-doc/html/WHOLEMOLECULES" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ENTITY0<span class="right">the atoms that make up a molecule that you wish to align<i></i></span></span>=1-1000

<span style="color:blue" class="comment"># ── Biased collective variables ───────────────────────────────────────────────</span>
<br/><span style="color:blue" class="comment"># Site1 RT-loop flank jaw (GLU-124 Cα ↔ LEU-129 Cα)</span>
<span style="display:none;" id="data/plumed_S4_CD2AP_SH3-2.dat">The WHOLEMOLECULES action with label <b></b> calculates something</span><b name="data/plumed_S4_CD2AP_SH3-2.datcv_site1" onclick='showPath("data/plumed_S4_CD2AP_SH3-2.dat","data/plumed_S4_CD2AP_SH3-2.datcv_site1","data/plumed_S4_CD2AP_SH3-2.datcv_site1","brown")'>cv_site1</b>: <span class="plumedtooltip" style="color:green">DISTANCE<span class="right">Calculate the distance/s between pairs of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/DISTANCE" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS<span class="right">the pair of atom that we are calculating the distance between<i></i></span></span>=238,314

<span style="color:blue" class="comment"># Site2 groove jaw (LYS-114 Cα ↔ TYR-119 Cα)</span>
<span style="display:none;" id="data/plumed_S4_CD2AP_SH3-2.datcv_site1">The DISTANCE action with label <b>cv_site1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cv_site1.value</td><td>the DISTANCE between this pair of atoms</td></tr></table></span><b name="data/plumed_S4_CD2AP_SH3-2.datcv_site2" onclick='showPath("data/plumed_S4_CD2AP_SH3-2.dat","data/plumed_S4_CD2AP_SH3-2.datcv_site2","data/plumed_S4_CD2AP_SH3-2.datcv_site2","brown")'>cv_site2</b>: <span class="plumedtooltip" style="color:green">DISTANCE<span class="right">Calculate the distance/s between pairs of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/DISTANCE" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS<span class="right">the pair of atom that we are calculating the distance between<i></i></span></span>=61,153

<span style="color:blue" class="comment"># ── Native contact restraint (unfolding guard) ────────────────────────────────</span>
<span style="color:blue" class="comment"># TODO — required before production run (leave commented for 1 ns test):</span>
<span style="color:blue" class="comment">#   Step 1: Compute stable Cα–Cα contacts (&lt;0.8 nm, &gt;80% occupancy)</span>
<span style="color:blue" class="comment">#           from last 50 ns of production MD.</span>
<span style="color:blue" class="comment">#   Step 2: Exclude residues within 12 Å of Site1 centroid (37.0,27.26,30.56)</span>
<span style="color:blue" class="comment">#           (residues ~120–132) and Site2 centroid (28.4,20.88,26.86)</span>
<span style="color:blue" class="comment">#           (residues ~110–122, groove residues — functional interface, EXCLUDE).</span>
<span style="color:blue" class="comment">#   Step 3: Stable core estimate for CD2AP SH3-2: β-barrel core residues</span>
<span style="color:blue" class="comment">#           away from RT-loop (~residues 109–113 and 130–170 in full-protein numbering).</span>
<span style="color:blue" class="comment">#           → translate to Cα atom indices with gmx_mpi select.</span>
<span style="color:blue" class="comment">#   Step 4: AT = 0.80 × nc_mean.  Uncomment below.</span>
<span style="color:blue" class="comment">#</span>
<span style="color:blue" class="comment"># nc: COORDINATION ...</span>
<span style="color:blue" class="comment">#   GROUPA=CA_STABLE GROUPB=CA_STABLE</span>
<span style="color:blue" class="comment">#   SWITCH={RATIONAL R_0=0.8 D_MAX=0.8 NN=6 MM=10}</span>
<span style="color:blue" class="comment"># ...</span>
<span style="color:blue" class="comment"># nc_wall: LOWER_WALLS ARG=nc AT=NC_THRESHOLD KAPPA=1000.0 EXP=2 OFFSET=0</span>
<br/><span style="color:blue" class="comment"># ── Well-tempered metadynamics ────────────────────────────────────────────────</span>
<span style="color:blue" class="comment"># SIGMA=0.1,0.1 nm — SH3 jaw distances ~1.3 nm; tune after 1 ns test.</span>
<span style="color:blue" class="comment"># T_eff = 10 × 310.15 = 3,101.5 K</span>
<span style="color:blue" class="comment"># PACE=500 → 2 ps Gaussian interval (dt=0.004 HMR)</span>
<span style="display:none;" id="data/plumed_S4_CD2AP_SH3-2.datcv_site2">The DISTANCE action with label <b>cv_site2</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cv_site2.value</td><td>the DISTANCE between this pair of atoms</td></tr></table></span><b name="data/plumed_S4_CD2AP_SH3-2.datmetad" onclick='showPath("data/plumed_S4_CD2AP_SH3-2.dat","data/plumed_S4_CD2AP_SH3-2.datmetad","data/plumed_S4_CD2AP_SH3-2.datmetad","brown")'>metad</b>: <span class="plumedtooltip" style="color:green">METAD<span class="right">Used to performed metadynamics on one or more collective variables. <a href="https://www.plumed.org/doc-master/user-doc/html/METAD" style="color:green">More details</a><i></i></span></span> ...
  <span class="plumedtooltip">ARG<span class="right">the labels of the scalars on which the bias will act<i></i></span></span>=<b name="data/plumed_S4_CD2AP_SH3-2.datcv_site1">cv_site1</b>,<b name="data/plumed_S4_CD2AP_SH3-2.datcv_site2">cv_site2</b>
  <span class="plumedtooltip">PACE<span class="right">the frequency for hill addition<i></i></span></span>=500
  <span class="plumedtooltip">HEIGHT<span class="right">the heights of the Gaussian hills<i></i></span></span>=1.2
  <span class="plumedtooltip">SIGMA<span class="right">the widths of the Gaussian hills<i></i></span></span>=0.1,0.1
  <span class="plumedtooltip">BIASFACTOR<span class="right">use well tempered metadynamics and use this bias factor<i></i></span></span>=10
  <span class="plumedtooltip">TEMP<span class="right">the system temperature - this is only needed if you are doing well-tempered metadynamics<i></i></span></span>=310.15
  <span class="plumedtooltip">FILE<span class="right"> a file in which the list of added hills is stored<i></i></span></span>=HILLS
  <span class="plumedtooltip">WALKERS_N<span class="right">number of walkers<i></i></span></span>=1
...
<br/><span style="color:blue" class="comment"># ── Output ────────────────────────────────────────────────────────────────────</span>
<span style="display:none;" id="data/plumed_S4_CD2AP_SH3-2.datmetad">The METAD action with label <b>metad</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">metad.bias</td><td>the instantaneous value of the bias potential</td></tr></table></span><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/PRINT" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=<b name="data/plumed_S4_CD2AP_SH3-2.datcv_site1">cv_site1</b>,<b name="data/plumed_S4_CD2AP_SH3-2.datcv_site2">cv_site2</b>,<b name="data/plumed_S4_CD2AP_SH3-2.datmetad">metad.bias</b> <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=500 <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=COLVAR
</pre></div>

{% endraw %}
