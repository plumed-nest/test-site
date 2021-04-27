**Project ID:** [plumID:20.009]({{ '/' | absolute_url }}eggs/20/009/)  
**Source:** Ub4/plumed-cv.dat  
**Originally used with PLUMED version:** 2.6  
**Stable:** [raw zipped stdout](plumed-cv.dat.plumed.stdout.txt.zip) - [stderr](plumed-cv.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed-cv.dat.plumed_master.stdout.txt.zip) - [stderr](plumed-cv.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">MOLINFO</a> STRUCTURE=template.pdb

<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=1-652

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
<span style="color:blue">#ubi4</span>
e: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=490,492,494,496,500,502,505,507,509,511,512,515,517,519,521,523,525,527,529,531,533,535,537,539,541,543,545,548,549,552,554,556,558,561,563,564,566,568,570,572,574,576,579,581,583,587,588,589,592,594,596,598,600,601,604,606,608,610,612,616,618,620,622,625,627,629,631,633,637,639 NOPBC
e1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=490,492,494,496,500,502,505,507,509,511,512,515,517,519,521,523,525,527,529,531,533,535,537,539,541,543,545,548,549,552,554,556,558,561,563,564 NOPBC
e2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=566,568,570,572,574,576,579,581,583,587,588,589,592,594,596,598,600,601,604,606,608,610,612,616,618,620,622,625,627,629,631,633,637,639 NOPBC

<span style="color:blue"># distance between ubiquitins </span>
d1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=a,b NOPBC
d2: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=a,c NOPBC
d3: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=a,e NOPBC
d4: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=b,c NOPBC
d5: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=b,e NOPBC
d6: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=c,e NOPBC


<span style="color:blue">#relativ orientation</span>
tor1: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=a1,a2,b1,b2 NOPBC
tor2: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=a1,a2,c1,c2 NOPBC
tor3: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=a1,a2,e1,e2 NOPBC
tor4: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=b1,b2,c1,c2 NOPBC
tor5: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=b1,b2,e1,e2 NOPBC
tor6: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=c1,c2,e1,e2 NOPBC

<span style="color:blue">#global radius</span>

rg: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_y_r_a_t_i_o_n.html">GYRATION</a> ATOMS=1,3,5,7,11,13,16,18,20,22,23,26,28,30,32,34,36,38,40,42,44,46,48,50,52,54,56,59,60,63,65,67,69,72,74,75,77,79,81,83,85,87,90,92,94,98,99,100,103,105,107,109,111,112,115,117,119,121,123,127,129,131,133,136,138,140,142,144,148,150,152,154,157,159,162,163,164,166,168,170,174,176,179,181,183,185,186,189,191,193,195,197,199,201,203,205,207,209,211,213,215,217,219,222,223,226,228,230,232,235,237,238,240,242,244,246,248,250,253,255,257,261,262,263,266,268,270,272,274,275,278,280,282,284,286,290,292,294,296,299,301,303,305,307,311,313,315,317,320,322,325,326,327,329,331,333,337,339,342,344,346,348,349,352,354,356,358,360,362,364,366,368,370,372,374,376,378,380,382,385,386,389,391,393,395,398,400,401,403,405,407,409,411,413,416,418,420,424,425,426,429,431,433,435,437,438,441,443,445,447,449,453,455,457,459,462,464,466,468,470,474,476,478,480,483,485,488,489,490,492,494,496,500,502,505,507,509,511,512,515,517,519,521,523,525,527,529,531,533,535,537,539,541,543,545,548,549,552,554,556,558,561,563,564,566,568,570,572,574,576,579,581,583,587,588,589,592,594,596,598,600,601,604,606,608,610,612,616,618,620,622,625,627,629,631,633,637,639,641,643,646,648,651,652 NOPBC

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

<a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_b_e_t_a.html">ALPHABETA</a> ...
LABEL=linktor3
REFERENCE=0
ATOMS1=476,478,480,483
ATOMS2=478,480,483,485
ATOMS3=480,483,485,488
ATOMS4=483,485,488,489
ATOMS5=485,488,489,490
ATOMS6=488,489,490,492
... <a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_b_e_t_a.html">ALPHABETA</a>


<a href="https://plumed.github.io/doc-master/user-doc/html/_s_a_x_s.html">SAXS</a> ...
LABEL=test2
ATOMS=1-652
NOPBC

MARTINI

QVALUE1=0.02
QVALUE2=0.03
QVALUE3=0.04
QVALUE4=0.05
QVALUE5=0.06
QVALUE6=0.07
QVALUE7=0.08
QVALUE8=0.09
QVALUE9=0.1
QVALUE10=0.11
QVALUE11=0.12
QVALUE12=0.13
QVALUE13=0.14
QVALUE14=0.15
QVALUE15=0.16
QVALUE16=0.17
QVALUE17=0.18
QVALUE18=0.19
QVALUE19=0.2
QVALUE20=0.21

 EXPINT1=5.24833
 EXPINT2=4.39027
 EXPINT3=3.50363
 EXPINT4=2.70379
 EXPINT5=2.07676
 EXPINT6=1.62809
 EXPINT7=1.31061
 EXPINT8=1.07411
 EXPINT9=0.887992
EXPINT10=0.738255
EXPINT11=0.617356
EXPINT12=0.518766
EXPINT13=0.436834
EXPINT14=0.367909
EXPINT15=0.310039
EXPINT16=0.261567
EXPINT17=0.220234
EXPINT18=0.183526
EXPINT19=0.149622
EXPINT20=0.117966
... <a href="https://plumed.github.io/doc-master/user-doc/html/_s_a_x_s.html">SAXS</a>

lsaxs: <a href="https://plumed.github.io/doc-master/user-doc/html/_s_t_a_t_s.html">STATS</a> ARG=(test2\.q-.*) PARARG=(test2\.exp-.*)


<a href="https://plumed.github.io/doc-master/user-doc/html/_p_b_m_e_t_a_d.html">PBMETAD</a> ...
LABEL=bias
ARG=d1,d2,d3,d4,d5,d6,linktor1,linktor2,linktor3,rg,tor1,tor2,tor3,tor4,tor5,tor6
HEIGHT=0.075
PACE=200
BIASFACTOR=40
ADAPTIVE=DIFF
GRID_WFILES=GRID.0,GRID.1,GRID.2,GRID.3,GRID.4,GRID.5,GRID.6,GRID.7,GRID.8,GRID.9,GRID.10,GRID.11,GRID.12,GRID.13,GRID.14,GRID.15
GRID_WSTRIDE=2000
<span style="color:blue">#GRID_RFILES=GRID.0,GRID.1,GRID.2,GRID.3,GRID.4,GRID.5,GRID.6,GRID.7,GRID.8,GRID.9,GRID.10,GRID.11,GRID.12,GRID.13,GRID.14,GRID.15</span>
SIGMA=1000
SIGMA_MIN=0.005,0.005,0.005,0.005,0.005,0.005,0.005,0.005,0.005,0.005,0.005,0.005,0.005,0.005,0.005,0.005
SIGMA_MAX=0.2,0.2,0.2,0.2,0.2,0.2,0.2,0.2,0.2,0.2,0.2,0.2,0.2,0.2,0.2,0.2

GRID_MIN=0,0,0,0,0,0,0,0,0,0,-pi,-pi,-pi,-pi,-pi,-pi
GRID_MAX=7,14,18,7,14,7,6,6,6,7,pi,pi,pi,pi,pi,pi

WALKERS_MPI
UPDATE_FROM=2000
... <a href="https://plumed.github.io/doc-master/user-doc/html/_p_b_m_e_t_a_d.html">PBMETAD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_i_n_f_e_r_e_n_c_e.html">METAINFERENCE</a> ...
SCALEDATA
NOISETYPE=MOUTLIERS
AVERAGING=100
ARG=(test2\.q-.*),bias.bias REWEIGHT PARARG=(test2\.exp-.*)
SCALE_PRIOR=FLAT
ADDOFFSET
OFFSET_PRIOR=FLAT
OFFSET0=0 OFFSET_MIN=-10 OFFSET_MAX=10 DOFFSET=0.01
SCALE0=1.00 SCALE_MIN=0.8 SCALE_MAX=1.2 DSCALE=0.001
SIGMA0=0.01 SIGMA_MIN=0. SIGMA_MAX=0.05
OPTSIGMAMEAN=SEM
LABEL=bq
WRITE_STRIDE=10000
STRIDE=5
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_i_n_f_e_r_e_n_c_e.html">METAINFERENCE</a>


ensaxs: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_s_e_m_b_l_e.html">ENSEMBLE</a> ARG=(test2\.q-.*),bias.bias REWEIGHT
statsq: <a href="https://plumed.github.io/doc-master/user-doc/html/_s_t_a_t_s.html">STATS</a> ARG=(ensaxs\.test2\.q-.*) PARARG=(test2\.exp-.*)



<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=1000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=(test2\.q-.*),(test2\.exp-.*) FILE=CV.dat STRIDE=100
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FILE=RESTRAINTS ARG=bq.* STRIDE=100
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FILE=q.dat ARG=statsq.*,lsaxs.* STRIDE=100
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FILE=Analyse.dat ARG=d1,d2,d3,d4,d5,d6,linktor1,linktor2,linktor3,rg,tor1,tor2,tor3,tor4,tor5,tor6 STRIDE=100
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FILE=ENSAXS ARG=(ensaxs\.test2\.q-.*) STRIDE=100

enANA: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_s_e_m_b_l_e.html">ENSEMBLE</a> ARG=d1,d2,d3,d4,d5,d6,linktor1,linktor2,linktor3,rg,tor1,tor2,tor3,tor4,tor5,tor6,bias.bias REWEIGHT
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FILE=ENANA ARG=enANA.* STRIDE=100



</pre>{% endraw %}
