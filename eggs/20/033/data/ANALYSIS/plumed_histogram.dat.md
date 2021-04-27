**Project ID:** [plumID:20.033]({{ '/' | absolute_url }}eggs/20/033/)  
**Source:** ANALYSIS/plumed_histogram.dat  
**Originally used with PLUMED version:** 2.6  
**Stable:** [raw zipped stdout](plumed_histogram.dat.plumed.stdout.txt.zip) - [stderr](plumed_histogram.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_histogram.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_histogram.dat.plumed_master.stderr)  

{% raw %}<pre>
rmsd_closed: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_a_d.html">READ</a> FILE=COLVAR_final VALUES=rmsd_closed_charmm_6vxx IGNORE_TIME
rmsd_open: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_a_d.html">READ</a> FILE=COLVAR_final VALUES=rmsd_open IGNORE_TIME
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=rmsd_closed,rmsd_open FILE=check

<span style="color:blue">#rw: REWEIGHT_METAD TEMP=300</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ...
  ARG=rmsd_closed,rmsd_open
  GRID_MIN=0,0
  GRID_MAX=2.0,2.0
  GRID_BIN=200,200
  BANDWIDTH=0.01,0.01
  <span style="color:blue">#KERNEL=discrete</span>
  <span style="color:blue">#LOGWEIGHTS=rw</span>
  LABEL=hh
... <a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a>


<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=hh FILE=histo  STRIDE=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=hh LABEL=FES_temp TEMP=300
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=FES_temp FILE=fes_reweighted.dat STRIDE=10000
</pre>{% endraw %}
