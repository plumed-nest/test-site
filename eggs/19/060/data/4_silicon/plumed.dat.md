**Project ID:** [plumID:19.060]({{ '/' | absolute_url }}eggs/19/060/)  
**Source:** 4_silicon/plumed.dat  
**Originally used with PLUMED version:** 2.5-mod  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_f_c_v.html">REFCV</a> ...
 SPECIES=1-216
 SIGMA=0.04
 LATTICE_CONSTANTS=0.5431
 CRYSTAL_STRUCTURE=DIAMOND
 LABEL=refcv
 MORE_THAN={RATIONAL R_0=0.5 NN=12 MM=24}
 MEAN
... <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_f_c_v.html">REFCV</a>

ene: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a>

q6: <a href="https://plumed.github.io/doc-master/user-doc/html/_q6.html">Q6</a> SPECIES=1-216 SWITCH={CUBIC D_0=0.235 D_MAX=0.3} LOWMEM VMEAN

<span style="color:blue"># nn bias</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_n_n__v_e_s.html">NN_VES</a> ...
LABEL=nn
ARG=refcv.morethan
NODES=48,24,12
OPTIM=ADAM
ACTIVATION=RELU
GRID_MIN=0.
GRID_MAX=216.
GRID_BIN=500
TEMP=1700.
AVE_STRIDE=500
PRINT_STRIDE=1000
TARGET_STRIDE=1
GAMMA=70
LRATE=0.001
TAU_KL=5000
DECAY=2000
ADAPTIVE_DECAY=0.5
... <a href="https://plumed.github.io/doc-master/user-doc/html/_n_n__v_e_s.html">NN_VES</a>


<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=500  ARG=* FILE=COLVAR


<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
<span style="color:blue"></span>
<span style="color:blue">METAD ...</span>
<span style="color:blue"> ARG=refcv.morethan</span>
<span style="color:blue"> BIASFACTOR=50</span>
<span style="color:blue"> GRID_MIN=-5</span>
<span style="color:blue"> GRID_MAX=220.0</span>
<span style="color:blue"> GRID_BIN=1000</span>
<span style="color:blue"> ADAPTIVE=DIFF</span>
<span style="color:blue"> SIGMA=250</span>
<span style="color:blue"> SIGMA_MIN=0.5</span>
<span style="color:blue"> SIGMA_MAX=20.</span>
<span style="color:blue"> TEMP=1600.</span>
<span style="color:blue"> PACE=500</span>
<span style="color:blue"> LABEL=metad</span>
<span style="color:blue"> HEIGHT=60.</span>
<span style="color:blue"> CALC_RCT</span>
<span style="color:blue">... METAD</span>
<span style="color:blue"><span style="color:blue"># to avoid other structures</span></span>
<span style="color:blue">Q6 SPECIES=1-216 SWITCH={CUBIC D_0=0.235 D_MAX=0.3} VMEAN LABEL=q6</span>
<span style="color:blue"><span style="color:blue">#diff: MATHEVAL ARG=q6.vmean,refcv.mean FUNC=(x-0.035)/(0.42-0.035)-(y-0.34)/(0.85-0.34) PERIODIC=NO</span></span>
<span style="color:blue"><span style="color:blue">#UPPER_WALLS ARG=diff AT=0.15 KAPPA=50000 EXP=2 LABEL=uwall</span></span>
<span style="color:blue"></span>
<span style="color:blue"></span>
</pre>{% endraw %}
