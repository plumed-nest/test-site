**Project ID:** [plumID:19.071]({{ '/' | absolute_url }}eggs/19/071/)  
**Source:** MFI_paper_scripts/reweighting/plumed_REWE.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed_REWE.dat.plumed.stdout.txt.zip) - [stderr](plumed_REWE.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_REWE.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_REWE.dat.plumed_master.stderr)  

{% raw %}<pre>
p: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_a_d.html">READ</a>  FILE=./position  VALUES=p.x IGNORE_FORCES IGNORE_TIME

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ... 
ARG=p.x
SIGMA=0.05 
HEIGHT=0.1 
PACE=500 
BIASFACTOR=5 
LABEL=metad 
TEMP=120
GRID_MIN=-2.6
GRID_MAX=2.6
GRID_BIN=500 
REWEIGHTING_NGRID=200 
REWEIGHTING_NHILLS=10
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>


bias: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__m_e_t_a_d.html">REWEIGHT_METAD</a> TEMP=120

<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ...
  ARG=p.x
  GRID_MIN=-2.6
  GRID_MAX=2.6
  GRID_BIN=500
  BANDWIDTH=0.04
  LOGWEIGHTS=bias
  LABEL=hh
... <a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a>

ff: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=hh TEMP=120 


<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=ff FILE=fes STRIDE=500

</pre>{% endraw %}
