**Project ID:** [plumID:20.007]({{ '/' | absolute_url }}eggs/20/007/)  
**Source:** single/plumed.dat  
**Originally used with PLUMED version:** 2.4.2  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># The commented out lines are the original implementation. They have been altered to be compatible with newer PLUMED versions.</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">MOLINFO</a> STRUCTURE=reference.pdb MOLTYPE=protein
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=1-2604  
rmsd: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_m_s_d.html">RMSD</a> REFERENCE=rmsd.pdb TYPE=OPTIMAL

d-r28_l110: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-28</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-110</a>
d-l110_l118: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-110</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-118</a>
d-r85_l112: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-85</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-112</a>
d-r157_l116: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-157</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-116</a>
d-r25_l115: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-25</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-115</a>
d-l111_l112: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-111</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-112</a>
d-r97_l115: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-97</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-115</a>
d-r142_l119: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-142</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-119</a>
d-r154_l113: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-154</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-113</a>
d-r67_l116: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-67</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-116</a>
d-r43_l114: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-43</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-114</a>
d-r34_l114: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-34</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-114</a>
d-r34_l118: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-34</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-118</a>
d-l112_l113: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-112</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-113</a>
d-r49_l116: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-49</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-116</a>
d-l115_l116: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-115</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">CA-116</a>

d1769_1819: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1769,1819
psi_114_1: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=1770,1772,1788,1790


<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ...
LABEL=rc1 ARG=d-r28_l110,d-l110_l118,d-r85_l112,d-r157_l116,d-r25_l115,d-l111_l112,d-r97_l115,d-r142_l119,d-r154_l113,d-r67_l116,d-r43_l114,d-r34_l114,d-r34_l118,d-l112_l113,d-r49_l116,d-l115_l116
COEFFICIENTS=5.690912902355194092e-02,-1.696033775806427002e-01,-1.088943518698215485e-02,-3.811309486627578735e-02,-3.845035657286643982e-02,-3.398763835430145264e-01,6.818664073944091797e-01,1.402324438095092773e-01,5.613043904304504395e-02,1.617383360862731934e-01,8.190712332725524902e-02,-2.790833413600921631e-01,4.563379585742950439e-01,1.509449779987335205e-01,4.242382943630218506e-02,-1.344945281744003296e-01 PERIODIC=NO
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a>



<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ...
LABEL=rc2 ARG=d-r28_l110,d-l110_l118,d-r85_l112,d-r157_l116,d-r25_l115,d-l111_l112,d-r97_l115,d-r142_l119,d-r154_l113,d-r67_l116,d-r43_l114,d-r34_l114,d-r34_l118,d-l112_l113,d-r49_l116,d-l115_l116
COEFFICIENTS=-1.883340626955032349e-01,4.097261726856231689e-01,1.357467919588088989e-01,4.463798403739929199e-01,-1.859887838363647461e-01,2.378992550075054169e-02,-3.209500312805175781e-01,4.577260613441467285e-01,1.797014027833938599e-01,3.510920107364654541e-01,-1.946701705455780029e-01,-2.567137824371457100e-03,1.762732118368148804e-01,-7.985947653651237488e-03,-7.434802502393722534e-02,-3.417430073022842407e-02 PERIODIC=NO
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a>


<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
LABEL=metad
ARG=rc1,rc2
PACE=500
HEIGHT=1.5
SIGMA=0.05,0.05
BIASFACTOR=10.0
<span style="color:blue">#GRID_MIN=1.00,0.21</span>
<span style="color:blue">#GRID_MAX=5.50,4.70</span>
<span style="color:blue">#GRID_BIN=300,300</span>
<span style="color:blue">#REWEIGHTING_NGRID=300,300</span>
TEMP=300.0
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>


<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=rmsd AT=0.5 KAPPA=1000.0 EXP=4 EPS=1 OFFSET=0 LABEL=uwall


<span style="color:blue">#PRINT ARG=d-r28_l110,d-l110_l118,d-r85_l112,d-r157_l116,d-r25_l115,d-l111_l112,d-r97_l115,d-r142_l119,d-r154_l113,d-r67_l116,d-r43_l114,d-r34_l114,d-r34_l118,d-l112_l113,d-r49_l116,d-l115_l116,rc1,rc2,uwall.bias,metad.bias,metad.rbias STRIDE=1 FILE=COLVAR</span>
<span style="color:blue">#PRINT ARG=d1769_1819,psi_114_1,rmsd,uwall.bias,metad.bias,metad.rbias STRIDE=50 FILE=COLVAR_strucutre</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=d-r28_l110,d-l110_l118,d-r85_l112,d-r157_l116,d-r25_l115,d-l111_l112,d-r97_l115,d-r142_l119,d-r154_l113,d-r67_l116,d-r43_l114,d-r34_l114,d-r34_l118,d-l112_l113,d-r49_l116,d-l115_l116,rc1,rc2,uwall.bias,metad.bias STRIDE=1 FILE=COLVAR
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=d1769_1819,psi_114_1,rmsd,uwall.bias,metad.bias STRIDE=50 FILE=COLVAR_strucutre


</pre>{% endraw %}
