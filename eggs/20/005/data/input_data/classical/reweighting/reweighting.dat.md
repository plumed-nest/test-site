**Project ID:** [plumID:20.005]({{ '/' | absolute_url }}eggs/20/005/)  
**Source:** input_data/classical/reweighting/reweighting.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [raw zipped stdout](reweighting.dat.plumed.stdout.txt.zip) - [stderr](reweighting.dat.plumed.stderr)  
**Master:** [raw zipped stdout](reweighting.dat.plumed_master.stdout.txt.zip) - [stderr](reweighting.dat.plumed_master.stderr)  

{% raw %}<pre>
p1: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_a_d.html">READ</a> FILE=../test_data/metad_data.dat VALUES=p1.* IGNORE_FORCES IGNORE_TIME
metad: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_a_d.html">READ</a> FILE=../test_data/metad_data.dat VALUES=metad.* IGNORE_FORCES IGNORE_TIME

weights: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__m_e_t_a_d.html">REWEIGHT_METAD</a> TEMP=310.15 ARG=metad.rbias

<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ...
  ARG=p1.s,p1.z
  GRID_MIN=0,-0.2
  GRID_MAX=12,0.3
  GRID_BIN=200,200
  KERNEL=DISCRETE
  LOGWEIGHTS=weights
  LABEL=hD
... <a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a>

ff: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=hD TEMP=310.15
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=ff FILE=rew_fes.dat


<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
