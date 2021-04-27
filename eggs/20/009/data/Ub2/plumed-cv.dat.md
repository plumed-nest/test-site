**Project ID:** [plumID:20.009]({{ '/' | absolute_url }}eggs/20/009/)  
**Source:** Ub2/plumed-cv.dat  
**Originally used with PLUMED version:** 2.6  
**Stable:** [raw zipped stdout](plumed-cv.dat.plumed.stdout.txt.zip) - [stderr](plumed-cv.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed-cv.dat.plumed_master.stdout.txt.zip) - [stderr](plumed-cv.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">MOLINFO</a> STRUCTURE=template.pdb

<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=1-355

a: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=31,32,34,36,40,42,45,47,49,51,52,55,57,59,61,63,65,67,69,71,73,75,77,79,81,83,85,88,89,92,94,96,98,101,103,104,106,108,110,112,114,116,119,121,123,127,128,129,132,134,136,138,140,141,144,146,148,150,152,156,158,160,162,167,169,171,173,177,179 NOPBC
b: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=193,195,197,199,203,205,208,210,212,214,215,218,220,222,224,226,228,230,232,234,236,238,240,242,244,246,248,251,252,255,257,259,261,264,266,267,269,271,273,275,277,279,282,284,286,290,291,292,295,297,299,301,303,304,307,309,311,313,315,319,321,323,325,328,330,332,334,336,340,342 NOPBC

<span style="color:blue">#Centers in ubiquitin</span>
a1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=31,32,34,36,40,42,45,47,49,51,52,55,57,59,61,63,65,67,69,71,73,75,77,79,81,83,85,88,89,92,94,96,98,101,103,104 NOPBC
a2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=106,108,110,112,114,116,119,121,123,127,128,129,132,134,136,138,140,141,144,146,148,150,152,156,158,160,162,167,169,171,173,177,179 NOPBC
b1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=193,195,197,199,203,205,208,210,212,214,215,218,220,222,224,226,228,230,232,234,236,238,240,242,244,246,248,251,252,255,257,259,261,264,266,267 NOPBC
b2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=269,271,273,275,277,279,282,284,286,290,291,292,295,297,299,301,303,304,307,309,311,313,315,319,321,323,325,328,330,332,334,336,340,342 NOPBC


<span style="color:blue"># distance both ubiquitin</span>
d1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=a,b NOPBC
<span style="color:blue">#relativ orientation</span>
tor1: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=a1,a2,b1,b2 NOPBC

rg: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_y_r_a_t_i_o_n.html">GYRATION</a> ATOMS=1,3,4,6,10,14,18,22,26,30,31,32,34,36,40,42,45,47,49,51,52,55,57,59,61,63,65,67,69,71,73,75,77,79,81,83,85,88,89,92,94,96,98,101,103,104,106,108,110,112,114,116,119,121,123,127,128,129,132,134,136,138,140,141,144,146,148,150,152,156,158,160,162,165,167,169,171,173,177,179,181,183,186,188,191,192,193,195,197,199,203,205,208,210,212,214,215,218,220,222,224,226,228,230,232,234,236,238,240,242,244,246,248,251,252,255,257,259,261,264,266,267,269,271,273,275,277,279,282,284,286,290,291,292,295,297,299,301,303,304,307,309,311,313,315,319,321,323,325,328,330,332,334,336,340,342,344,346,349,351,354,355 NOPBC


<a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_b_e_t_a.html">ALPHABETA</a> ...
LABEL=linktor1
REFERENCE=0
ATOMS1=179,181,183,186
ATOMS2=181,183,186,188
ATOMS3=183,186,188,191
ATOMS4=186,188,191,192
ATOMS5=188,191,192,193
ATOMS6=191,192,193,195
... <a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_b_e_t_a.html">ALPHABETA</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_s_a_x_s.html">SAXS</a> ...
LABEL=test2
ATOMS=1-355
NOPBC

MARTINI

QVALUE1=0.0178612
QVALUE2=0.0290150
QVALUE3=0.0401689
QVALUE4=0.0513227
QVALUE5=0.0624766
QVALUE6=0.0736304
QVALUE7=0.0847843
QVALUE8=0.0959381
QVALUE9=0.1070922
QVALUE10=0.118246
QVALUE11=0.129399
QVALUE12=0.140553
QVALUE13=0.151707
QVALUE14=0.162861
QVALUE15=0.174015
QVALUE16=0.185169
QVALUE17=0.196323
QVALUE18=0.207476
QVALUE19=0.218630
QVALUE20=0.229784
QVALUE21=0.240938

EXPINT1=1.11825
EXPINT2=1.02402
EXPINT3=0.901402
EXPINT4=0.768395
EXPINT5=0.637896
EXPINT6=0.51898
EXPINT7=0.417004
EXPINT8=0.333873
EXPINT9=0.268715
EXPINT10=0.218862
EXPINT11=0.18084
EXPINT12=0.151206
EXPINT13=0.127107
EXPINT14=0.106525
EXPINT15=0.0882832
EXPINT16=0.0718846
EXPINT17=0.0572756
EXPINT18=0.0446096
EXPINT19=0.0340539
EXPINT20=0.0256793
EXPINT21=0.0194114

... <a href="https://plumed.github.io/doc-master/user-doc/html/_s_a_x_s.html">SAXS</a>

lsaxs: <a href="https://plumed.github.io/doc-master/user-doc/html/_s_t_a_t_s.html">STATS</a> ARG=(test2\.q-.*) PARARG=(test2\.exp-.*)

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_b_m_e_t_a_d.html">PBMETAD</a> ...
LABEL=bias
ARG=d1,tor1,rg,linktor1
HEIGHT=0.1
PACE=200
BIASFACTOR=20
ADAPTIVE=DIFF
GRID_WFILES=GRID.0,GRID.1,GRID.2,GRID.3
GRID_WSTRIDE=2000
<span style="color:blue">#GRID_RFILES=GRID.0,GRID.1,GRID.2,GRID.3</span>
SIGMA=10000
SIGMA_MIN=0.005,0.005,0.005,0.005
SIGMA_MAX=0.2,0.2,0.2,0.2

GRID_MIN=0,-pi,0,0
GRID_MAX=7,pi,6,6

WALKERS_MPI
UPDATE_FROM=2000
... <a href="https://plumed.github.io/doc-master/user-doc/html/_p_b_m_e_t_a_d.html">PBMETAD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_i_n_f_e_r_e_n_c_e.html">METAINFERENCE</a> ...
SCALEDATA
AVERAGING=100
NOISETYPE=MOUTLIERS
ARG=(test2\.q-.*),bias.bias REWEIGHT PARARG=(test2\.exp-.*)
SCALE_PRIOR=FLAT
ADDOFFSET
OFFSET_PRIOR=FLAT
OFFSET0=0 OFFSET_MIN=-1 OFFSET_MAX=1 DOFFSET=0.002
SCALE0=1.00 SCALE_MIN=0.9 SCALE_MAX=1.1 DSCALE=0.00005
SIGMA0=0.001 SIGMA_MIN=0. SIGMA_MAX=0.02 DSIGMA=0.0001
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
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FILE=Analyse.dat ARG=d1,tor1,rg,linktor1 STRIDE=100
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FILE=BIAS ARG=bias.bias STRIDE=100
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FILE=ENSAXS ARG=(ensaxs\.test2\.q-.*) STRIDE=100

enANA: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_s_e_m_b_l_e.html">ENSEMBLE</a> ARG=d1,tor1,rg,linktor1,bias.bias REWEIGHT
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FILE=ENANA ARG=enANA.* STRIDE=100


</pre>{% endraw %}
