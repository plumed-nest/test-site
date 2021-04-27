**Project ID:** [plumID:19.082]({{ '/' | absolute_url }}eggs/19/082/)  
**Source:** Ammonia_borane/2.AaDB_to_AB2/AaDB_bis/plumed.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue">#RESTART</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> LENGTH=A

h: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=5-128:16,6-128:16,7-128:16,8-128:16,9-128:16,10-128:16,11-128:16,12-128:16,13-128:16,14-128:16,15-128:16,16-128:16 
n: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=3-128:16,4-128:16   
b: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=1-128:16,2-128:16   
hb: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=7-128:16,8-128:16,13-128:16,14-128:16,15-128:16,16-128:16 
hn: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=5-128:16,6-128:16,9-128:16,10-128:16,11-128:16,12-128:16 
bm2: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=1-128:16,18-128:16  
nm4: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=3-128:16,20-128:16  

bbinter: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIESA=2 SPECIESB=bm2 SWITCH={RATIONAL D_0=0.0 R_0=2.5 NN=6 MM=12} MEAN
nninter: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIESA=4 SPECIESB=nm4 SWITCH={RATIONAL D_0=0.0 R_0=2.5 NN=7 MM=14} MEAN
bhbridge: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIESA=hb SPECIESB=b R_0=1.9 NN=6 MM=12 MAX={BETA=0.02}
nhbridge: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIESA=hn SPECIESB=n R_0=1.6 NN=6 MM=12 MAX={BETA=0.02}
nhcoord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIESA=4 SPECIESB=hn R_0=1.6 NN=7 MM=14 MEAN
bhcoord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIESA=2 SPECIESB=hb R_0=1.8 NN=7 MM=14 MEAN

d1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=bbinter.mean COEFFICIENTS=0.8107 PERIODIC=NO
d2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=nninter.mean COEFFICIENTS=1.1786 PERIODIC=NO
d3: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=bhbridge.max COEFFICIENTS=0.4960 PERIODIC=NO
d4: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=nhbridge.max COEFFICIENTS=0.6050 PERIODIC=NO
d5: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=nhcoord.mean COEFFICIENTS=0.2545 PERIODIC=NO
d6: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=bhcoord.mean COEFFICIENTS=0.2388 PERIODIC=NO

sdg1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3,d4,d5,d6 COEFFICIENTS=-0.0481,-0.0473,-0.1976,-0.2464,0.9415,0.0959 PERIODIC=NO
sdg2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1,d2,d3,d4,d5,d6 COEFFICIENTS=0.6319,-0.0329,-0.2130,-0.0029,0.4767,-0.5719 PERIODIC=NO

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
   ARG=sdg1,sdg2 SIGMA=0.03,0.03 HEIGHT=1.5 PACE=100 TEMP=400 BIASFACTOR=8 LABEL=restraint 
   WALKERS_N=4
   WALKERS_ID=1
   WALKERS_DIR=../
   WALKERS_RSTRIDE=50
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=* STRIDE=1 FILE=COLVAR
<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=1

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
