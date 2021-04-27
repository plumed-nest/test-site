**Project ID:** [plumID:19.082]({{ '/' | absolute_url }}eggs/19/082/)  
**Source:** Ammonia_borane/1.AB_to_AaDB/AB_bis/plumed.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> LENGTH=A

h: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=5-128:16,6-128:16,7-128:16,8-128:16,9-128:16,10-128:16,11-128:16,12-128:16,13-128:16,14-128:16,15-128:16,16-128:16 
n: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=3-128:16,4-128:16   
b: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=1-128:16,2-128:16   
hb: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=7-128:16,8-128:16,13-128:16,14-128:16,15-128:16,16-128:16 
hn: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=5-128:16,6-128:16,9-128:16,10-128:16,11-128:16,12-128:16  
bm2: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=1-128:16,18-128:16  

bnintrag: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIESA=b SPECIESB=n R_0=2.0 NN=6 MM=12 MIN={BETA=20.0}
bnintranew: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIESA=2 SPECIESB=4 R_0=2.2 NN=4 MM=8 MEAN
bbinter: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIESA=2 SPECIESB=bm2 SWITCH={RATIONAL D_0=0.0 R_0=2.5 NN=6 MM=12} MAX={BETA=0.02} 
bhbridge: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIESA=hb SPECIESB=b R_0=1.9 NN=6 MM=12 MAX={BETA=0.02}

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
   ARG=bnintrag.min,bhbridge.max SIGMA=0.075,0.075 HEIGHT=1.5 PACE=100 TEMP=400 BIASFACTOR=16 LABEL=restraint 
   WALKERS_N=4
   WALKERS_ID=1
   WALKERS_DIR=../
   WALKERS_RSTRIDE=1
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=* STRIDE=1 FILE=COLVAR
<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=1

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
