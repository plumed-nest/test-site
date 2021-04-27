**Project ID:** [plumID:20.026]({{ '/' | absolute_url }}eggs/20/026/)  
**Source:** plumed_WTMD.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [raw zipped stdout](plumed_WTMD.dat.plumed.stdout.txt.zip) - [stderr](plumed_WTMD.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_WTMD.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_WTMD.dat.plumed_master.stderr)  

{% raw %}<pre>
rmsd_a: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_u_l_t_i__r_m_s_d.html">MULTI_RMSD</a> REFERENCE=OBP_lis_final.pdb TYPE=MULTI-OPTIMAL
rmsd_b: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_u_l_t_i__r_m_s_d.html">MULTI_RMSD</a> REFERENCE=OBP_lsd_final.pdb TYPE=MULTI-OPTIMAL
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
LABEL=metad 
ARG=rmsd_a,rmsd_b 
SIGMA=0.01,0.01 
HEIGHT=1.0 
TEMP=310.15 
PACE=100 
GRID_MIN=0,0 GRID_MAX=1.1,1.1 
GRID_BIN=400,400
BIASFACTOR=5
CALC_RCT
RCT_USTRIDE=10
FILE=hills
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=100 ARG=* FILE=colvar
bias: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__m_e_t_a_d.html">REWEIGHT_METAD</a> TEMP=310.15
<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ...
LABEL=hist
ARG=rmsd_a,rmsd_b 
GRID_MIN=0,0 
GRID_MAX=1.1,1.1
GRID_BIN=400,400 
BANDWIDTH=0.05,0.05 
LOGWEIGHTS=bias
... <a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a>
fes: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=hist TEMP=310.15
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=fes FILE=fes STRIDE=1000000
</pre>{% endraw %}
