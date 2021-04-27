**Project ID:** [plumID:19.009]({{ '/' | absolute_url }}eggs/19/009/)  
**Source:** GAGA/ccGAGAgg.plumed.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](ccGAGAgg.plumed.dat.plumed.stdout.txt.zip) - [stderr](ccGAGAgg.plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](ccGAGAgg.plumed.dat.plumed_master.stdout.txt.zip) - [stderr](ccGAGAgg.plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">MOLINFO</a> STRUCTURE=GAGA_8_H.pdb
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=1-263

e0: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_r_m_s_d.html">ERMSD</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-1</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-2</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-3</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-4</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-5</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-6</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-7</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-8</a> REFERENCE=GAGA_8_H.pdb
e3: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_r_m_s_d.html">ERMSD</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-1</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-2</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-3</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-4</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-5</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-6</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-7</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-8</a> REFERENCE=GAGA_8_L.pdb

ee3: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_r_m_s_d.html">ERMSD</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-1</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-2</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-3</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-4</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-5</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-6</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-7</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-8</a> REFERENCE=GAGA_8_L.pdb CUTOFF=3.2

r0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_m_s_d.html">RMSD</a> REFERENCE=GAGA_8_H.pdb TYPE=OPTIMAL
r3: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_m_s_d.html">RMSD</a> REFERENCE=GAGA_8_L.pdb TYPE=OPTIMAL


metad: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=ee3 PACE=500000001 HEIGHT=0.0 SIGMA=0.1 FILE=HILLS_avg_5 TEMP=300.882 BIASFACTOR=15 GRID_MIN=0.0 GRID_MAX=5.0 GRID_BIN=250

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=e3,ee3,e0,r3,r0,metad.bias FILE=colvar_5 STRIDE=1

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
<span style="color:blue"></span>
<span style="color:blue"><span style="color:blue"># histograms below are computed using PLUMED 2.3 syntax</span></span>
<span style="color:blue"></span>
<span style="color:blue">HISTOGRAM ...</span>
<span style="color:blue">REWEIGHT_BIAS</span>
<span style="color:blue">ARG=e3</span>
<span style="color:blue">TEMP=300.882</span>
<span style="color:blue">USE_ALL_DATA</span>
<span style="color:blue">UNNORMALIZED</span>
<span style="color:blue">GRID_MIN=0</span>
<span style="color:blue">GRID_MAX=3</span>
<span style="color:blue">GRID_BIN=250</span>
<span style="color:blue">RESTART=NO</span>
<span style="color:blue">BANDWIDTH=0.0075</span>
<span style="color:blue">GRID_WFILE=fes_ermsd_5_0</span>
<span style="color:blue">UPDATE_FROM=200000</span>
<span style="color:blue">UPDATE_UNTIL=400000</span>
<span style="color:blue">... HISTOGRAM</span>
<span style="color:blue"></span>
<span style="color:blue">HISTOGRAM ...</span>
<span style="color:blue">REWEIGHT_BIAS</span>
<span style="color:blue">ARG=e3</span>
<span style="color:blue">TEMP=300.882</span>
<span style="color:blue">USE_ALL_DATA</span>
<span style="color:blue">UNNORMALIZED</span>
<span style="color:blue">GRID_MIN=0</span>
<span style="color:blue">GRID_MAX=3</span>
<span style="color:blue">GRID_BIN=250</span>
<span style="color:blue">RESTART=NO</span>
<span style="color:blue">BANDWIDTH=0.0075</span>
<span style="color:blue">GRID_WFILE=fes_ermsd_5_1</span>
<span style="color:blue">UPDATE_FROM=400000</span>
<span style="color:blue">UPDATE_UNTIL=600000</span>
<span style="color:blue">... HISTOGRAM</span>
<span style="color:blue"></span>
<span style="color:blue"></span>
<span style="color:blue">HISTOGRAM ...</span>
<span style="color:blue">REWEIGHT_BIAS</span>
<span style="color:blue">ARG=e3</span>
<span style="color:blue">TEMP=300.882</span>
<span style="color:blue">USE_ALL_DATA</span>
<span style="color:blue">UNNORMALIZED</span>
<span style="color:blue">GRID_MIN=0</span>
<span style="color:blue">GRID_MAX=3</span>
<span style="color:blue">GRID_BIN=250</span>
<span style="color:blue">RESTART=NO</span>
<span style="color:blue">BANDWIDTH=0.0075</span>
<span style="color:blue">GRID_WFILE=fes_ermsd_5_2</span>
<span style="color:blue">UPDATE_FROM=600000</span>
<span style="color:blue">UPDATE_UNTIL=800000</span>
<span style="color:blue">... HISTOGRAM</span>
<span style="color:blue"></span>
<span style="color:blue"></span>
<span style="color:blue">HISTOGRAM ...</span>
<span style="color:blue">REWEIGHT_BIAS</span>
<span style="color:blue">ARG=e3</span>
<span style="color:blue">TEMP=300.882</span>
<span style="color:blue">USE_ALL_DATA</span>
<span style="color:blue">UNNORMALIZED</span>
<span style="color:blue">GRID_MIN=0</span>
<span style="color:blue">GRID_MAX=3</span>
<span style="color:blue">GRID_BIN=250</span>
<span style="color:blue">RESTART=NO</span>
<span style="color:blue">BANDWIDTH=0.0075</span>
<span style="color:blue">GRID_WFILE=fes_ermsd_5_3</span>
<span style="color:blue">UPDATE_FROM=800000</span>
<span style="color:blue">UPDATE_UNTIL=1000000</span>
<span style="color:blue">... HISTOGRAM</span>
<span style="color:blue"></span>
<span style="color:blue"><span style="color:blue">################################</span></span>
<span style="color:blue"></span>
<span style="color:blue">HISTOGRAM ...</span>
<span style="color:blue">REWEIGHT_BIAS</span>
<span style="color:blue">ARG=r3</span>
<span style="color:blue">TEMP=300.882</span>
<span style="color:blue">USE_ALL_DATA</span>
<span style="color:blue">UNNORMALIZED</span>
<span style="color:blue">GRID_MIN=0</span>
<span style="color:blue">GRID_MAX=1</span>
<span style="color:blue">GRID_BIN=250</span>
<span style="color:blue">RESTART=NO</span>
<span style="color:blue">BANDWIDTH=0.0025</span>
<span style="color:blue">GRID_WFILE=fes_rmsd_5_0</span>
<span style="color:blue">UPDATE_FROM=0</span>
<span style="color:blue">UPDATE_UNTIL=250000</span>
<span style="color:blue">... HISTOGRAM</span>
<span style="color:blue"></span>
<span style="color:blue">HISTOGRAM ...</span>
<span style="color:blue">REWEIGHT_BIAS</span>
<span style="color:blue">ARG=r3</span>
<span style="color:blue">TEMP=300.882</span>
<span style="color:blue">USE_ALL_DATA</span>
<span style="color:blue">UNNORMALIZED</span>
<span style="color:blue">GRID_MIN=0</span>
<span style="color:blue">GRID_MAX=1</span>
<span style="color:blue">GRID_BIN=250</span>
<span style="color:blue">RESTART=NO</span>
<span style="color:blue">BANDWIDTH=0.0025</span>
<span style="color:blue">GRID_WFILE=fes_rmsd_5_1</span>
<span style="color:blue">UPDATE_FROM=250000</span>
<span style="color:blue">UPDATE_UNTIL=500000</span>
<span style="color:blue">... HISTOGRAM</span>
<span style="color:blue"></span>
<span style="color:blue"></span>
<span style="color:blue">HISTOGRAM ...</span>
<span style="color:blue">REWEIGHT_BIAS</span>
<span style="color:blue">ARG=r3</span>
<span style="color:blue">TEMP=300.882</span>
<span style="color:blue">USE_ALL_DATA</span>
<span style="color:blue">UNNORMALIZED</span>
<span style="color:blue">GRID_MIN=0</span>
<span style="color:blue">GRID_MAX=1</span>
<span style="color:blue">GRID_BIN=250</span>
<span style="color:blue">RESTART=NO</span>
<span style="color:blue">BANDWIDTH=0.0025</span>
<span style="color:blue">GRID_WFILE=fes_rmsd_5_2</span>
<span style="color:blue">UPDATE_FROM=500000</span>
<span style="color:blue">UPDATE_UNTIL=750000</span>
<span style="color:blue">... HISTOGRAM</span>
<span style="color:blue"></span>
<span style="color:blue"></span>
<span style="color:blue">HISTOGRAM ...</span>
<span style="color:blue">REWEIGHT_BIAS</span>
<span style="color:blue">ARG=r3</span>
<span style="color:blue">TEMP=300.882</span>
<span style="color:blue">USE_ALL_DATA</span>
<span style="color:blue">UNNORMALIZED</span>
<span style="color:blue">GRID_MIN=0</span>
<span style="color:blue">GRID_MAX=1</span>
<span style="color:blue">GRID_BIN=250</span>
<span style="color:blue">RESTART=NO</span>
<span style="color:blue">BANDWIDTH=0.0025</span>
<span style="color:blue">GRID_WFILE=fes_rmsd_5_3</span>
<span style="color:blue">UPDATE_FROM=750000</span>
<span style="color:blue">UPDATE_UNTIL=1000000</span>
<span style="color:blue">... HISTOGRAM</span>
<span style="color:blue"></span>
<span style="color:blue"></span>
<span style="color:blue"></span>
</pre>{% endraw %}
