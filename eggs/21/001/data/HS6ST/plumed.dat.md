**Project ID:** [plumID:21.001]({{ '/' | absolute_url }}eggs/21/001/)  
**Source:** HS6ST/plumed.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">MOLINFO</a> STRUCTURE=refe_sel.pdb

<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> STRIDE=10 ENTITY0=506,513,520,534,548,568,575,599,616,635,651,675,689,1737,1751,1771,1792,1813,1832,1846,1863,1882,1926,1932,1948,1959,1983,2004,2023,2034,2049,2073,2095,2112,2128,2145,3595,3615,3632,3656

<span style="color:blue"># Assign atoms to group names.</span>
<span style="color:blue"># Chooses only the the water oxygens for coordination number with water (CN_W)</span>
OW: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=5523-27022:3
S: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=5482 <span style="color:blue">#paps sulfate</span>
G: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=5460 <span style="color:blue">#GlcNAc-acceptor oxygen</span>
T: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=1248 <span style="color:blue">#soluble exposed nitrogen from TRP</span>
ene: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a>

dP:   <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=S,G
cn: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=T GROUPB=OW R_0=0.261 NLIST NL_CUTOFF=0.6 NL_STRIDE=100

<a href="https://plumed.github.io/doc-master/user-doc/html/_r_a_n_d_o_m__e_x_c_h_a_n_g_e_s.html">RANDOM_EXCHANGES</a> 
<a href="https://plumed.github.io/doc-master/user-doc/html/_i_n_c_l_u_d_e.html">INCLUDE</a> FILE=<a href="cvs.dat.html">cvs.dat</a>
metadP: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=dP,cn SIGMA=0.1,0.1 PACE=500 HEIGHT=1.5 BIASFACTOR=5 GRID_MIN=0,0 GRID_MAX=10,20 GRID_BIN=100,100 CALC_RCT RCT_USTRIDE=50 FILE=HILLS_dP3

<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=dP AT=0.0 KAPPA=35100 EXP=2 OFFSET=0 LABEL=lwall
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=dP AT=1.5 KAPPA=35100 EXP=2 OFFSET=0 LABEL=uwall

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=uwall.bias,lwall.bias FILE=bias STRIDE=100 
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=dP,cn STRIDE=100  FILE=COLVAR

bias: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__m_e_t_a_d.html">REWEIGHT_METAD</a> TEMP=300
<a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ...
  ARG=dP
  GRID_MIN=0.0
  GRID_MAX=10
  GRID_BIN=100
  BANDWIDTH=0.1
  LOGWEIGHTS=bias
  LABEL=hB
... <a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a>
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=hB FILE=histoB STRIDE=100 FMT=%8.4f
</pre>{% endraw %}
