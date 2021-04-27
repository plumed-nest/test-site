**Project ID:** [plumID:20.011]({{ '/' | absolute_url }}eggs/20/011/)  
**Source:** plumed.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># restart</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=1-8844  <span style="color:blue"># include toxin for appropriate RMSD/COM calcs</span>

<span style="color:blue"># groups</span>
toxin: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=8824,8825,8826,8827,8828,8829,8830,8831,8838,8839,8842,8843,8844

380PRO: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=5967,5968,5971,5974,5977,5979,5980
383LEU: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6012,6014,6016,6019,6021,6025,6029,6030
384ILE: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6031,6033,6035,6037,6041,6044,6048,6049
385LYS: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6050,6052,6054,6057,6060,6063,6066,6070,6071
386GLN: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6072,6074,6076,6079,6082,6083,6084,6087,6088
387ASN: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6089,6091,6093,6096,6097,6098,6101,6102
388CYS: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6103,6105,6107,6110,6111,6112
391PHE: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6147,6149,6151,6154,6155,6157,6159,6161,6163,6165,6166
399PHE: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6283,6285,6287,6290,6291,6293,6295,6297,6299,6301,6302
403LEU: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6344,6346,6348,6351,6353,6357,6361,6362
406ARG: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6398,6400,6402,6405,6408,6411,6413,6414,6417,6420,6421
407TYR: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6422,6424,6426,6429,6430,6432,6434,6435,6437,6439,6441,6442
410LYS: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6479,6481,6483,6486,6489,6492,6495,6499,6500
423SER: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6683,6685,6687,6690,6692,6693
425ASN: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6718,6720,6722,6725,6726,6727,6730,6731
426LEU: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6732,6734,6736,6739,6741,6745,6749,6750
427GLY: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6751,6753,6756,6757
428LYS: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6758,6760,6762,6765,6768,6771,6774,6778,6779
429VAL: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6780,6782,6784,6786,6790,6794,6795
430GLY: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6796,6798,6801,6802
431SER: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6803,6805,6807,6810,6812,6813
433CYS: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6836,6838,6840,6843,6844,6845
434CYS: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6846,6848,6850,6853,6854,6855
441ARG: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6956,6958,6960,6963,6966,6969,6971,6972,6975,6978,6979
442MET: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6980,6982,6984,6987,6990,6991,6995,6996
445ALA: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=7021,7023,7025,7029,7030
446GLU: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=7031,7033,7035,7038,7041,7042,7043,7044,7045
448TYR: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=7058,7060,7062,7065,7066,7068,7070,7071,7073,7075,7077,7078
449LEU: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=7079,7081,7083,7086,7088,7092,7096,7097
452VAL: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=7125,7127,7129,7131,7135,7139,7140
453LEU: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=7141,7143,7145,7148,7150,7154,7158,7159
480ARG: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=7561,7563,7565,7568,7571,7574,7576,7577,7580,7583,7584
481ARG: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=7585,7587,7589,7592,7595,7598,7600,7601,7604,7607,7608
484PHE: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=7633,7635,7637,7640,7641,7643,7645,7647,7649,7651,7652
485SER: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=7653,7655,7657,7660,7662,7663
486ALA: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=7664,7666,7668,7672,7673
487LEU: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=7674,7676,7678,7681,7683,7687,7691,7692

<span style="color:blue"># collective variables</span>
380PRO_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=380PRO GROUPB=toxin D_0=0.27 R_0=0.03
383LEU_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=383LEU GROUPB=toxin D_0=0.27 R_0=0.03
384ILE_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=384ILE GROUPB=toxin D_0=0.27 R_0=0.03
385LYS_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=385LYS GROUPB=toxin D_0=0.27 R_0=0.03
386GLN_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=386GLN GROUPB=toxin D_0=0.27 R_0=0.03
387ASN_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=387ASN GROUPB=toxin D_0=0.27 R_0=0.03
388CYS_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=388CYS GROUPB=toxin D_0=0.27 R_0=0.03
391PHE_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=391PHE GROUPB=toxin D_0=0.27 R_0=0.03
399PHE_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=399PHE GROUPB=toxin D_0=0.27 R_0=0.03
403LEU_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=403LEU GROUPB=toxin D_0=0.27 R_0=0.03
406ARG_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=406ARG GROUPB=toxin D_0=0.27 R_0=0.03
407TYR_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=407TYR GROUPB=toxin D_0=0.27 R_0=0.03
410LYS_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=410LYS GROUPB=toxin D_0=0.27 R_0=0.03
423SER_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=423SER GROUPB=toxin D_0=0.27 R_0=0.03
425ASN_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=425ASN GROUPB=toxin D_0=0.27 R_0=0.03
426LEU_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=426LEU GROUPB=toxin D_0=0.27 R_0=0.03
427GLY_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=427GLY GROUPB=toxin D_0=0.27 R_0=0.03
428LYS_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=428LYS GROUPB=toxin D_0=0.27 R_0=0.03
429VAL_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=429VAL GROUPB=toxin D_0=0.27 R_0=0.03
430GLY_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=430GLY GROUPB=toxin D_0=0.27 R_0=0.03
431SER_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=431SER GROUPB=toxin D_0=0.27 R_0=0.03
433CYS_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=433CYS GROUPB=toxin D_0=0.27 R_0=0.03
434CYS_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=434CYS GROUPB=toxin D_0=0.27 R_0=0.03
441ARG_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=441ARG GROUPB=toxin D_0=0.27 R_0=0.03
442MET_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=442MET GROUPB=toxin D_0=0.27 R_0=0.03
445ALA_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=445ALA GROUPB=toxin D_0=0.27 R_0=0.03
446GLU_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=446GLU GROUPB=toxin D_0=0.27 R_0=0.03
448TYR_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=448TYR GROUPB=toxin D_0=0.27 R_0=0.03
449LEU_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=449LEU GROUPB=toxin D_0=0.27 R_0=0.03
452VAL_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=452VAL GROUPB=toxin D_0=0.27 R_0=0.03
453LEU_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=453LEU GROUPB=toxin D_0=0.27 R_0=0.03
480ARG_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=480ARG GROUPB=toxin D_0=0.27 R_0=0.03
481ARG_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=481ARG GROUPB=toxin D_0=0.27 R_0=0.03
484PHE_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=484PHE GROUPB=toxin D_0=0.27 R_0=0.03
485SER_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=485SER GROUPB=toxin D_0=0.27 R_0=0.03
486ALA_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=486ALA GROUPB=toxin D_0=0.27 R_0=0.03
487LEU_coord: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=487LEU GROUPB=toxin D_0=0.27 R_0=0.03


<span style="color:blue">##############################################</span>
<span style="color:blue">############## DEFINE RESIDUES ###############</span>
<span style="color:blue">##############################################</span>

<span style="color:blue">### toxin (heavy)</span>
toxin_com: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=toxin

<span style="color:blue">### important residues from unbiased + experiment (heavy)</span>
L383: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6012,6014,6016,6019,6021,6025,6029,6030
L383_com: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=L383

N387: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6089,6091,6093,6096,6097,6098,6101,6102
N387_com: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=N387

R406: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6398,6400,6402,6405,6408,6411,6413,6414,6417,6420,6421
R406_com: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=R406

Y407: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6422,6424,6426,6429,6430,6432,6434,6435,6437,6439,6441,6442
Y407_com: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=Y407

K410: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6479,6481,6483,6486,6489,6492,6495,6499,6500
K410_com: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=K410

L426: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6732,6734,6736,6739,6741,6745,6749,6750
L426_com: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=L426

V429: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=6780,6782,6784,6786,6790,6794,6795
V429_com: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=V429

L449: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=7079,7081,7083,7086,7088,7092,7096,7097
L449_com: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=L449

S485: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=7653,7655,7657,7660,7662,7663
S485_com: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=S485

<span style="color:blue">### calph CENTER for relevant helices</span>
helix1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=5707,5722,5732,5753,5763,5785,5801,5821,5833,5848,5868,5898,5904,5923,5939,5954,5977,5983,6000,6014,6033,6052,6074,6091,6105,6115,6130,6149,6169,6184
helix2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=6242,6263,6285,6305,6322,6336,6346,6365,6384,6400,6424,6445,6459,6481,6503
helix3: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=7533,7549,7563,7587,7619,7625,7635,7655,7666,7676

<span style="color:blue">###############################################</span>
<span style="color:blue">############### DEFINE COLVARS ################</span>
<span style="color:blue">###############################################</span>

<span style="color:blue">### protein-ligand dists</span>
L383_com_dist: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=L383_com,toxin_com
L383_dist: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=L383 GROUPB=toxin MIN={BETA=100}
N387_com_dist: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=N387_com,toxin_com
N387_min_dist: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=N387 GROUPB=toxin MIN={BETA=100}
R406_com_dist: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=R406_com,toxin_com
R406_min_dist: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=R406 GROUPB=toxin MIN={BETA=100}
Y407_com_dist: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=Y407_com,toxin_com
Y407_min_dist: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=Y407 GROUPB=toxin MIN={BETA=100}
K410_com_dist: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=K410_com,toxin_com
K410_min_dist: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=K410 GROUPB=toxin MIN={BETA=100}
L426_com_dist: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=L426_com,toxin_com
L426_min_dist: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=L426 GROUPB=toxin MIN={BETA=100}
V429_com_dist: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=V429_com,toxin_com
V429_min_dist: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=V429 GROUPB=toxin MIN={BETA=100}
L449_com_dist: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=L449_com,toxin_com
L449_min_dist: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=L449 GROUPB=toxin MIN={BETA=100}
S485_com_dist: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=S485_com,toxin_com
S485_min_dist: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=S485 GROUPB=toxin MIN={BETA=100}

<span style="color:blue">### protein-protein backbone distances</span>
h1_h2: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=helix1,helix2
h1_h3: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=helix1,helix3
h2_h3: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=helix2,helix3

<span style="color:blue">### linear combination of order parameters</span>
<span style="color:blue">#rc1: COMBINE ARG=L383_dist,N387_dist,R406_dist,Y407_dist,K410_dist,L426_dist,V429_dist,L449_dist,S485_dist,h1_h2,h1_h3,h2_h3 PERIODIC=NO COEFFICIENTS=0,0,0,0,0,0,0,0,0,1,0,0</span>

<span style="color:blue"># make STRIDE = to your exchange attempt frequency!!!</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FILE=COLVAR ARG=* STRIDE=1

</pre>{% endraw %}
