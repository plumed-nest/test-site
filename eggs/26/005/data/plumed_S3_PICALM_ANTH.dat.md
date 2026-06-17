**Project ID:** [plumID:26.005]({{ '/' | absolute_url }}eggs/26/005/)  
**Source:** plumed_S3_PICALM_ANTH.dat  
**Originally used with PLUMED version:** 2.9  
**Stable:** [zipped raw stdout](plumed_S3_PICALM_ANTH.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_S3_PICALM_ANTH.dat.plumed.stderr.txt.zip) - [stderr](plumed_S3_PICALM_ANTH.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed_S3_PICALM_ANTH.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_S3_PICALM_ANTH.dat.plumed_master.stderr.txt.zip) - [stderr](plumed_S3_PICALM_ANTH.dat.plumed_master.stderr)  

{% raw %}
<div class="plumedInputContainer">
<div class="plumedpreheader">
<div class="headerInfo" id="value_details_data/plumed_S3_PICALM_ANTH.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div class="containerBadge">
<div class="headerBadge"><a href="plumed_S3_PICALM_ANTH.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-passing-green.svg" alt="tested onv2.10" /></a></div>
<div class="headerBadge"><a href="plumed_S3_PICALM_ANTH.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></div>
</div>
</div>
<pre class="plumedlisting">
<span style="color:blue" class="comment"># plumed_S3_PICALM_ANTH.dat  —  CRYPTAD</span>
<span style="color:blue" class="comment"># WTMetaD for PICALM ANTH domain (S3)</span>
<span style="color:blue" class="comment"># 2 CVs: PI(4,5)P2-loop face pocket jaw distances for Site1 and Site4</span>
<span style="color:blue" class="comment">#</span>
<span style="color:blue" class="comment"># Confirmed GROMACS atom indices (1-based, Cα):</span>
<span style="color:blue" class="comment">#   cv_site1:  LEU-131 = 1822  |  ARG-139 = 1950   (ref dist = 1.234 nm)</span>
<span style="color:blue" class="comment">#   cv_site4:  ASP-203 = 2979  |  SER-248 = 3753   (ref dist = 1.544 nm)</span>
<span style="color:blue" class="comment">#</span>
<span style="color:blue" class="comment"># BEFORE RUNNING:</span>
<span style="color:blue" class="comment">#   1. Verify WHOLEMOLECULES atom range (estimate: ANTH domain ~270 residues</span>
<span style="color:blue" class="comment">#      × ~15 atoms/res ≈ 4050 protein atoms; adjust ENTITY0 upper bound).</span>
<span style="color:blue" class="comment">#   2. Compute nc_threshold from last 50 ns of production MD (see TODO below).</span>
<br/><span style="color:blue" class="comment"># ── PBC molecule reconstruction ───────────────────────────────────────────────</span>
<span style="color:blue" class="comment"># PICALM ANTH domain ~270 residues × 15 atoms/res ≈ 4050 protein atoms.</span>
<span class="plumedtooltip" style="color:green">WHOLEMOLECULES<span class="right">This action is used to rebuild molecules that can become split by the periodic boundary conditions. <a href="https://www.plumed.org/doc-master/user-doc/html/WHOLEMOLECULES" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ENTITY0<span class="right">the atoms that make up a molecule that you wish to align<i></i></span></span>=1-4500

<span style="color:blue" class="comment"># ── Biased collective variables ───────────────────────────────────────────────</span>
<br/><span style="color:blue" class="comment"># Site1 PIP2-loop face jaw (LEU-131 Cα ↔ ARG-139 Cα)</span>
<span style="display:none;" id="data/plumed_S3_PICALM_ANTH.dat">The WHOLEMOLECULES action with label <b></b> calculates something</span><b name="data/plumed_S3_PICALM_ANTH.datcv_site1" onclick='showPath("data/plumed_S3_PICALM_ANTH.dat","data/plumed_S3_PICALM_ANTH.datcv_site1","data/plumed_S3_PICALM_ANTH.datcv_site1","brown")'>cv_site1</b>: <span class="plumedtooltip" style="color:green">DISTANCE<span class="right">Calculate the distance/s between pairs of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/DISTANCE" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS<span class="right">the pair of atom that we are calculating the distance between<i></i></span></span>=1822,1950

<span style="color:blue" class="comment"># Site4 PIP2-loop face jaw (ASP-203 Cα ↔ SER-248 Cα)</span>
<span style="display:none;" id="data/plumed_S3_PICALM_ANTH.datcv_site1">The DISTANCE action with label <b>cv_site1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cv_site1.value</td><td>the DISTANCE between this pair of atoms</td></tr></table></span><b name="data/plumed_S3_PICALM_ANTH.datcv_site4" onclick='showPath("data/plumed_S3_PICALM_ANTH.dat","data/plumed_S3_PICALM_ANTH.datcv_site4","data/plumed_S3_PICALM_ANTH.datcv_site4","brown")'>cv_site4</b>: <span class="plumedtooltip" style="color:green">DISTANCE<span class="right">Calculate the distance/s between pairs of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/DISTANCE" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS<span class="right">the pair of atom that we are calculating the distance between<i></i></span></span>=2979,3753

<span style="color:blue" class="comment"># ── Native contact restraint (unfolding guard) ────────────────────────────────</span>
<span style="color:blue" class="comment"># TODO — required before production run (leave commented for 1 ns test):</span>
<span style="color:blue" class="comment">#   Step 1: Compute stable Cα–Cα contact pairs (&lt;0.8 nm, &gt;80% occupancy)</span>
<span style="color:blue" class="comment">#           from last 50 ns of production MD.</span>
<span style="color:blue" class="comment">#   Step 2: Exclude residues within 12 Å of Site1 centroid (41.26,42.15,42.59)</span>
<span style="color:blue" class="comment">#           (residues ~125–145) and Site4 centroid (49.25,55.70,53.12)</span>
<span style="color:blue" class="comment">#           (residues ~195–255, PIP2-binding loop region — functional interface,</span>
<span style="color:blue" class="comment">#           EXCLUDE per §9 rule c: these are expected to move under bias).</span>
<span style="color:blue" class="comment">#   Step 3: Stable core estimate for PICALM ANTH: residues away from PIP2 loop,</span>
<span style="color:blue" class="comment">#           roughly residues 1–120 and 160–195.</span>
<span style="color:blue" class="comment">#           → translate to Cα atom indices with gmx_mpi select.</span>
<span style="color:blue" class="comment">#   Step 4: AT = 0.80 × nc_mean.  Uncomment below.</span>
<span style="color:blue" class="comment">#</span>
<span style="color:blue" class="comment"># nc: COORDINATION ...</span>
<span style="color:blue" class="comment">#   GROUPA=CA_STABLE GROUPB=CA_STABLE</span>
<span style="color:blue" class="comment">#   SWITCH={RATIONAL R_0=0.8 D_MAX=0.8 NN=6 MM=10}</span>
<span style="color:blue" class="comment"># ...</span>
<span style="color:blue" class="comment"># nc_wall: LOWER_WALLS ARG=nc AT=NC_THRESHOLD KAPPA=1000.0 EXP=2 OFFSET=0</span>
<br/><span style="color:blue" class="comment"># ── Well-tempered metadynamics ────────────────────────────────────────────────</span>
<span style="color:blue" class="comment"># SIGMA=0.1,0.1 nm — tuned for ANTH jaw distances ~1.2–1.5 nm;</span>
<span style="color:blue" class="comment">#   cv_site4 ref dist = 1.544 nm; consider SIGMA=0.1,0.15 after 1 ns test.</span>
<span style="color:blue" class="comment"># T_eff = 10 × 310.15 = 3,101.5 K</span>
<span style="color:blue" class="comment"># PACE=500 → 2 ps Gaussian interval (dt=0.004 HMR)</span>
<span style="color:blue" class="comment">#</span>
<span style="color:blue" class="comment"># Multiple-walker WTMetaD recommended for PICALM (larger domain, §9 Step 3.3):</span>
<span style="color:blue" class="comment">#   Add WALKERS_N=2 WALKERS_ID=0/1 WALKERS_DIR=./ WALKERS_RSTRIDE=100</span>
<span style="color:blue" class="comment">#   to both walkers&#x27; METAD blocks.</span>
<span style="display:none;" id="data/plumed_S3_PICALM_ANTH.datcv_site4">The DISTANCE action with label <b>cv_site4</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cv_site4.value</td><td>the DISTANCE between this pair of atoms</td></tr></table></span><b name="data/plumed_S3_PICALM_ANTH.datmetad" onclick='showPath("data/plumed_S3_PICALM_ANTH.dat","data/plumed_S3_PICALM_ANTH.datmetad","data/plumed_S3_PICALM_ANTH.datmetad","brown")'>metad</b>: <span class="plumedtooltip" style="color:green">METAD<span class="right">Used to performed metadynamics on one or more collective variables. <a href="https://www.plumed.org/doc-master/user-doc/html/METAD" style="color:green">More details</a><i></i></span></span> ...
  <span class="plumedtooltip">ARG<span class="right">the labels of the scalars on which the bias will act<i></i></span></span>=<b name="data/plumed_S3_PICALM_ANTH.datcv_site1">cv_site1</b>,<b name="data/plumed_S3_PICALM_ANTH.datcv_site4">cv_site4</b>
  <span class="plumedtooltip">PACE<span class="right">the frequency for hill addition<i></i></span></span>=500
  <span class="plumedtooltip">HEIGHT<span class="right">the heights of the Gaussian hills<i></i></span></span>=1.2
  <span class="plumedtooltip">SIGMA<span class="right">the widths of the Gaussian hills<i></i></span></span>=0.1,0.1
  <span class="plumedtooltip">BIASFACTOR<span class="right">use well tempered metadynamics and use this bias factor<i></i></span></span>=10
  <span class="plumedtooltip">TEMP<span class="right">the system temperature - this is only needed if you are doing well-tempered metadynamics<i></i></span></span>=310.15
  <span class="plumedtooltip">FILE<span class="right"> a file in which the list of added hills is stored<i></i></span></span>=HILLS
  <span class="plumedtooltip">WALKERS_N<span class="right">number of walkers<i></i></span></span>=1
...
<br/><span style="color:blue" class="comment"># ── Output ────────────────────────────────────────────────────────────────────</span>
<span style="display:none;" id="data/plumed_S3_PICALM_ANTH.datmetad">The METAD action with label <b>metad</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">metad.bias</td><td>the instantaneous value of the bias potential</td></tr></table></span><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/PRINT" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=<b name="data/plumed_S3_PICALM_ANTH.datcv_site1">cv_site1</b>,<b name="data/plumed_S3_PICALM_ANTH.datcv_site4">cv_site4</b>,<b name="data/plumed_S3_PICALM_ANTH.datmetad">metad.bias</b> <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=500 <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=COLVAR
</pre></div>

{% endraw %}
