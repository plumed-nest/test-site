**Project ID:** [plumID:20.014]({{ '/' | absolute_url }}eggs/20/014/)  
**Source:** PLUMED_input_files/AB42_alone/plumed/plumed.dat  
**Originally used with PLUMED version:** 2.6.0  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue">#this is the master plumed.dat file for metadynamic metainference simulations</span>

<span style="color:blue"># define groups</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">MOLINFO</a> STRUCTURE=../system/template.pdb
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=1-627
<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=1000

<span style="color:blue">#include file with definition of metadynamics CVs</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_i_n_c_l_u_d_e.html">INCLUDE</a> FILE=<a href="CVs.dat.html">CVs.dat</a>

<span style="color:blue"># Chemical shifts at 278 K</span>
cs: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_s2_b_a_c_k_b_o_n_e.html">CS2BACKBONE</a> ATOMS=1-627 DATADIR=../data NOPBC TEMPLATE=../system/template.pdb

<span style="color:blue">#activate parallel bias metadynamics </span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_b_m_e_t_a_d.html">PBMETAD</a> ...
    ARG=helix.lessthan,beta,rgyr,hydro,salt,dihcor
    HEIGHT=1.2
    BIASFACTOR=24 <span style="color:blue">#10*SQRT(NUM_OF_CVS)</span>
    SIGMA=0.64,0.33,0.03,0.69,2.75,1.34
    PACE=500
    GRID_MIN=-1,-1,-1,-1,-1,-1
    GRID_MAX=100,100,20,200,400,50
    GRID_SPACING=0.1,0.1,0.01,0.1,0.1,0.01    
    GRID_WSTRIDE=10000
<span style="color:blue">#    GRID_RFILES=GRID.helix.lessthan,GRID.beta,GRID.rgyr,GRID.hydro,GRID.salt,GRID.dihcor</span>
    FILE=HILLS_helix,HILLS_beta,HILLS_rgyr,HILLS_hydro,HILLS_salt,HILLS_dihcor
    WALKERS_MPI
    LABEL=pbmetad
... <a href="https://plumed.github.io/doc-master/user-doc/html/_p_b_m_e_t_a_d.html">PBMETAD</a>

<span style="color:blue"># Metainference - one sigma per nucleus</span>
cs_ha: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_i_n_f_e_r_e_n_c_e.html">METAINFERENCE</a> ARG=(cs\.ha-.*),pbmetad.bias PARARG=(cs\.expha-.*) SIGMA0=9.0 SIGMA_MIN=0.00001 SIGMA_MAX=10.0 DSIGMA=0.1 NOISETYPE=GAUSS REWEIGHT SIGMA_MEAN0=0.5 OPTSIGMAMEAN=SEM AVERAGING=500 WRITE_STRIDE=2500 STATUS_FILE=MISTATUS.cs_ha
cs_hn: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_i_n_f_e_r_e_n_c_e.html">METAINFERENCE</a> ARG=(cs\.hn-.*),pbmetad.bias PARARG=(cs\.exphn-.*) SIGMA0=9.0 SIGMA_MIN=0.00001 SIGMA_MAX=10.0 DSIGMA=0.1 NOISETYPE=GAUSS REWEIGHT SIGMA_MEAN0=0.5 OPTSIGMAMEAN=SEM AVERAGING=500 WRITE_STRIDE=2500 STATUS_FILE=MISTATUS.cs_hn
cs_nh: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_i_n_f_e_r_e_n_c_e.html">METAINFERENCE</a> ARG=(cs\.nh-.*),pbmetad.bias PARARG=(cs\.expnh-.*) SIGMA0=9.0 SIGMA_MIN=0.00001 SIGMA_MAX=10.0 DSIGMA=0.1 NOISETYPE=GAUSS REWEIGHT SIGMA_MEAN0=0.5 OPTSIGMAMEAN=SEM AVERAGING=500 WRITE_STRIDE=2500 STATUS_FILE=MISTATUS.cs_nh
cs_ca: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_i_n_f_e_r_e_n_c_e.html">METAINFERENCE</a> ARG=(cs\.ca-.*),pbmetad.bias PARARG=(cs\.expca-.*) SIGMA0=9.0 SIGMA_MIN=0.00001 SIGMA_MAX=10.0 DSIGMA=0.1 NOISETYPE=GAUSS REWEIGHT SIGMA_MEAN0=0.5 OPTSIGMAMEAN=SEM AVERAGING=500 WRITE_STRIDE=2500 STATUS_FILE=MISTATUS.cs_ca
cs_cb: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_i_n_f_e_r_e_n_c_e.html">METAINFERENCE</a> ARG=(cs\.cb-.*),pbmetad.bias PARARG=(cs\.expcb-.*) SIGMA0=9.0 SIGMA_MIN=0.00001 SIGMA_MAX=10.0 DSIGMA=0.1 NOISETYPE=GAUSS REWEIGHT SIGMA_MEAN0=0.5 OPTSIGMAMEAN=SEM AVERAGING=500 WRITE_STRIDE=2500 STATUS_FILE=MISTATUS.cs_cb
cs_co: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_i_n_f_e_r_e_n_c_e.html">METAINFERENCE</a> ARG=(cs\.co-.*),pbmetad.bias PARARG=(cs\.expco-.*) SIGMA0=9.0 SIGMA_MIN=0.00001 SIGMA_MAX=10.0 DSIGMA=0.1 NOISETYPE=GAUSS REWEIGHT SIGMA_MEAN0=0.5 OPTSIGMAMEAN=SEM AVERAGING=500 WRITE_STRIDE=2500 STATUS_FILE=MISTATUS.cs_co

<span style="color:blue"># Ensemble statistics</span>
ens: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_s_e_m_b_l_e.html">ENSEMBLE</a> ARG=(cs\.ha-.*),(cs\.hn-.*),(cs\.nh-.*),(cs\.ca-.*),(cs\.cb-.*),(cs\.co-.*),pbmetad.bias REWEIGHT

<a href="https://plumed.github.io/doc-master/user-doc/html/_s_t_a_t_s.html">STATS</a> ...
    ARG=(ens\.cs\.ha-.*),(ens\.cs\.hn-.*),(ens\.cs\.nh-.*),(ens\.cs\.ca-.*),(ens\.cs\.cb-.*),(ens\.cs\.co-.*)
    PARARG=(cs\.expha-.*),(cs\.exphn-.*),(cs\.expnh-.*),(cs\.expca-.*),(cs\.expcb-.*),(cs\.expco-.*) 
    LABEL=stat
... <a href="https://plumed.github.io/doc-master/user-doc/html/_s_t_a_t_s.html">STATS</a>

<span style="color:blue">#print out relevant info</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=helix.lessthan,beta,rgyr,hydro,salt,dihcor,pbmetad.bias FILE=COLVAR STRIDE=500
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=(ens.*),(stat.*) FILE=STATS STRIDE=500
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=(cs_ha.*) FILE=BAYES.HA STRIDE=500
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=(cs_hn.*) FILE=BAYES.HN STRIDE=500
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=(cs_nh.*) FILE=BAYES.NH STRIDE=500
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=(cs_ca.*) FILE=BAYES.CA STRIDE=500
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=(cs_cb.*) FILE=BAYES.CB STRIDE=500
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=(cs_co.*) FILE=BAYES.CO STRIDE=500
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
