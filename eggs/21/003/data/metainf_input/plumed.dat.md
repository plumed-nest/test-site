**Project ID:** [plumID:21.003]({{ '/' | absolute_url }}eggs/21/003/)  
**Source:** metainf_input/plumed.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># M&M plumed input file</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">MOLINFO</a> MOLTYPE=protein STRUCTURE=master.pdb
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=1-2016

protein-h: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> NDX_FILE=index.ndx NDX_GROUP=Protein-H
solv: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_e_f_s_o_l_v.html">EEFSOLV</a> ATOMS=protein-h NL_STRIDE=20 NL_BUFFER=0.1
Sbias: <a href="https://plumed.github.io/doc-master/user-doc/html/_b_i_a_s_v_a_l_u_e.html">BIASVALUE</a> ARG=solv

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=solv FILE=SOLV

bead1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1,2,3,4,5,18,19 WEIGHTS=14,1,1,1,12,12,16 NOPBC
bead2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=7,10,13,14 WEIGHTS=12,12,32,12 NOPBC
bead3: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=20,22,30,31 WEIGHTS=14,12,12,16 NOPBC
bead4: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=24,27,28,29 WEIGHTS=12,12,16,16 NOPBC
bead5: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=32,34,46,47 WEIGHTS=14,12,12,16 NOPBC
bead6: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=36,38,42 WEIGHTS=12,12,12 NOPBC
bead7: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=48,50,66,67 WEIGHTS=14,12,12,16 NOPBC
bead8: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=52,55,56,57 WEIGHTS=12,12,12,1 NOPBC
bead9: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=62,63,64,65 WEIGHTS=12,1,12,1 NOPBC
bead10: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=58,59,60,61 WEIGHTS=12,1,12,1 NOPBC
bead11: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=68,70,83,84 WEIGHTS=14,12,12,16 NOPBC
bead12: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=72,75,78,79 WEIGHTS=12,12,32,12 NOPBC
bead13: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=85,87,105,106 WEIGHTS=14,12,12,16 NOPBC
bead14: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=89,92,95 WEIGHTS=12,12,12 NOPBC
bead15: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=98,101,102,103,104 WEIGHTS=12,14,1,1,1 NOPBC
bead16: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=107,109,112,113 WEIGHTS=14,12,12,16 NOPBC
bead17: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=114,116,131,132 WEIGHTS=14,12,12,16 NOPBC
bead18: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=118,121,123,127 WEIGHTS=12,12,12,12 NOPBC
bead19: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=133,135,142,143 WEIGHTS=14,12,12,16 NOPBC
bead20: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=137,140 WEIGHTS=12,16 NOPBC
bead21: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=144,146,164,165 WEIGHTS=14,12,12,16 NOPBC
bead22: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=148,151,154 WEIGHTS=12,12,12 NOPBC
bead23: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=157,160,161,162,163 WEIGHTS=12,14,1,1,1 NOPBC
bead24: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=166,168,170,174,175 WEIGHTS=14,12,12,12,16 NOPBC
bead25: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=176,178,196,197 WEIGHTS=14,12,12,16 NOPBC
bead26: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=180,183,186 WEIGHTS=12,12,12 NOPBC
bead27: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=189,192,193,194,195 WEIGHTS=12,14,1,1,1 NOPBC
bead28: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=198,200,211,212 WEIGHTS=14,12,12,16 NOPBC
bead29: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=202,205,208,209,210 WEIGHTS=12,12,12,16,16 NOPBC
bead30: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=213,215,218,219 WEIGHTS=14,12,12,16 NOPBC
bead31: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=220,222,234,235 WEIGHTS=14,12,12,16 NOPBC
bead32: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=224,226,230 WEIGHTS=12,12,12 NOPBC
bead33: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=236,238,250,251 WEIGHTS=14,12,12,16 NOPBC
bead34: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=240,242,246 WEIGHTS=12,12,12 NOPBC
bead35: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=252,254,256,260,261 WEIGHTS=14,12,12,12,16 NOPBC
bead36: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=262,264,266,270,271 WEIGHTS=14,12,12,12,16 NOPBC
bead37: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=272,274,276,280,281 WEIGHTS=14,12,12,12,16 NOPBC
bead38: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=282,284,295,296 WEIGHTS=14,12,12,16 NOPBC
bead39: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=286,289,292,293,294 WEIGHTS=12,12,12,16,16 NOPBC
bead40: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=297,299,317,318 WEIGHTS=14,12,12,16 NOPBC
bead41: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=301,304,307 WEIGHTS=12,12,12 NOPBC
bead42: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=310,313,314,315,316 WEIGHTS=12,14,1,1,1 NOPBC
bead43: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=319,321,331,332 WEIGHTS=14,12,12,16 NOPBC
bead44: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=323,325,326,327 WEIGHTS=12,16,1,12 NOPBC
bead45: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=333,335,353,354 WEIGHTS=14,12,12,16 NOPBC
bead46: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=337,340,343 WEIGHTS=12,12,12 NOPBC
bead47: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=346,349,350,351,352 WEIGHTS=12,14,1,1,1 NOPBC
bead48: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=355,357,370,371 WEIGHTS=14,12,12,16 NOPBC
bead49: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=359,362,365,366,367 WEIGHTS=12,12,12,16,14 NOPBC
bead50: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=372,374,377,378 WEIGHTS=14,12,12,16 NOPBC
bead51: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=379,381,393,394 WEIGHTS=14,12,12,16 NOPBC
bead52: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=383,385,389 WEIGHTS=12,12,12 NOPBC
bead53: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=395,397,399,403,404 WEIGHTS=14,12,12,12,16 NOPBC
bead54: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=405,407,418,419 WEIGHTS=14,12,12,16 NOPBC
bead55: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=409,412,415,416,417 WEIGHTS=12,12,12,16,16 NOPBC
bead56: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=420,422,424,428,429 WEIGHTS=14,12,12,12,16 NOPBC
bead57: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=430,432,434,438,439 WEIGHTS=14,12,12,12,16 NOPBC
bead58: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=440,442,445,446 WEIGHTS=14,12,12,16 NOPBC
bead59: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=447,449,467,468 WEIGHTS=14,12,12,16 NOPBC
bead60: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=451,454,457 WEIGHTS=12,12,12 NOPBC
bead61: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=460,463,464,465,466 WEIGHTS=12,14,1,1,1 NOPBC
bead62: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=469,471,481,482 WEIGHTS=14,12,12,16 NOPBC
bead63: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=473,475,476,477 WEIGHTS=12,16,1,12 NOPBC
bead64: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=483,485,503,504 WEIGHTS=14,12,12,16 NOPBC
bead65: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=487,490,493 WEIGHTS=12,12,12 NOPBC
bead66: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=496,499,500,501,502 WEIGHTS=12,14,1,1,1 NOPBC
bead67: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=505,507,518,519 WEIGHTS=14,12,12,16 NOPBC
bead68: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=509,512,515,516,517 WEIGHTS=12,12,12,16,16 NOPBC
bead69: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=520,522,525,526 WEIGHTS=14,12,12,16 NOPBC
bead70: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=527,529,541,542 WEIGHTS=14,12,12,16 NOPBC
bead71: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=531,533,537 WEIGHTS=12,12,12 NOPBC
bead72: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=543,545,560,561 WEIGHTS=14,12,12,16 NOPBC
bead73: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=547,550,552,556 WEIGHTS=12,12,12,12 NOPBC
bead74: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=562,564,581,582 WEIGHTS=14,12,12,16 NOPBC
bead75: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=566,569,570,571 WEIGHTS=12,12,12,1 NOPBC
bead76: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=577,578,579,580 WEIGHTS=12,1,12,1 NOPBC
bead77: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=572,573,574,575,576 WEIGHTS=12,1,12,16,1 NOPBC
bead78: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=583,585,597,598 WEIGHTS=14,12,12,16 NOPBC
bead79: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=587,589,593 WEIGHTS=12,12,12 NOPBC
bead80: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=599,601,604,605 WEIGHTS=14,12,12,16 NOPBC
bead81: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=606,608,615,616 WEIGHTS=14,12,12,16 NOPBC
bead82: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=610,613 WEIGHTS=12,16 NOPBC
bead83: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=617,619,637,638 WEIGHTS=14,12,12,16 NOPBC
bead84: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=621,624,627 WEIGHTS=12,12,12 NOPBC
bead85: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=630,633,634,635,636 WEIGHTS=12,14,1,1,1 NOPBC
bead86: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=639,641,651,652 WEIGHTS=14,12,12,16 NOPBC
bead87: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=643,645,646,647 WEIGHTS=12,16,1,12 NOPBC
bead88: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=653,655,673,674 WEIGHTS=14,12,12,16 NOPBC
bead89: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=657,660,663 WEIGHTS=12,12,12 NOPBC
bead90: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=666,669,670,671,672 WEIGHTS=12,14,1,1,1 NOPBC
bead91: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=675,677,688,689 WEIGHTS=14,12,12,16 NOPBC
bead92: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=679,682,685,686,687 WEIGHTS=12,12,12,16,16 NOPBC
bead93: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=690,692,695,696 WEIGHTS=14,12,12,16 NOPBC
bead94: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=697,699,711,712 WEIGHTS=14,12,12,16 NOPBC
bead95: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=701,703,707 WEIGHTS=12,12,12 NOPBC
bead96: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=713,715,727,728 WEIGHTS=14,12,12,16 NOPBC
bead97: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=717,719,723 WEIGHTS=12,12,12 NOPBC
bead98: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=729,731,744,745 WEIGHTS=14,12,12,16 NOPBC
bead99: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=733,737 WEIGHTS=12,12 NOPBC
bead100: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=740,741,742,743 WEIGHTS=14,1,12,1 NOPBC
bead101: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=736,738,739 WEIGHTS=14,12,1 NOPBC
bead102: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=746,748,751,752 WEIGHTS=14,12,12,16 NOPBC
bead103: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=753,755,767,768 WEIGHTS=14,12,12,16 NOPBC
bead104: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=757,759,763 WEIGHTS=12,12,12 NOPBC
bead105: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=769,771,773,777,778 WEIGHTS=14,12,12,12,16 NOPBC
bead106: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=779,781,791,792 WEIGHTS=14,12,12,16 NOPBC
bead107: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=783,785,786,787 WEIGHTS=12,16,1,12 NOPBC
bead108: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=793,795,807,808 WEIGHTS=14,12,12,16 NOPBC
bead109: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=797,799,803 WEIGHTS=12,12,12 NOPBC
bead110: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=809,811,813,817,818 WEIGHTS=14,12,12,12,16 NOPBC
bead111: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=819,821,832,833 WEIGHTS=14,12,12,16 NOPBC
bead112: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=823,826,829,830,831 WEIGHTS=12,12,12,16,16 NOPBC
bead113: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=834,836,854,855 WEIGHTS=14,12,12,16 NOPBC
bead114: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=838,841,844 WEIGHTS=12,12,12 NOPBC
bead115: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=847,850,851,852,853 WEIGHTS=12,14,1,1,1 NOPBC
bead116: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=856,858,868,869 WEIGHTS=14,12,12,16 NOPBC
bead117: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=860,862,863,864 WEIGHTS=12,16,1,12 NOPBC
bead118: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=870,872,890,891 WEIGHTS=14,12,12,16 NOPBC
bead119: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=874,877,880 WEIGHTS=12,12,12 NOPBC
bead120: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=883,886,887,888,889 WEIGHTS=12,14,1,1,1 NOPBC
bead121: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=892,894,905,906 WEIGHTS=14,12,12,16 NOPBC
bead122: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=896,899,902,903,904 WEIGHTS=12,12,12,16,16 NOPBC
bead123: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=907,909,922,923 WEIGHTS=14,12,12,16 NOPBC
bead124: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=911,914,917,918,919 WEIGHTS=12,12,12,16,14 NOPBC
bead125: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=924,926,938,939 WEIGHTS=14,12,12,16 NOPBC
bead126: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=928,930,934 WEIGHTS=12,12,12 NOPBC
bead127: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=940,942,952,953 WEIGHTS=14,12,12,16 NOPBC
bead128: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=944,946,947,948 WEIGHTS=12,16,1,12 NOPBC
bead129: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=954,956,966,967 WEIGHTS=14,12,12,16 NOPBC
bead130: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=958,961,962,963 WEIGHTS=12,12,16,14 NOPBC
bead131: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=968,970,982,983 WEIGHTS=14,12,12,16 NOPBC
bead132: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=972,974,978 WEIGHTS=12,12,12 NOPBC
bead133: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=984,986,989,990 WEIGHTS=14,12,12,16 NOPBC
bead134: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=991,993,996,997 WEIGHTS=14,12,12,16 NOPBC
bead135: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=998,1000,1002,1006,1007 WEIGHTS=14,12,12,12,16 NOPBC
bead136: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1008,1010,1022,1023 WEIGHTS=14,12,12,16 NOPBC
bead137: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1012,1014,1018 WEIGHTS=12,12,12 NOPBC
bead138: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1024,1026,1038,1039 WEIGHTS=14,12,12,16 NOPBC
bead139: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1028,1030,1034 WEIGHTS=12,12,12 NOPBC
bead140: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1040,1042,1052,1053 WEIGHTS=14,12,12,16 NOPBC
bead141: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1044,1046,1047,1048 WEIGHTS=12,16,1,12 NOPBC
bead142: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1054,1056,1059,1060 WEIGHTS=14,12,12,16 NOPBC
bead143: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1061,1063,1075,1076 WEIGHTS=14,12,12,16 NOPBC
bead144: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1065,1067,1071 WEIGHTS=12,12,12 NOPBC
bead145: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1077,1079,1089,1090 WEIGHTS=14,12,12,16 NOPBC
bead146: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1081,1083,1084,1085 WEIGHTS=12,16,1,12 NOPBC
bead147: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1091,1093,1095,1099,1100 WEIGHTS=14,12,12,12,16 NOPBC
bead148: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1101,1103,1115,1116 WEIGHTS=14,12,12,16 NOPBC
bead149: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1105,1107,1111 WEIGHTS=12,12,12 NOPBC
bead150: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1117,1119,1121,1125,1126 WEIGHTS=14,12,12,12,16 NOPBC
bead151: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1127,1129,1142,1143 WEIGHTS=14,12,12,16 NOPBC
bead152: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1131,1134,1137,1138,1139 WEIGHTS=12,12,12,16,14 NOPBC
bead153: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1144,1146,1164,1165 WEIGHTS=14,12,12,16 NOPBC
bead154: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1148,1151,1154 WEIGHTS=12,12,12 NOPBC
bead155: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1157,1160,1161,1162,1163 WEIGHTS=12,14,1,1,1 NOPBC
bead156: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1166,1168,1178,1179 WEIGHTS=14,12,12,16 NOPBC
bead157: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1170,1172,1173,1174 WEIGHTS=12,16,1,12 NOPBC
bead158: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1180,1182,1194,1195 WEIGHTS=14,12,12,16 NOPBC
bead159: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1184,1186,1190 WEIGHTS=12,12,12 NOPBC
bead160: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1196,1198,1209,1210 WEIGHTS=14,12,12,16 NOPBC
bead161: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1200,1203,1206,1207,1208 WEIGHTS=12,12,12,16,16 NOPBC
bead162: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1211,1213,1216,1217 WEIGHTS=14,12,12,16 NOPBC
bead163: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1218,1220,1222,1226,1227 WEIGHTS=14,12,12,12,16 NOPBC
bead164: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1228,1230,1233,1234 WEIGHTS=14,12,12,16 NOPBC
bead165: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1235,1237,1244,1245 WEIGHTS=14,12,12,16 NOPBC
bead166: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1239,1242 WEIGHTS=12,16 NOPBC
bead167: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1246,1248,1263,1264 WEIGHTS=14,12,12,16 NOPBC
bead168: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1250,1252,1256,1259 WEIGHTS=12,12,12,12 NOPBC
bead169: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1265,1267,1269,1273,1274 WEIGHTS=14,12,12,12,16 NOPBC
bead170: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1275,1277,1279,1283,1284 WEIGHTS=14,12,12,12,16 NOPBC
bead171: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1285,1287,1289,1293,1294 WEIGHTS=14,12,12,12,16 NOPBC
bead172: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1295,1297,1307,1308 WEIGHTS=14,12,12,16 NOPBC
bead173: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1299,1301,1302,1303 WEIGHTS=12,16,1,12 NOPBC
bead174: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1309,1311,1314,1315 WEIGHTS=14,12,12,16 NOPBC
bead175: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1316,1318,1334,1335 WEIGHTS=14,12,12,16 NOPBC
bead176: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1320,1323,1324,1325 WEIGHTS=12,12,12,1 NOPBC
bead177: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1330,1331,1332,1333 WEIGHTS=12,1,12,1 NOPBC
bead178: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1326,1327,1328,1329 WEIGHTS=12,1,12,1 NOPBC
bead179: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1336,1338,1350,1351 WEIGHTS=14,12,12,16 NOPBC
bead180: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1340,1342,1346 WEIGHTS=12,12,12 NOPBC
bead181: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1352,1354,1372,1373 WEIGHTS=14,12,12,16 NOPBC
bead182: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1356,1359,1362 WEIGHTS=12,12,12 NOPBC
bead183: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1365,1368,1369,1370,1371 WEIGHTS=12,14,1,1,1 NOPBC
bead184: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1374,1376,1394,1395 WEIGHTS=14,12,12,16 NOPBC
bead185: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1378,1381,1384 WEIGHTS=12,12,12 NOPBC
bead186: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1387,1390,1391,1392,1393 WEIGHTS=12,14,1,1,1 NOPBC
bead187: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1396,1398,1406,1407 WEIGHTS=14,12,12,16 NOPBC
bead188: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1400,1403,1404,1405 WEIGHTS=12,12,16,16 NOPBC
bead189: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1408,1410,1423,1424 WEIGHTS=14,12,12,16 NOPBC
bead190: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1412,1415,1418,1419,1420 WEIGHTS=12,12,12,16,14 NOPBC
bead191: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1425,1427,1442,1443 WEIGHTS=14,12,12,16 NOPBC
bead192: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1429,1432,1434,1438 WEIGHTS=12,12,12,12 NOPBC
bead193: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1444,1446,1449,1450 WEIGHTS=14,12,12,16 NOPBC
bead194: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1451,1453,1471,1472 WEIGHTS=14,12,12,16 NOPBC
bead195: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1455,1458,1461 WEIGHTS=12,12,12 NOPBC
bead196: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1464,1467,1468,1469,1470 WEIGHTS=12,14,1,1,1 NOPBC
bead197: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1473,1475,1485,1486 WEIGHTS=14,12,12,16 NOPBC
bead198: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1477,1480,1481,1482 WEIGHTS=12,12,16,14 NOPBC
bead199: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1487,1489,1500,1501 WEIGHTS=14,12,12,16 NOPBC
bead200: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1491,1494,1497,1498,1499 WEIGHTS=12,12,12,16,16 NOPBC
bead201: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1502,1504,1515,1516 WEIGHTS=14,12,12,16 NOPBC
bead202: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1506,1509,1512,1513,1514 WEIGHTS=12,12,12,16,16 NOPBC
bead203: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1517,1519,1522,1523 WEIGHTS=14,12,12,16 NOPBC
bead204: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1524,1526,1528,1532,1533 WEIGHTS=14,12,12,12,16 NOPBC
bead205: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1534,1538,1546,1547 WEIGHTS=14,12,12,16 NOPBC
bead206: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1535,1540,1543 WEIGHTS=12,12,12 NOPBC
bead207: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1548,1550,1563,1564 WEIGHTS=14,12,12,16 NOPBC
bead208: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1552,1555,1558,1559,1560 WEIGHTS=12,12,12,16,14 NOPBC
bead209: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1565,1567,1578,1579 WEIGHTS=14,12,12,16 NOPBC
bead210: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1569,1572,1575,1576,1577 WEIGHTS=12,12,12,16,16 NOPBC
bead211: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1580,1582,1585,1586 WEIGHTS=14,12,12,16 NOPBC
bead212: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1587,1589,1604,1605 WEIGHTS=14,12,12,16 NOPBC
bead213: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1591,1593,1597,1600 WEIGHTS=12,12,12,12 NOPBC
bead214: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1606,1608,1623,1624 WEIGHTS=14,12,12,16 NOPBC
bead215: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1610,1613,1615,1619 WEIGHTS=12,12,12,12 NOPBC
bead216: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1625,1627,1638,1639 WEIGHTS=14,12,12,16 NOPBC
bead217: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1629,1632,1635,1636,1637 WEIGHTS=12,12,12,16,16 NOPBC
bead218: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1640,1642,1650,1651 WEIGHTS=14,12,12,16 NOPBC
bead219: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1644,1647,1648,1649 WEIGHTS=12,12,16,16 NOPBC
bead220: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1652,1654,1667,1668 WEIGHTS=14,12,12,16 NOPBC
bead221: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1656,1659,1662,1663 WEIGHTS=12,12,32,12 NOPBC
bead222: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1669,1673,1681,1682 WEIGHTS=14,12,12,16 NOPBC
bead223: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1670,1675,1678 WEIGHTS=12,12,12 NOPBC
bead224: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1683,1685,1697,1698 WEIGHTS=14,12,12,16 NOPBC
bead225: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1687,1689,1693 WEIGHTS=12,12,12 NOPBC
bead226: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1699,1701,1709,1710 WEIGHTS=14,12,12,16 NOPBC
bead227: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1703,1706,1707,1708 WEIGHTS=12,12,16,16 NOPBC
bead228: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1711,1715,1723,1724 WEIGHTS=14,12,12,16 NOPBC
bead229: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1712,1717,1720 WEIGHTS=12,12,12 NOPBC
bead230: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1725,1727,1735,1736 WEIGHTS=14,12,12,16 NOPBC
bead231: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1729,1732,1733,1734 WEIGHTS=12,12,16,16 NOPBC
bead232: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1737,1739,1749,1750 WEIGHTS=14,12,12,16 NOPBC
bead233: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1741,1744,1745,1746 WEIGHTS=12,12,16,14 NOPBC
bead234: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1751,1753,1764,1765 WEIGHTS=14,12,12,16 NOPBC
bead235: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1755,1758,1761,1762,1763 WEIGHTS=12,12,12,16,16 NOPBC
bead236: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1766,1768,1770,1774,1775 WEIGHTS=14,12,12,12,16 NOPBC
bead237: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1776,1778,1795,1796 WEIGHTS=14,12,12,16 NOPBC
bead238: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1780,1783,1784,1785 WEIGHTS=12,12,12,1 NOPBC
bead239: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1791,1792,1793,1794 WEIGHTS=12,1,12,1 NOPBC
bead240: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1786,1787,1788,1789,1790 WEIGHTS=12,1,12,16,1 NOPBC
bead241: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1797,1799,1810,1811 WEIGHTS=14,12,12,16 NOPBC
bead242: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1801,1804,1807,1808,1809 WEIGHTS=12,12,12,16,16 NOPBC
bead243: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1812,1814,1827,1828 WEIGHTS=14,12,12,16 NOPBC
bead244: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1816,1819,1822,1823 WEIGHTS=12,12,32,12 NOPBC
bead245: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1829,1833,1841,1842 WEIGHTS=14,12,12,16 NOPBC
bead246: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1830,1835,1838 WEIGHTS=12,12,12 NOPBC
bead247: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1843,1845,1852,1853 WEIGHTS=14,12,12,16 NOPBC
bead248: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1847,1850 WEIGHTS=12,16 NOPBC
bead249: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1854,1856,1867,1868 WEIGHTS=14,12,12,16 NOPBC
bead250: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1858,1861,1864,1865,1866 WEIGHTS=12,12,12,16,16 NOPBC
bead251: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1869,1871,1882,1883 WEIGHTS=14,12,12,16 NOPBC
bead252: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1873,1876,1879,1880,1881 WEIGHTS=12,12,12,16,16 NOPBC
bead253: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1884,1886,1889,1890 WEIGHTS=14,12,12,16 NOPBC
bead254: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1891,1893,1910,1911 WEIGHTS=14,12,12,16 NOPBC
bead255: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1895,1898,1899,1900 WEIGHTS=12,12,12,1 NOPBC
bead256: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1906,1907,1908,1909 WEIGHTS=12,1,12,1 NOPBC
bead257: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1901,1902,1903,1904,1905 WEIGHTS=12,1,12,16,1 NOPBC
bead258: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1912,1914,1927,1928 WEIGHTS=14,12,12,16 NOPBC
bead259: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1916,1919,1922,1923,1924 WEIGHTS=12,12,12,16,14 NOPBC
bead260: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1929,1931,1939,1940 WEIGHTS=14,12,12,16 NOPBC
bead261: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1933,1936,1937,1938 WEIGHTS=12,12,16,16 NOPBC
bead262: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1941,1943,1960,1961 WEIGHTS=14,12,12,16 NOPBC
bead263: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1945,1948,1949,1950 WEIGHTS=12,12,12,1 NOPBC
bead264: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1956,1957,1958,1959 WEIGHTS=12,1,12,1 NOPBC
bead265: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1951,1952,1953,1954,1955 WEIGHTS=12,1,12,16,1 NOPBC
bead266: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1962,1964,1975,1976 WEIGHTS=14,12,12,16 NOPBC
bead267: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1966,1969,1972,1973,1974 WEIGHTS=12,12,12,16,16 NOPBC
bead268: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1977,1981,1989,1990 WEIGHTS=14,12,12,16 NOPBC
bead269: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1978,1983,1986 WEIGHTS=12,12,12 NOPBC
bead270: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1991,1993,2004,2005 WEIGHTS=14,12,12,16 NOPBC
bead271: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=1995,1998,2001,2002,2003 WEIGHTS=12,12,12,16,16 NOPBC
bead272: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=2006,2008,2010,2014 WEIGHTS=14,12,12,12 NOPBC

<span style="color:blue">#MetaD CVs </span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_r_m_s_d.html">ALPHARMSD</a> ...
RESIDUES=1-6 TYPE=OPTIMAL LESS_THAN={RATIONAL R_0=0.08 NN=8 MM=12}
LABEL=ab1
... <a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_r_m_s_d.html">ALPHARMSD</a> 
<a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_r_m_s_d.html">ALPHARMSD</a> ...
RESIDUES=7-12 TYPE=OPTIMAL LESS_THAN={RATIONAL R_0=0.08 NN=8 MM=12}
LABEL=ab2
... <a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_r_m_s_d.html">ALPHARMSD</a> 
<a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_r_m_s_d.html">ALPHARMSD</a> ...
RESIDUES=13-18 TYPE=OPTIMAL LESS_THAN={RATIONAL R_0=0.08 NN=8 MM=12}
LABEL=ab3
... <a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_r_m_s_d.html">ALPHARMSD</a> 
<a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_r_m_s_d.html">ALPHARMSD</a> ...
RESIDUES=19-24 TYPE=OPTIMAL LESS_THAN={RATIONAL R_0=0.08 NN=8 MM=12}
LABEL=ab4
... <a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_r_m_s_d.html">ALPHARMSD</a> 
<a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_r_m_s_d.html">ALPHARMSD</a> ...
RESIDUES=25-30 TYPE=OPTIMAL LESS_THAN={RATIONAL R_0=0.08 NN=8 MM=12}
LABEL=ab5
... <a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_r_m_s_d.html">ALPHARMSD</a> 
<a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_r_m_s_d.html">ALPHARMSD</a> ...
RESIDUES=26-36 TYPE=OPTIMAL LESS_THAN={RATIONAL R_0=0.08 NN=8 MM=12}
LABEL=ab6
... <a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_r_m_s_d.html">ALPHARMSD</a> 
<a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_r_m_s_d.html">ALPHARMSD</a> ...
RESIDUES=37-42 TYPE=OPTIMAL LESS_THAN={RATIONAL R_0=0.08 NN=8 MM=12}
LABEL=ab7
... <a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_r_m_s_d.html">ALPHARMSD</a> 
<a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_r_m_s_d.html">ALPHARMSD</a> ...
RESIDUES=43-48 TYPE=OPTIMAL LESS_THAN={RATIONAL R_0=0.08 NN=8 MM=12}
LABEL=ab8
... <a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_r_m_s_d.html">ALPHARMSD</a> 
<a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_r_m_s_d.html">ALPHARMSD</a> ...
RESIDUES=49-54 TYPE=OPTIMAL LESS_THAN={RATIONAL R_0=0.08 NN=8 MM=12}
LABEL=ab9
... <a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_r_m_s_d.html">ALPHARMSD</a>
<a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_r_m_s_d.html">ALPHARMSD</a> ...
RESIDUES=55-60 TYPE=OPTIMAL LESS_THAN={RATIONAL R_0=0.08 NN=8 MM=12}
LABEL=ab10
... <a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_r_m_s_d.html">ALPHARMSD</a>
<a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_r_m_s_d.html">ALPHARMSD</a> ...
RESIDUES=61-66 TYPE=OPTIMAL LESS_THAN={RATIONAL R_0=0.08 NN=8 MM=12}
LABEL=ab11
... <a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_r_m_s_d.html">ALPHARMSD</a>

<span style="color:blue">#radius of gyration</span>
Calpha: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> NDX_FILE=index.ndx NDX_GROUP=C-alpha
<a href="https://plumed.github.io/doc-master/user-doc/html/_g_y_r_a_t_i_o_n.html">GYRATION</a> TYPE=RADIUS ATOMS=Calpha LABEL=rg NOPBC 

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_b_m_e_t_a_d.html">PBMETAD</a> ...
LABEL=bias
ARG=rg,ab1.lessthan,ab2.lessthan,ab3.lessthan,ab4.lessthan,ab5.lessthan,ab6.lessthan,ab7.lessthan,ab8.lessthan,ab9.lessthan,ab10.lessthan,ab11.lessthan

HEIGHT=0.1
PACE=200
BIASFACTOR=20
<span style="color:blue">#ADAPTIVE=DIFF</span>
<span style="color:blue">#GRID_WFILES=GRID.0,GRID.1,GRID.2,GRID.3,GRID.4,GRID.5,GRID.6,GRID.7,GRID.8,GRID.9,GRID.10,GRID.11</span>
GRID_WSTRIDE=2000
<span style="color:blue">#GRID_RFILES=GRID.0,GRID.1,GRID.2,GRID.3,GRID.4,GRID.5,GRID.6,GRID.7,GRID.8,GRID.9,GRID.10,GRID.11</span>

SIGMA=0.2,0.1,0.1,0.1,0.1,0.1,0.1,0.1,0.1,0.1,0.1,0.1
GRID_MIN=-10,-20,-20,-20,-20,-20,-20,-20,-20,-20,-20,-20
GRID_MAX=50,20,20,20,20,20,20,20,20,20,20,20
UPDATE_FROM=1
... <a href="https://plumed.github.io/doc-master/user-doc/html/_p_b_m_e_t_a_d.html">PBMETAD</a>


<span style="color:blue"># metainf</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_s_a_x_s.html">SAXS</a> ...
LABEL=test2
ATOMS=2017-2288
MARTINI
NOPBC

<span style="color:blue">#ADDEXPVALUES</span>
<span style="color:blue">#RESCALE</span>
<span style="color:blue">#NUMQ=19</span>
<span style="color:blue">#SCEXP=1680</span>
SCALEINT=1680

QVALUE1=0.01100010
QVALUE2=0.02127519
QVALUE3=0.03155028
QVALUE4=0.04182537
QVALUE5=0.05210046
QVALUE6=0.06237555
QVALUE7=0.07265064
QVALUE8=0.08292573
QVALUE9=0.09320082
QVALUE10=0.10347591
QVALUE11=0.11375100
QVALUE12=0.12402609
QVALUE13=0.13430118
QVALUE14=0.14457627
QVALUE15=0.15485136
QVALUE16=0.16512645
QVALUE17=0.17540154
QVALUE18=0.18567663
QVALUE19=0.19595172

EXPINT1=1667.55
EXPINT2=1439.16
EXPINT3=1157.47
EXPINT4=897.121
EXPINT5=685.309
EXPINT6=524.694
EXPINT7=407.433
EXPINT8=323.015
EXPINT9=261.99
EXPINT10=217.205
EXPINT11=183.73
EXPINT12=158.26
EXPINT13=138.495
EXPINT14=122.736
EXPINT15=109.728
EXPINT16=98.6766
EXPINT17=89.2737
EXPINT18=81.5691
EXPINT19=75.5662
... <a href="https://plumed.github.io/doc-master/user-doc/html/_s_a_x_s.html">SAXS</a>


<span style="color:blue">#lsaxs: STATS ARG=(test2\.q_.*) PARARG=(test2\.exp_.*)</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_i_n_f_e_r_e_n_c_e.html">METAINFERENCE</a> ...
SCALEDATA
<span style="color:blue">#NOISETYPE=MOUTLIERS</span>
NOISETYPE=MGAUSS
AVERAGING=200
<span style="color:blue">#ARG=(test2\.q_.*),bias.bias REWEIGHT PARARG=(test2\.exp_.*)</span>
SCALE_PRIOR=FLAT
<span style="color:blue">#SCALE0=1.00 SCALE_MIN=0.995 SCALE_MAX=1.005 DSCALE=0.001</span>
SCALE0=1.00 SCALE_MIN=0.5 SCALE_MAX=2.0 DSCALE=0.001
SIGMA0=0.1 SIGMA_MIN=0. SIGMA_MAX=30 DSIGMA=0.1
ADDOFFSET
OFFSET_PRIOR=FLAT
<span style="color:blue">#OFFSET0=-5 OFFSET_MIN=-6 OFFSET_MAX=4 DOFFSET=0.01</span>
OFFSET0=-9 OFFSET_MIN=-20 OFFSET_MAX=20 DOFFSET=0.01
OPTSIGMAMEAN=SEM
LABEL=bq
WRITE_STRIDE=10000
STRIDE=10
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_i_n_f_e_r_e_n_c_e.html">METAINFERENCE</a>

<span style="color:blue">#ensaxs: ENSEMBLE ARG=(test2\.q_.*),bias.bias REWEIGHT</span>
<span style="color:blue">#statsq: STATS ARG=(ensaxs\.test2\.q_.*) PARARG=(test2\.exp_.*)</span>

<span style="color:blue">#bq: RESTRAINT ARG=statsq.corr AT=0 KAPPA=0 SLOPE=-1000000 STRIDE=2</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=1000
<span style="color:blue">#PRINT FILE=q.dat ARG=statsq.*,lsaxs.* STRIDE=100</span>
<span style="color:blue">#PRINT ARG=(test2\.q_.*) FILE=CV.dat STRIDE=100</span>
<span style="color:blue">#PRINT FILE=ENSAXS ARG=(ensaxs\.test2\.q_.*) STRIDE=100</span>
<span style="color:blue">#PRINT FILE=RESTRAINTS ARG=bq.* STRIDE=100</span>
<span style="color:blue">#STRIDE=100 FILE=colvar</span>
<span style="color:blue">#PRINT ARG=rg,ab1,ab2,ab3,ab4,ab5,ab6,ab7,ab8,ab9,ab10,ab11</span>
</pre>{% endraw %}
