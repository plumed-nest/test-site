**Project ID:** [plumID:20.009]({{ '/' | absolute_url }}eggs/20/009/)  
**Source:** Ub3/plumed-cv.dat  
**Originally used with PLUMED version:** 2.6  
**Stable:** [raw zipped stdout](plumed-cv.dat.plumed.stdout.txt.zip) - [stderr](plumed-cv.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed-cv.dat.plumed_master.stdout.txt.zip) - [stderr](plumed-cv.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">MOLINFO</a> STRUCTURE=template.pdb

<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=1-489

<span style="color:blue">#ubi1</span>
a: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1,3,5,7,11,13,16,18,20,22,23,26,28,30,32,34,36,38,40,42,44,46,48,50,52,54,56,59,60,63,65,67,69,72,74,75,77,79,81,83,85,87,90,92,94,98,99,100,103,105,107,109,111,112,115,117,119,121,123,127,129,131,133,136,138,140,142,144,148,150 NOPBC
a1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1,3,5,7,11,13,16,18,20,22,23,26,28,30,32,34,36,38,40,42,44,46,48,50,52,54,56,59,60,63,65,67,69,72,74,75 NOPBC
a2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=77,79,81,83,85,87,90,92,94,98,99,100,103,105,107,109,111,112,115,117,119,121,123,127,129,131,133,136,138,140,142,144,148,150 NOPBC
<span style="color:blue">#ubi2</span>
b: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=164,166,168,170,174,176,179,181,183,185,186,189,191,193,195,197,199,201,203,205,207,209,211,213,215,217,219,222,223,226,228,230,232,235,237,238,240,242,244,246,248,250,253,255,257,261,262,263,266,268,270,272,274,275,278,280,282,284,286,290,292,294,296,299,301,303,305,307,311,313 NOPBC
b1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=164,166,168,170,174,176,179,181,183,185,186,189,191,193,195,197,199,201,203,205,207,209,211,213,215,217,219,222,223,226,228,230,232,235,237,238 NOPBC
b2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=,240,242,244,246,248,250,253,255,257,261,262,263,266,268,270,272,274,275,278,280,282,284,286,290,292,294,296,299,301,303,305,307,311,313 NOPBC
<span style="color:blue">#ubi3</span>
c: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=327,329,331,333,337,339,342,344,346,348,349,352,354,356,358,360,362,364,366,368,370,372,374,376,378,380,382,385,386,389,391,393,395,398,400,401,403,405,407,409,411,413,416,418,420,424,425,426,429,431,433,435,437,438,441,443,445,447,449,453,455,457,459,462,464,466,468,470,474,476 NOPBC
c1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=327,329,331,333,337,339,342,344,346,348,349,352,354,356,358,360,362,364,366,368,370,372,374,376,378,380,382,385,386,389,391,393,395,398,400,401 NOPBC
c2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=403,405,407,409,411,413,416,418,420,424,425,426,429,431,433,435,437,438,441,443,445,447,449,453,455,457,459,462,464,466,468,470,474,476 NOPBC

<span style="color:blue"># distance between ubiquitins </span>
d1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=a,b NOPBC
d2: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=a,c NOPBC
d3: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=b,c NOPBC
<span style="color:blue">#relativ orientation</span>
tor1: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=a1,a2,b1,b2 NOPBC
tor2: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=a1,a2,c1,c2 NOPBC
tor3: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=b1,b2,c1,c2 NOPBC

<span style="color:blue">#global radius</span>
rg: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_y_r_a_t_i_o_n.html">GYRATION</a> ATOMS=1,3,5,7,11,13,16,18,20,22,23,26,28,30,32,34,36,38,40,42,44,46,48,50,52,54,56,59,60,63,65,67,69,72,74,75,77,79,81,83,85,87,90,92,94,98,99,100,103,105,107,109,111,112,115,117,119,121,123,127,129,131,133,136,138,140,142,144,148,150,152,154,157,159,162,163,164,166,168,170,174,176,179,181,183,185,186,189,191,193,195,197,199,201,203,205,207,209,211,213,215,217,219,222,223,226,228,230,232,235,237,238,240,242,244,246,248,250,253,255,257,261,262,263,266,268,270,272,274,275,278,280,282,284,286,290,292,294,296,299,301,303,305,307,311,313,315,317,320,322,325,326,327,329,331,333,337,339,342,344,346,348,349,352,354,356,358,360,362,364,366,368,370,372,374,376,378,380,382,385,386,389,391,393,395,398,400,401,403,405,407,409,411,413,416,418,420,424,425,426,429,431,433,435,437,438,441,443,445,447,449,453,455,457,459,462,464,466,468,470,474,476,478,480,483,485,488,489 NOPBC

<span style="color:blue">#linker angle</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_b_e_t_a.html">ALPHABETA</a> ...
LABEL=linktor1
REFERENCE=0
ATOMS1=150,152,154,157
ATOMS2=152,154,157,159
ATOMS3=154,157,159,162
ATOMS4=157,159,162,163
ATOMS5=159,162,163,164
ATOMS6=162,163,164,166
... <a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_b_e_t_a.html">ALPHABETA</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_b_e_t_a.html">ALPHABETA</a> ...
LABEL=linktor2
REFERENCE=0
ATOMS1=313,315,317,320
ATOMS2=315,317,320,322
ATOMS3=317,320,322,325
ATOMS4=320,322,325,326
ATOMS5=322,325,326,327
ATOMS6=325,326,327,329
... <a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_b_e_t_a.html">ALPHABETA</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_s_a_x_s.html">SAXS</a> ...
LABEL=test2
ATOMS=1-489
NOPBC

MARTINI

QVALUE1=0.0178612
QVALUE2=0.029015
QVALUE3=0.0401689
QVALUE4=0.0513227
QVALUE5=0.0624766
QVALUE6=0.0736304
QVALUE7=0.0847843
QVALUE8=0.0959381
QVALUE9=0.107092
QVALUE10=0.118246
QVALUE11=0.129399
QVALUE12=0.140553
QVALUE13=0.151707
QVALUE14=0.162861
QVALUE15=0.174015
QVALUE16=0.185169
QVALUE17=0.196323
QVALUE18=0.207476
QVALUE19=0.21863
QVALUE20=0.229784
QVALUE21=0.240938


EXPINT1=4.68143
EXPINT2=4.11699
EXPINT3=3.45783
EXPINT4=2.76077
EXPINT5=2.15094
EXPINT6=1.67643
EXPINT7=1.32305
EXPINT8=1.06339
EXPINT9=0.870742
EXPINT10=0.721004
EXPINT11=0.597613
EXPINT12=0.493722
EXPINT13=0.407671
EXPINT14=0.337263
EXPINT15=0.27869
EXPINT16=0.228546
EXPINT17=0.184443
EXPINT18=0.144056
EXPINT19=0.106039
EXPINT20=0.0725692
EXPINT21=0.0480033

... <a href="https://plumed.github.io/doc-master/user-doc/html/_s_a_x_s.html">SAXS</a>

lsaxs: <a href="https://plumed.github.io/doc-master/user-doc/html/_s_t_a_t_s.html">STATS</a> ARG=(test2\.q-.*) PARARG=(test2\.exp-.*)


<a href="https://plumed.github.io/doc-master/user-doc/html/_p_b_m_e_t_a_d.html">PBMETAD</a> ...
LABEL=bias
ARG=d1,d2,d3,tor1,tor2,tor3,rg,linktor1,linktor2
HEIGHT=0.1
PACE=200
BIASFACTOR=30
ADAPTIVE=DIFF
GRID_WFILES=GRID.0,GRID.1,GRID.2,GRID.3,GRID.4,GRID.5,GRID.6,GRID.7,GRID.8
GRID_WSTRIDE=2000
<span style="color:blue">#GRID_RFILES=GRID.0,GRID.1,GRID.2,GRID.3,GRID.4,GRID.5,GRID.6,GRID.7,GRID.8</span>
SIGMA=10000
SIGMA_MIN=0.005,0.005,0.005,0.005,0.005,0.005,0.005,0.005,0.005
SIGMA_MAX=0.2,0.2,0.2,0.2,0.2,0.2,0.2,0.2,0.2

GRID_MIN=0,0,0,-pi,-pi,-pi,0,0,0
GRID_MAX=7,14,7,pi,pi,pi,7,6,6

WALKERS_MPI
UPDATE_FROM=10000
... <a href="https://plumed.github.io/doc-master/user-doc/html/_p_b_m_e_t_a_d.html">PBMETAD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_i_n_f_e_r_e_n_c_e.html">METAINFERENCE</a> ...
SCALEDATA
AVERAGING=100
NOISETYPE=MOUTLIERS
ARG=(test2\.q-.*),bias.bias REWEIGHT PARARG=(test2\.exp-.*)
SCALE_PRIOR=FLAT
ADDOFFSET
OFFSET_PRIOR=FLAT
OFFSET0=0 OFFSET_MIN=-10 OFFSET_MAX=10 DOFFSET=0.005
SCALE0=1.00 SCALE_MIN=0.8 SCALE_MAX=1.2 DSCALE=0.001
SIGMA0=0.01 SIGMA_MIN=0. SIGMA_MAX=0.05
OPTSIGMAMEAN=SEM
LABEL=bq
WRITE_STRIDE=10000
STRIDE=5
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_i_n_f_e_r_e_n_c_e.html">METAINFERENCE</a>

ensaxs: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_s_e_m_b_l_e.html">ENSEMBLE</a> ARG=(test2\.q-.*),bias.bias REWEIGHT
statsq: <a href="https://plumed.github.io/doc-master/user-doc/html/_s_t_a_t_s.html">STATS</a> ARG=(ensaxs\.test2\.q-.*) PARARG=(test2\.exp-.*)
enANA: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_s_e_m_b_l_e.html">ENSEMBLE</a> ARG=d1,d2,d3,tor1,tor2,tor3,rg,linktor1,linktor2,bias.bias REWEIGHT

<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=1000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=(test2\.q-.*),(test2\.exp-.*) FILE=CV.dat STRIDE=100
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FILE=RESTRAINTS ARG=bq.* STRIDE=100
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FILE=q.dat ARG=statsq.*,lsaxs.* STRIDE=100
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FILE=Analyse.dat ARG=d1,d2,d3,tor1,tor2,tor3,rg,linktor1,linktor2 STRIDE=100
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FILE=ENSAXS ARG=(ensaxs\.test2\.q-.*) STRIDE=100
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FILE=ENANA ARG=enANA.* STRIDE=100

</pre>{% endraw %}
