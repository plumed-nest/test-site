**Project ID:** [plumID:21.014]({{ '/' | absolute_url }}eggs/21/014/)  
**Source:** PLUMED-NEST_chignolin/Part2_MM/plumed_PB4_MM.dat  
**Originally used with PLUMED version:** 2.7  
**Stable:** [raw zipped stdout](plumed_PB4_MM.dat.plumed.stdout.txt.zip) - [stderr](plumed_PB4_MM.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_PB4_MM.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_PB4_MM.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">MOLINFO</a> STRUCTURE=../template.pdb
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=1-166

s1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">back-1</a> NOPBC 
s2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">back-2</a> NOPBC
s3: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">back-3</a> NOPBC
s4: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">back-4</a> NOPBC
s5: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">back-5</a> NOPBC
s6: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">back-6</a> NOPBC
s7: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">back-7</a> NOPBC
s8: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">back-8</a> NOPBC
s9: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">back-9</a> NOPBC
s10: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">back-10</a> NOPBC

<a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_b_e_t_a.html">ALPHABETA</a> ...
NOPBC
LABEL=back
REFERENCE=0
ATOMS1=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-1</a>    COEFFICIENT1=-0.01427455
ATOMS2=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">phi-2</a>    COEFFICIENT2=-0.03003557
ATOMS3=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-2</a>    COEFFICIENT3=-0.23777775
ATOMS4=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">phi-3</a>    COEFFICIENT4=0.139227
ATOMS5=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-3</a>    COEFFICIENT5=0.26525215
ATOMS6=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">phi-4</a>    COEFFICIENT6=-0.18108167
ATOMS7=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-4</a>    COEFFICIENT7=0.01530576
ATOMS8=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">phi-5</a>    COEFFICIENT8=0.07231603
ATOMS9=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-5</a>    COEFFICIENT9=-0.1183752
ATOMS10=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">phi-6</a>  COEFFICIENT10=0.00089293
ATOMS11=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-6</a>  COEFFICIENT11=-0.23744683
ATOMS12=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">phi-7</a>  COEFFICIENT12=0.15661255
ATOMS13=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-7</a>  COEFFICIENT13=0.63855605
ATOMS14=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">phi-8</a>  COEFFICIENT14=-0.15161411
ATOMS15=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-8</a>  COEFFICIENT15=0.50759965
ATOMS16=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">phi-9</a>  COEFFICIENT16=-0.04886669
ATOMS17=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-9</a>  COEFFICIENT17=0.13599118
ATOMS18=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">phi-10</a> COEFFICIENT18=-0.1007816
...
          
cmap: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t_m_a_p.html">CONTACTMAP</a> ...
NOPBC
SWITCH={RATIONAL R_0=0.6}
ATOMS1=s1,s4     WEIGHT1=0.02521988
ATOMS2=s1,s5     WEIGHT2=0.20455216
ATOMS3=s1,s6     WEIGHT3=-0.54414755
ATOMS4=s1,s7     WEIGHT4=0.36219968
ATOMS5=s1,s8     WEIGHT5=0.1279484
ATOMS6=s1,s9     WEIGHT6=-0.22453008
ATOMS7=s1,s10    WEIGHT7=0.29550159
ATOMS8=s2,s5     WEIGHT8=-0.03385588
ATOMS9=s2,s6     WEIGHT9=0.09919236
ATOMS10=s2,s7   WEIGHT10=-0.03330457
ATOMS11=s2,s8   WEIGHT11=-0.13847136
ATOMS12=s2,s9   WEIGHT12=0.39094173
ATOMS13=s2,s10  WEIGHT13=-0.1983029
ATOMS14=s3,s6   WEIGHT14=-0.02328201
ATOMS15=s3,s7   WEIGHT15=0.0069981
ATOMS16=s3,s8   WEIGHT16=0.2231250
ATOMS17=s3,s9   WEIGHT17=-0.25618473
ATOMS18=s3,s10  WEIGHT18=0.113674
ATOMS19=s4,s7   WEIGHT19=0.01257499
ATOMS20=s4,s8   WEIGHT20=-0.01498744
ATOMS21=s4,s9   WEIGHT21=-0.11663488
ATOMS22=s4,s10  WEIGHT22=0.084924
ATOMS23=s5,s8   WEIGHT23=-0.005496
ATOMS24=s5,s9   WEIGHT24=0.03150733
ATOMS25=s5,s10  WEIGHT25=-0.03456732
ATOMS26=s6,s9   WEIGHT26=0.00233215
ATOMS27=s6,s10  WEIGHT27=0.01574143
ATOMS28=s7,s10  WEIGHT28=-0.01026257
SUM
...

rg: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_y_r_a_t_i_o_n.html">GYRATION</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-1</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-1</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">C-1</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-2</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-2</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">C-2</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-3</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-3</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">C-3</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-4</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-4</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">C-4</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-5</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-5</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">C-5</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-6</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-6</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">C-6</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-7</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-7</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">C-7</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-8</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-8</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">C-8</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-9</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-9</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">C-9</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-10</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-10</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">C-10</a> NOPBC
hh: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_n_t_i_b_e_t_a_r_m_s_d.html">ANTIBETARMSD</a> RESIDUES=all TYPE=DRMSD R_0=0.1 STRANDS_CUTOFF=1 NOPBC

mm: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_b_m_e_t_a_d.html">PBMETAD</a> ... 
ARG=back,cmap,rg,hh 
SIGMA_MAX=0.2,0.2,0.2,0.2 
SIGMA_MIN=0.01,0.001,0.004,0.02 
SIGMA=0.015 ADAPTIVE=GEOM 
GRID_MIN=-4,-2,0.3,0 
GRID_MAX=4,2,1.4,3
HEIGHT=0.5 BIASFACTOR=10 PACE=200 
WALKERS_MPI 
FILE=../HILLS.back,../HILLS.cmap,../HILLS.rg,../HILLS.hh
GRID_WFILES=../GRID.back,../GRID.cmap,../GRID.rg,../GRID.hh
<span style="color:blue">#GRID_RFILES=../GRID.back,../GRID.cmap,../GRID.rg,../GRID.hh</span>
GRID_WSTRIDE=10000000
...

<a href="https://plumed.github.io/doc-master/user-doc/html/_s_a_x_s.html">SAXS</a> ...
        NOPBC
        <span style="color:blue">#GPU</span>
        LABEL=saxs
        ATOMS=1-166  
        ATOMISTIC
        SCALEINT=100

	QVALUE1=0.010000	EXPINT1=99.884787
	QVALUE2=0.070000	EXPINT2=94.573283
	QVALUE3=0.130000	EXPINT3=82.964898
	QVALUE4=0.190000	EXPINT4=68.296624
	QVALUE5=0.250000	EXPINT5=53.565198
	QVALUE6=0.310000	EXPINT6=40.540191
	QVALUE7=0.370000	EXPINT7=29.869842
	QVALUE8=0.430000	EXPINT8=21.605034
	QVALUE9=0.490000	EXPINT9=15.542217
	QVALUE10=0.550000	EXPINT10=11.346918
	QVALUE11=0.610000	EXPINT11=8.628281
	QVALUE12=0.670000	EXPINT12=7.008095
	QVALUE13=0.730000	EXPINT13=6.154012
	QVALUE14=0.790000	EXPINT14=5.789840
	QVALUE15=0.850000	EXPINT15=5.711048
	QVALUE16=0.910000	EXPINT16=5.799616
	QVALUE17=0.970000	EXPINT17=6.016059
	QVALUE18=1.030000	EXPINT18=6.361548
	QVALUE19=1.090000	EXPINT19=6.825863
	QVALUE20=1.150000	EXPINT20=7.352355	
	QVALUE21=1.210000	EXPINT21=7.844432
	QVALUE22=1.270000	EXPINT22=8.208167
	QVALUE23=1.330000	EXPINT23=8.399227
	QVALUE24=1.390000	EXPINT24=8.442345

        DOSCORE
        REWEIGHT ARG=mm.bias
        NOISETYPE=MGAUSS
        SCALEDATA  SCALE_PRIOR=FLAT SCALE0=1.00 SCALE_MIN=0.5 SCALE_MAX=1.5 DSCALE=0.0002
        SIGMA0=1
        SIGMA_MIN=0.001
        MC_CHUNKSIZE=2 MC_STEPS=12 
        SIGMA_MEAN0=3
        OPTSIGMAMEAN=SEM_MAX 
	AVERAGING=200
        WRITE_STRIDE=10000
... <a href="https://plumed.github.io/doc-master/user-doc/html/_s_a_x_s.html">SAXS</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_b_i_a_s_v_a_l_u_e.html">BIASVALUE</a> ARG=saxs.score STRIDE=2

ens: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_s_e_m_b_l_e.html">ENSEMBLE</a> ARG=(saxs\.q-.*),mm.bias REWEIGHT
st: <a href="https://plumed.github.io/doc-master/user-doc/html/_s_t_a_t_s.html">STATS</a> ARG=(ens\.saxs\.q-.*) PARARG=(saxs\.exp-.*)

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=(saxs\.score),(saxs\.biasDer),(saxs\.weight),(saxs\.neff),(saxs\.scale),(saxs\.acceptScale),(saxs\.acceptSigma),(saxs\.sigma.*)  FILE=BAYES STRIDE=5000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=st.*,(ens\.saxs\.q-.*) FILE=STATS STRIDE=5000
<span style="color:blue">#PRINT ARG=(saxs\.q-.*)  FILE=QVALUE STRIDE=5000</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=back,cmap,rg,hh FILE=COLVAR STRIDE=5000
</pre>{% endraw %}
