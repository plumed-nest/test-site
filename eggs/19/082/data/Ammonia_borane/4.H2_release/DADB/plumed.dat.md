**Project ID:** [plumID:19.082]({{ '/' | absolute_url }}eggs/19/082/)  
**Source:** Ammonia_borane/4.H2_release/DADB/plumed.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue">#RESTART</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> LENGTH=A

h: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=5-128:16,6-128:16,7-128:16,8-128:16,9-128:16,10-128:16,11-128:16,12-128:16,13-128:16,14-128:16,15-128:16,16-128:16   
hb: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=7-128:16,8-128:16,13-128:16,14-128:16,15-128:16,16-128:16  
hn: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=5-128:16,6-128:16,9-128:16,10-128:16,11-128:16,12-128:16  
n: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=3-128:16,4-128:16   
b: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=1-128:16,2-128:16 
bn1: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=1-128:16,3-128:16 
bn2: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=2-128:16,4-128:16 

cnHB: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIESA=hb SPECIESB=b SWITCH={RATIONAL D_0=0.0 R_0=1.8 NN=6 MM=12} MAX={BETA=0.02}
cnHH: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIESA=hn SPECIESB=hb SWITCH={GAUSSIAN R_0=0.2 D_0=0.8 } MAX={BETA=0.02}
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_x_t_e_r_n_a_l.html">EXTERNAL</a> ARG=cnHH.max FILE=ext_bias.dat LABEL=external 

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=cnHH.max SIGMA=0.05 HEIGHT=0.1 PACE=4000 TEMP=400 BIASFACTOR=10 LABEL=restraint 

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=* STRIDE=1 FILE=COLVAR
<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=1

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
