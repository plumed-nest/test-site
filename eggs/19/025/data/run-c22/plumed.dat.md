**Project ID:** [plumID:19.025]({{ '/' | absolute_url }}eggs/19/025/)  
**Source:** run-c22/plumed.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># this is optional and tell to VIM that this is a PLUMED file</span>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim: ft=plumed</a></span>
<span style="color:blue"># see comments just below this input file</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">MOLINFO</a> MOLTYPE=protein STRUCTURE=template.pdb
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=1-111

<span style="color:blue"># CVs, Psi9, Phi1 are not defined</span>
psi1: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-1</a> NOPBC
psi2: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-2</a> NOPBC
psi3: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-3</a> NOPBC
psi4: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-4</a> NOPBC
psi5: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-5</a> NOPBC
psi6: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-6</a> NOPBC
psi7: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-7</a> NOPBC
psi8: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-8</a> NOPBC

phi2: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">phi-2</a> NOPBC
phi3: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">phi-3</a> NOPBC
phi4: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">phi-4</a> NOPBC
phi5: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">phi-5</a> NOPBC
phi6: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">phi-6</a> NOPBC
phi7: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">phi-7</a> NOPBC
phi8: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">phi-8</a> NOPBC
phi9: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">phi-9</a> NOPBC

<span style="color:blue"># Bulky Trp residue dihedral</span>
dihtrp_cacb: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=67,47,49,52
dihtrp_cbcg: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=47,49,52,53

gyr: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_y_r_a_t_i_o_n.html">GYRATION</a> TYPE=RADIUS ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-1</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-2</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-3</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-4</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-5</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-6</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-7</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-8</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-9</a> NOPBC

<span style="color:blue"># PBMetaD</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_b_m_e_t_a_d.html">PBMETAD</a> ...
    LABEL=pb
    ARG=phi2,phi3,phi4,phi5,phi6,phi7,phi8,phi9,psi1,psi2,psi3,psi4,psi5,psi6,psi7,psi8,dihtrp_cacb,dihtrp_cbcg
    SIGMA=1000 
    SIGMA_MIN=0.06,0.06,0.06,0.06,0.06,0.06,0.06,0.06,0.06,0.06,0.06,0.06,0.06,0.06,0.06,0.06,0.06,0.06
    SIGMA_MAX=0.6,0.6,0.6,0.6,0.6,0.6,0.6,0.6,0.6,0.6,0.6,0.6,0.6,0.6,0.6,0.6,0.6,0.6
    ADAPTIVE=DIFF
    HEIGHT=0.5
    PACE=200
    BIASFACTOR=34
    GRID_MIN=-pi,-pi,-pi,-pi,-pi,-pi,-pi,-pi,-pi,-pi,-pi,-pi,-pi,-pi,-pi,-pi,-pi,-pi
    GRID_MAX=pi,pi,pi,pi,pi,pi,pi,pi,pi,pi,pi,pi,pi,pi,pi,pi,pi,pi
    GRID_WSTRIDE=50000
    WALKERS_MPI
... <a href="https://plumed.github.io/doc-master/user-doc/html/_p_b_m_e_t_a_d.html">PBMETAD</a>

<span style="color:blue"># output from the collective variable</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FILE=COLVAR ARG=gyr,phi2,phi3,phi4,phi5,phi6,phi7,phi8,phi9,psi1,psi2,psi3,psi4,psi5,psi6,psi7,psi8,dihtrp_cacb,dihtrp_cbcg STRIDE=2000

<span style="color:blue"># EXPERIMENTAL DATA SECTION</span>

<span style="color:blue"># RDCs (Grzesiek et al.)</span>
<span style="color:blue"># xGAAWAASS</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_d_c.html">RDC</a> ...
    NOPBC
    GYROM=-72.5388
    SCALE=0.001
    ATOMS1=18,19 COUPLING1=-5.4
    ATOMS2=25,26 COUPLING2=-1.26
    ATOMS3=35,36 COUPLING3=-5.22
    ATOMS4=45,46 COUPLING4=-0.91
    ATOMS5=69,70 COUPLING5=2.33
    ATOMS6=79,80 COUPLING6=-2.88
    ATOMS7=89,90 COUPLING7=-8.37
    ATOMS8=100,101 COUPLING8=-3.78
    LABEL=nh
    DOSCORE
    ARG=pb.bias
    NOISETYPE=MGAUSS REWEIGHT OPTSIGMAMEAN=SEM AVERAGING=200
    REGRES_ZERO=200
    SIGMA0=1.0 SIGMA_MIN=0.0001 SIGMA_MAX=5.0 DSIGMA=0.1
    WRITE_STRIDE=10000
... <a href="https://plumed.github.io/doc-master/user-doc/html/_r_d_c.html">RDC</a>

mnh: <a href="https://plumed.github.io/doc-master/user-doc/html/_b_i_a_s_v_a_l_u_e.html">BIASVALUE</a> ARG=nh.score 

<span style="color:blue"># ExAAWAASx</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_d_c.html">RDC</a> ...
    NOPBC
    GYROM=179.9319
    SCALE=0.001
    ATOMS1=5,6 COUPLING1=12.95
    ATOMS2=27,28 COUPLING2=11.5
    ATOMS3=37,38 COUPLING3=21.42
    ATOMS4=47,48 COUPLING4=-9.37
    ATOMS5=71,72 COUPLING5=10.01
    ATOMS6=81,82 COUPLING6=15.01
    ATOMS7=91,92 COUPLING7=15.73
    LABEL=caha
    DOSCORE
    ARG=pb.bias
    NOISETYPE=MGAUSS  REWEIGHT  OPTSIGMAMEAN=SEM AVERAGING=200
    REGRES_ZERO=200
    SIGMA0=1.0 SIGMA_MIN=0.0001 SIGMA_MAX=5.0 DSIGMA=0.1
    WRITE_STRIDE=10000
... <a href="https://plumed.github.io/doc-master/user-doc/html/_r_d_c.html">RDC</a>

mcaha: <a href="https://plumed.github.io/doc-master/user-doc/html/_b_i_a_s_v_a_l_u_e.html">BIASVALUE</a> ARG=caha.score 

<span style="color:blue"># xGxAWxASx</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_j_c_o_u_p_l_i_n_g.html">JCOUPLING</a> ...
    NOPBC
    TYPE=HAN
    ATOMS1=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-2</a> COUPLING1=-0.49
    ATOMS2=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-4</a> COUPLING2=-0.54
    ATOMS3=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-5</a> COUPLING3=-0.53
    ATOMS4=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-7</a> COUPLING4=-0.39
    ATOMS5=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-8</a> COUPLING5=-0.39
    LABEL=jhan
... <a href="https://plumed.github.io/doc-master/user-doc/html/_j_c_o_u_p_l_i_n_g.html">JCOUPLING</a>

<span style="color:blue"># xxAAWAASS</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_j_c_o_u_p_l_i_n_g.html">JCOUPLING</a> ...
    NOPBC
    TYPE=HAHN
    ATOMS1=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">phi-2</a> COUPLING1=6.05
    ATOMS2=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">phi-3</a> COUPLING2=5.95
    ATOMS3=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">phi-4</a> COUPLING3=6.44
    ATOMS4=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">phi-5</a> COUPLING4=6.53
    ATOMS5=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">phi-6</a> COUPLING5=5.93
    ATOMS6=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">phi-7</a> COUPLING6=6.98
    ATOMS7=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">phi-8</a> COUPLING7=7.16
    LABEL=jhahn
... <a href="https://plumed.github.io/doc-master/user-doc/html/_j_c_o_u_p_l_i_n_g.html">JCOUPLING</a>

<span style="color:blue"># xxxxWxxxx</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_j_c_o_u_p_l_i_n_g.html">JCOUPLING</a> ...
    NOPBC
    TYPE=CCG
    ATOMS1=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-5</a> COUPLING1=1.59
    LABEL=jccg
... <a href="https://plumed.github.io/doc-master/user-doc/html/_j_c_o_u_p_l_i_n_g.html">JCOUPLING</a>

<span style="color:blue"># xxxxWxxxx</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_j_c_o_u_p_l_i_n_g.html">JCOUPLING</a> ...
    NOPBC
    TYPE=NCG
    ATOMS1=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-5</a> COUPLING1=1.21
    LABEL=jncg
... <a href="https://plumed.github.io/doc-master/user-doc/html/_j_c_o_u_p_l_i_n_g.html">JCOUPLING</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_i_n_f_e_r_e_n_c_e.html">METAINFERENCE</a> ...
    ARG=(jhan\.j-.*),(jhahn\.j-.*),(jccg\.j.*),(jncg\.j.*),pb.bias
    PARARG=(jhan\.exp-.*),(jhahn\.exp-.*),(jccg\.exp.*),(jncg\.exp.*)
    NOISETYPE=MGAUSS REWEIGHT OPTSIGMAMEAN=SEM AVERAGING=200
    SIGMA0=2.5 SIGMA_MIN=0.0001 SIGMA_MAX=5.0 DSIGMA=0.1
    WRITE_STRIDE=10000
    LABEL=byj
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_i_n_f_e_r_e_n_c_e.html">METAINFERENCE</a>
<span style="color:blue">#</span>
<span style="color:blue"># Chemical shifts</span>
cs: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_s2_b_a_c_k_b_o_n_e.html">CS2BACKBONE</a> NOPBC ATOMS=1-111 DATADIR=data TEMPLATE=template.pdb DOSCORE ARG=pb.bias NOISETYPE=MOUTLIERS REWEIGHT OPTSIGMAMEAN=SEM AVERAGING=200 SIGMA0=4.0 SIGMA_MIN=0.0001 SIGMA_MAX=5.0 DSIGMA=0.1 WRITE_STRIDE=10000
mcs: <a href="https://plumed.github.io/doc-master/user-doc/html/_b_i_a_s_v_a_l_u_e.html">BIASVALUE</a> ARG=cs.score

<span style="color:blue"># output from METAINFERENCE</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=nh.score,nh.acceptSigma,nh.weight,nh.scale,(nh\.sigma.*)   STRIDE=2000 FILE=BAYES.RDC.NH
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=caha.score,caha.acceptSigma,caha.weight,caha.scale,(caha\.sigma.*) STRIDE=2000 FILE=BAYES.RDC.CAHA
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=byj.*  STRIDE=2000 FILE=BAYES.J
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=cs.score,cs.acceptSigma,cs.weight,(cs\.sigma.*)   STRIDE=2000 FILE=BAYES.CS

<span style="color:blue"># Calculate weighted ensemble average</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_s_e_m_b_l_e.html">ENSEMBLE</a> ...
    ARG=(nh\.rdc-.*),(caha\.rdc-.*),pb.bias REWEIGHT
    LABEL=ens
... <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_s_e_m_b_l_e.html">ENSEMBLE</a>

<span style="color:blue"># We use the analogous function for all other observables</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_s_t_a_t_s.html">STATS</a> ...
    ARG=(ens\.nh\.rdc-.*) PARARG=(nh\.exp-.*)
    LABEL=nhst
... <a href="https://plumed.github.io/doc-master/user-doc/html/_s_t_a_t_s.html">STATS</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_s_t_a_t_s.html">STATS</a> ...
    ARG=(ens\.caha\.rdc-.*) PARARG=(caha\.exp-.*)
    LABEL=cahast
... <a href="https://plumed.github.io/doc-master/user-doc/html/_s_t_a_t_s.html">STATS</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=nhst.*,cahast.* FILE=STATS STRIDE=2000

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
<span style="color:blue"></span>
</pre>{% endraw %}
