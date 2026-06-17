**Project ID:** [plumID:26.005]({{ '/' | absolute_url }}eggs/26/005/)  
**Source:** plumed_S1_BIN1_BAR.dat  
**Originally used with PLUMED version:** 2.9  
**Stable:** [zipped raw stdout](plumed_S1_BIN1_BAR.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_S1_BIN1_BAR.dat.plumed.stderr.txt.zip) - [stderr](plumed_S1_BIN1_BAR.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed_S1_BIN1_BAR.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_S1_BIN1_BAR.dat.plumed_master.stderr.txt.zip) - [stderr](plumed_S1_BIN1_BAR.dat.plumed_master.stderr)  

{% raw %}
<div class="plumedInputContainer">
<div class="plumedpreheader">
<div class="headerInfo" id="value_details_data/plumed_S1_BIN1_BAR.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div class="containerBadge">
<div class="headerBadge"><a href="plumed_S1_BIN1_BAR.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-passing-green.svg" alt="tested onv2.10" /></a></div>
<div class="headerBadge"><a href="plumed_S1_BIN1_BAR.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></div>
</div>
</div>
<pre class="plumedlisting">
<span style="color:blue" class="comment"># plumed_S1_BIN1_BAR.dat  —  CRYPTAD</span>
<span style="color:blue" class="comment"># WTMetaD for BIN1 BAR homodimer (S1)</span>
<span style="color:blue" class="comment"># 2 CVs: concave-face inter-monomer jaw distance (CV1) + BAR long-axis hinge angle (CV2)</span>
<span style="color:blue" class="comment">#</span>
<span style="color:blue" class="comment"># Confirmed GROMACS atom indices (1-based, Cα):</span>
<span style="color:blue" class="comment">#   CV1 jaw:    A-TYR217 = 2595  |  B-GLU178 = 5230   (ref dist = 4.000 nm)</span>
<span style="color:blue" class="comment">#   CV2 hinge:  A-THR172 = 1974 (tip_A)</span>
<span style="color:blue" class="comment">#               B-ILE146 = 4682 (center / bend vertex)</span>
<span style="color:blue" class="comment">#               B-GLU250 = 6384 (tip_B)</span>
<span style="color:blue" class="comment">#</span>
<span style="color:blue" class="comment"># BEFORE RUNNING:</span>
<span style="color:blue" class="comment">#   1. Verify WHOLEMOLECULES atom range (current estimate: 1–8000 covers the</span>
<span style="color:blue" class="comment">#      BAR dimer protein heavy atoms; solvation atoms come after in CHARMM-GUI</span>
<span style="color:blue" class="comment">#      topologies). Confirm with:</span>
<span style="color:blue" class="comment">#        gmx_mpi dump -s meta.tpr 2&gt;&amp;1 | grep &#x27;natoms&#x27;</span>
<span style="color:blue" class="comment">#      Then adjust ENTITY0=1-N to match the last protein atom.</span>
<span style="color:blue" class="comment">#   2. Compute nc_threshold from last 50 ns of production MD (see TODO below).</span>
<span style="color:blue" class="comment">#   3. Temperature (TEMP=310.15) must match ref_t in meta.mdp.</span>
<span style="color:blue" class="comment">#</span>
<span style="color:blue" class="comment"># Reference: research plan §9 Step 3.3 (v1.3 template)</span>
<br/><span style="color:blue" class="comment"># ── PBC molecule reconstruction ───────────────────────────────────────────────</span>
<span style="color:blue" class="comment"># Covers both BAR chains (A+B, ~430 res × 2 × ~9 heavy atoms = ~7700 atoms)</span>
<span style="color:blue" class="comment"># Adjust upper bound to the actual last protein atom from the topology.</span>
<span class="plumedtooltip" style="color:green">WHOLEMOLECULES<span class="right">This action is used to rebuild molecules that can become split by the periodic boundary conditions. <a href="https://www.plumed.org/doc-master/user-doc/html/WHOLEMOLECULES" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ENTITY0<span class="right">the atoms that make up a molecule that you wish to align<i></i></span></span>=1-8000

<span style="color:blue" class="comment"># ── Biased collective variables ───────────────────────────────────────────────</span>
<br/><span style="color:blue" class="comment"># CV1: inter-monomer concave jaw (A-TYR217 Cα ↔ B-GLU178 Cα)</span>
<span style="color:blue" class="comment"># Selected by geometric concave-face projection opposite to convex centroid.</span>
<span style="display:none;" id="data/plumed_S1_BIN1_BAR.dat">The WHOLEMOLECULES action with label <b></b> calculates something</span><b name="data/plumed_S1_BIN1_BAR.datcv1" onclick='showPath("data/plumed_S1_BIN1_BAR.dat","data/plumed_S1_BIN1_BAR.datcv1","data/plumed_S1_BIN1_BAR.datcv1","brown")'>cv1</b>: <span class="plumedtooltip" style="color:green">DISTANCE<span class="right">Calculate the distance/s between pairs of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/DISTANCE" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS<span class="right">the pair of atom that we are calculating the distance between<i></i></span></span>=2595,5230

<span style="color:blue" class="comment"># CV2: BAR long-axis hinge angle (A-THR172 → B-ILE146 → B-GLU250)</span>
<span style="color:blue" class="comment"># tip_A → center (bend vertex) → tip_B — spans the full ~128 Å long axis.</span>
<span style="color:blue" class="comment"># PLUMED ANGLE order: ATOMS=tip_A,center,tip_B  (same order as IDX_A,IDX_C,IDX_B)</span>
<span style="display:none;" id="data/plumed_S1_BIN1_BAR.datcv1">The DISTANCE action with label <b>cv1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cv1.value</td><td>the DISTANCE between this pair of atoms</td></tr></table></span><b name="data/plumed_S1_BIN1_BAR.datcv2" onclick='showPath("data/plumed_S1_BIN1_BAR.dat","data/plumed_S1_BIN1_BAR.datcv2","data/plumed_S1_BIN1_BAR.datcv2","brown")'>cv2</b>: <span class="plumedtooltip" style="color:green">ANGLE<span class="right">Calculate one or multiple angle/s. <a href="https://www.plumed.org/doc-master/user-doc/html/ANGLE" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS<span class="right">the list of atoms involved in this collective variable (either 3 or 4 atoms)<i></i></span></span>=1974,4682,6384

<span style="color:blue" class="comment"># ── Native contact restraint (unfolding guard) ────────────────────────────────</span>
<span style="color:blue" class="comment"># Keeps the BAR dimer from denaturing under metadynamics bias.</span>
<span style="color:blue" class="comment">#</span>
<span style="color:blue" class="comment"># TODO — required before production run (leave commented for 1 ns test):</span>
<span style="color:blue" class="comment">#   Step 1: Identify stable residue pairs from last 50 ns of production MD:</span>
<span style="color:blue" class="comment">#     python -c &quot;</span>
<span style="color:blue" class="comment">#     import mdtraj as md, numpy as np</span>
<span style="color:blue" class="comment">#     t = md.load(&#x27;prod.xtc&#x27;, top=&#x27;prod.gro&#x27;, stride=10)</span>
<span style="color:blue" class="comment">#     t = t[-250:]  # last 50 ns at 200 ps/frame stride</span>
<span style="color:blue" class="comment">#     # Compute Cα–Cα contact occupancy at 0.8 nm; use mdtraj or MDAnalysis</span>
<span style="color:blue" class="comment">#     &quot;</span>
<span style="color:blue" class="comment">#   Step 2: Exclude residues within 12 Å of pocket centroid (81.84,71.23,74.61)</span>
<span style="color:blue" class="comment">#     → roughly residues A:200-220 and B:160-185 in the BAR concave face.</span>
<span style="color:blue" class="comment">#   Step 3: Exclude tip residues (chain A: &lt;175; chain B: &gt;245 and &lt;152)</span>
<span style="color:blue" class="comment">#     Stable core range estimate: chain A residues 175–215, chain B residues 155–245</span>
<span style="color:blue" class="comment">#     → translate to Cα atom index ranges using gmx_mpi select:</span>
<span style="color:blue" class="comment">#       gmx_mpi select -s meta.tpr -select &#x27;name CA and chain A and resnr &gt;= 175 and resnr &lt;= 215&#x27;</span>
<span style="color:blue" class="comment">#   Step 4: Set AT = 0.80 × nc_mean (20 % safety margin below equilibrium)</span>
<span style="color:blue" class="comment">#   Step 5: Uncomment the nc: and nc_wall: lines below.</span>
<span style="color:blue" class="comment">#</span>
<span style="color:blue" class="comment"># Placeholder (disabled) — fill in GROUPA/GROUPB atom lists from Step 3 above:</span>
<span style="color:blue" class="comment"># nc: COORDINATION ...</span>
<span style="color:blue" class="comment">#   GROUPA=CA_STABLE_ATOMS GROUPB=CA_STABLE_ATOMS</span>
<span style="color:blue" class="comment">#   SWITCH={RATIONAL R_0=0.8 D_MAX=0.8 NN=6 MM=10}</span>
<span style="color:blue" class="comment"># ...</span>
<span style="color:blue" class="comment">#</span>
<span style="color:blue" class="comment"># LOWER_WALLS fires when nc drops below AT (prevents unfolding).</span>
<span style="color:blue" class="comment"># nc_wall: LOWER_WALLS ARG=nc AT=NC_THRESHOLD KAPPA=1000.0 EXP=2 OFFSET=0</span>
<br/><span style="color:blue" class="comment"># ── Well-tempered metadynamics ────────────────────────────────────────────────</span>
<span style="color:blue" class="comment"># T_eff = BIASFACTOR × TEMP = 10 × 310.15 = 3,101.5 K</span>
<span style="color:blue" class="comment"># PACE=500 → deposit Gaussian every 500 × 0.004 ps = 2 ps (HMR dt=0.004)</span>
<span style="display:none;" id="data/plumed_S1_BIN1_BAR.datcv2">The ANGLE action with label <b>cv2</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">cv2.value</td><td>the ANGLE involving these atoms</td></tr></table></span><b name="data/plumed_S1_BIN1_BAR.datmetad" onclick='showPath("data/plumed_S1_BIN1_BAR.dat","data/plumed_S1_BIN1_BAR.datmetad","data/plumed_S1_BIN1_BAR.datmetad","brown")'>metad</b>: <span class="plumedtooltip" style="color:green">METAD<span class="right">Used to performed metadynamics on one or more collective variables. <a href="https://www.plumed.org/doc-master/user-doc/html/METAD" style="color:green">More details</a><i></i></span></span> ...
  <span class="plumedtooltip">ARG<span class="right">the labels of the scalars on which the bias will act<i></i></span></span>=<b name="data/plumed_S1_BIN1_BAR.datcv1">cv1</b>,<b name="data/plumed_S1_BIN1_BAR.datcv2">cv2</b>
  <span class="plumedtooltip">PACE<span class="right">the frequency for hill addition<i></i></span></span>=500
  <span class="plumedtooltip">HEIGHT<span class="right">the heights of the Gaussian hills<i></i></span></span>=1.2
  <span class="plumedtooltip">SIGMA<span class="right">the widths of the Gaussian hills<i></i></span></span>=0.3,0.05
  <span class="plumedtooltip">BIASFACTOR<span class="right">use well tempered metadynamics and use this bias factor<i></i></span></span>=10
  <span class="plumedtooltip">TEMP<span class="right">the system temperature - this is only needed if you are doing well-tempered metadynamics<i></i></span></span>=310.15
  <span class="plumedtooltip">FILE<span class="right"> a file in which the list of added hills is stored<i></i></span></span>=HILLS
  <span class="plumedtooltip">WALKERS_N<span class="right">number of walkers<i></i></span></span>=1
...
<span style="color:blue" class="comment"># For multiple-walker WTMetaD (recommended for BIN1 — §9 Step 3.3):</span>
<span style="color:blue" class="comment">#   Add to each walker&#x27;s METAD block:</span>
<span style="color:blue" class="comment">#     WALKERS_N=2  WALKERS_ID=0   (walker 1)  or  WALKERS_ID=1   (walker 2)</span>
<span style="color:blue" class="comment">#     WALKERS_DIR=./  WALKERS_RSTRIDE=100</span>
<span style="color:blue" class="comment">#   Both walkers share the same HILLS file on Lustre/NFS.</span>
<br/><span style="color:blue" class="comment"># ── Output ────────────────────────────────────────────────────────────────────</span>
<span style="color:blue" class="comment"># STRIDE=500 → write COLVAR every 500 × 0.004 ps = 2 ps</span>
<span style="color:blue" class="comment"># Once nc guard is active, add nc to ARG: ARG=cv1,cv2,nc,metad.bias</span>
<span style="display:none;" id="data/plumed_S1_BIN1_BAR.datmetad">The METAD action with label <b>metad</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">metad.bias</td><td>the instantaneous value of the bias potential</td></tr></table></span><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/PRINT" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=<b name="data/plumed_S1_BIN1_BAR.datcv1">cv1</b>,<b name="data/plumed_S1_BIN1_BAR.datcv2">cv2</b>,<b name="data/plumed_S1_BIN1_BAR.datmetad">metad.bias</b> <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=500 <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=COLVAR

<span style="color:blue" class="comment"># ── Monitoring notes ──────────────────────────────────────────────────────────</span>
<span style="color:blue" class="comment"># 1. After 1 ns test: HILLS and COLVAR files must exist → PLUMED working.</span>
<span style="color:blue" class="comment"># 2. SIGMA tuning: inspect CV1 and CV2 fluctuations in the first ~5 ns</span>
<span style="color:blue" class="comment">#    unbiased COLVAR columns; set SIGMA ~ 1× the thermal fluctuation width.</span>
<span style="color:blue" class="comment">#    If CV1 fluctuates ±0.1 nm → SIGMA=0.1 is sufficient; 0.3 is conservative.</span>
<span style="color:blue" class="comment"># 3. Convergence: run plumed sum_hills --hills HILLS --stride 100 --mintozero</span>
<span style="color:blue" class="comment">#    at t=67, 133, 200 ns; ΔΔF &lt; 1 kJ/mol → converged FES (§9 Step 3.3).</span>
</pre></div>

{% endraw %}
