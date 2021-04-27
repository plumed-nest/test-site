**Project ID:** [plumID:19.001]({{ '/' | absolute_url }}eggs/19/001/)  
**Source:** plumed-g3.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed-g3.dat.plumed.stdout.txt.zip) - [stderr](plumed-g3.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed-g3.dat.plumed_master.stdout.txt.zip) - [stderr](plumed-g3.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>
<span style="color:blue"># choose units - by default PLUMED uses kj/mol, nm, and ps</span>
<span style="color:blue"># UNITS ENERGY=kcal/mol LENGTH=A</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">MOLINFO</a> STRUCTURE=ref.pdb
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_a_n_d_o_m__e_x_c_h_a_n_g_e_s.html">RANDOM_EXCHANGES</a>
<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=1000

<a href="https://plumed.github.io/doc-master/user-doc/html/_i_n_c_l_u_d_e.html">INCLUDE</a> FILE=<a href="cv-s.dat.html">cv-s.dat</a>

<span style="color:blue">################################################################################################</span>
<span style="color:blue"># RESTRAINS, CONSTRAINS definition</span>
<span style="color:blue">################################################################################################</span>

eRMSD_start: ...
  <a href="https://plumed.github.io/doc-master/user-doc/html/_e_r_m_s_d.html">ERMSD</a>
  ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-1</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-2</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-3</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-4</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-5</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-7</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-8</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-9</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-10</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-11</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-12</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-13</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-14</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-15</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-16</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-17</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-18</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-19</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-20</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-21</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-22</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-23</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-24</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-25</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-26</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-27</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-28</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-29</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-30</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-31</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-32</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-33</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-34</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-35</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-36</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-37</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-38</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-39</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-40</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-41</a>
  REFERENCE=ref.pdb
...

u-wall_LPR: ...
  <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a>
  ARG=d1_lp1,d2_lp1,d3_lp1 AT=0.30,0.30,0.30 KAPPA=500.0,500.0,500.0 EXP=2,2,2 EPS=1,1,1 OFFSET=0,0,0
...

l-wall_aLPR: ...
  <a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a>
  ARG=a1_lp1,a2_lp1,a3_lp1,a4_lp1,a5_lp1 AT=2.75,2.75,2.75,2.75,2.75 KAPPA=100.0,100.0,100.0,100.0,100.0 EXP=2,2,2,2,2 EPS=1,1,1,1,1 OFFSET=0,0,0,0,0
...

LBP-rest: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=1328,1329,1330,1334,1336,1338,1339,1340,1341,1342 GROUPB=1,3,6,8,9,11,12,14,16,17,20,21,22,23,25,27,29,1296,1297,1300,1302,1303,1305,1306,1308,1309,1310,1311,1312,1314,1315,1318,1319,1320,1322,1324,1326 LOWEST

<span style="color:blue">##################################################################################################</span>
<span style="color:blue"># WALLS (PES/FES restrictions)</span>
<span style="color:blue">##################################################################################################</span>

u-wall_eRMSD_start: ...
  <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a>
  ARG=eRMSD_start AT=0.6 KAPPA=5000.0
...
 
l-wall_LBP-rest: ...
  <a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a>
  ARG=LBP-rest.lowest AT=0.8 KAPPA=5000.0 EXP=2 EPS=1 OFFSET=0
...

u-wall_d-3: ...
  <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a>
  ARG=d-3 AT=1.0 KAPPA=50.0
...
 
<span style="color:blue">####################################################################################################</span>
<span style="color:blue"># METADYNAMICS</span>
<span style="color:blue">####################################################################################################</span>

metad: ...
  <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>
  ARG=d-3 TEMP=298.16 BIASFACTOR=5 PACE=500 HEIGHT=1.0 SIGMA=0.02
  GRID_MIN=0.01 GRID_MAX=50.0 GRID_SPARSE FILE=HILLS_SRP-motif_BzCN
...

<span style="color:blue">####################################################################################################</span>
<span style="color:blue"># OUTPUTS</span>
<span style="color:blue">####################################################################################################</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=d-3,eRMSD_start,LBP-rest.lowest,metad.bias STRIDE=10 FILE=COLVAR_SRP-motif_BzCN
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=u-wall_d-3.bias,l-wall_LBP-rest.bias,u-wall_eRMSD_start.bias STRIDE=10 FILE=RESTR_BIAS_SRP-motif_BzCN

</pre>{% endraw %}
