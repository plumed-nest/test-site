**Project ID:** [plumID:19.017]({{ '/' | absolute_url }}eggs/19/017/)  
**Source:** plumed_reweight/reweight_rho_c.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [raw zipped stdout](reweight_rho_c.dat.plumed.stdout.txt.zip) - [stderr](reweight_rho_c.dat.plumed.stderr)  
**Master:** [raw zipped stdout](reweight_rho_c.dat.plumed_master.stdout.txt.zip) - [stderr](reweight_rho_c.dat.plumed_master.stderr)  

{% raw %}<pre>
rho: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_a_d.html">READ</a> FILE=../input/rtp_coord.dat VALUES=rho IGNORE_FORCES IGNORE_TIME
c: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_a_d.html">READ</a> FILE=../input/all_coordination_45.dat VALUES=c IGNORE_FORCES IGNORE_TIME
metad: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_a_d.html">READ</a> FILE=../input/metad_data.dat VALUES=metad.* IGNORE_FORCES IGNORE_TIME

weights: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__m_e_t_a_d.html">REWEIGHT_METAD</a> TEMP=300 ARG=metad.rbias

<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ...
  ARG=rho,c
  GRID_MIN=0.,0.
  GRID_MAX=3.0,160.
  GRID_BIN=100,100
  KERNEL=DISCRETE
  LOGWEIGHTS=weights
  LABEL=hD
... <a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a>

ff: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=hD TEMP=300.
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=ff FILE=rew_fes_rhoc.dat STRIDE=5000

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
