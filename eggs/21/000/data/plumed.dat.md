**Project ID:** [plumID:21.000]({{ '/' | absolute_url }}eggs/21/000/)  
**Source:** plumed.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=1-8843  <span style="color:blue"># include toxin for appropriate RMSD/COM calcs</span>

<span style="color:blue">##############################################</span>
<span style="color:blue">############## DEFINE RESIDUES ###############</span>
<span style="color:blue">##############################################</span>

<span style="color:blue">### toxin (heavy)</span>
toxin: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=8824,8825,8826,8827,8828,8829,8830,8831,8838,8839,8840,8841,8842,8843
toxin_com: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=toxin


LEU383: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6012,6014,6016,6019,6021,6025,6029,6030
LEU383_com: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=LEU383
ILE384: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6031,6033,6035,6037,6041,6044,6048,6049
ILE384_com: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=ILE384
ASN387: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6089,6091,6093,6096,6097,6098,6101,6102
ASN387_com: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=ASN387
PHE399: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6283,6285,6287,6290,6291,6293,6295,6297,6299,6301,6302
PHE399_com: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=PHE399
LEU403: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6344,6346,6348,6351,6353,6357,6361,6362
LEU403_com: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=LEU403
ARG406: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6398,6400,6402,6405,6408,6411,6413,6414,6417,6420,6421
ARG406_com: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=ARG406
TYR407: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6422,6424,6426,6429,6430,6432,6434,6435,6437,6439,6441,6442
TYR407_com: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=TYR407
LYS410: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6479,6481,6483,6486,6489,6492,6495,6499,6500
LYS410_com: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=LYS410
LEU426: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6732,6734,6736,6739,6741,6745,6749,6750
LEU426_com: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=LEU426
VAL429: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6780,6782,6784,6786,6790,6794,6795
VAL429_com: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=VAL429
LEU449: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=7079,7081,7083,7086,7088,7092,7096,7097
LEU449_com: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=LEU449
SER485: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=7653,7655,7657,7660,7662,7663
SER485_com: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=SER485


<span style="color:blue">### calph COM for relevant helices</span>
helix1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=5707,5722,5732,5753,5763,5785,5801,5821,5833,5848,5868,5898,5904,5923,5939,5954,5977,5983,6000,6014,6033,6052,6074,6091,6105,6115,6130,6149,6169,6184
helix2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=6242,6263,6285,6305,6322,6336,6346,6365,6384,6400,6424,6445,6459,6481,6503
helix3: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=7533,7549,7563,7587,7619,7625,7635,7655,7666,7676

<span style="color:blue">###############################################</span>
<span style="color:blue">############### DEFINE COLVARS ################</span>
<span style="color:blue">###############################################</span>

<span style="color:blue">### protein-ligand dists</span>
LEU383_com_dist: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=LEU383_com,toxin_com
ILE384_com_dist: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=ILE384_com,toxin_com
ASN387_com_dist: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=ASN387_com,toxin_com
PHE399_com_dist: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=PHE399_com,toxin_com
LEU403_com_dist: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=LEU403_com,toxin_com
ARG406_com_dist: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=ARG406_com,toxin_com
TYR407_com_dist: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=TYR407_com,toxin_com
LYS410_com_dist: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=LYS410_com,toxin_com
LEU426_com_dist: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=LEU426_com,toxin_com
VAL429_com_dist: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=VAL429_com,toxin_com
LEU449_com_dist: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=LEU449_com,toxin_com
SER485_com_dist: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=SER485_com,toxin_com

<span style="color:blue">### protein-protein backbone distances</span>
h1_h2: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=helix1,helix2
h1_h3: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=helix1,helix3
h2_h3: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=helix2,helix3

<span style="color:blue"># make STRIDE = to your exchange attempt frequency!!!</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FILE=COLVAR ARG=* STRIDE=1
</pre>{% endraw %}
