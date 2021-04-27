**Project ID:** [plumID:20.008]({{ '/' | absolute_url }}eggs/20/008/)  
**Source:** plumed.dat  
**Originally used with PLUMED version:** 2.5.1  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> LENGTH=A TIME=fs

cnh1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=9 GROUPB=2,3,5,16,29,42,55,68,81,94,107,120,133,146,159,172,185,198,211,224,237,250,263 D_0=0.9 R_0=0.4 NN=6
cnh2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=17 GROUPB=2,3,5,16,29,42,55,68,81,94,107,120,133,146,159,172,185,198,211,224,237,250,263 D_0=0.9 R_0=0.4 NN=6
cnh3: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=30 GROUPB=2,3,5,16,29,42,55,68,81,94,107,120,133,146,159,172,185,198,211,224,237,250,263 D_0=0.9 R_0=0.4 NN=6
cnh4: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=43 GROUPB=2,3,5,16,29,42,55,68,81,94,107,120,133,146,159,172,185,198,211,224,237,250,263 D_0=0.9 R_0=0.4 NN=6
cnh5: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=56 GROUPB=2,3,5,16,29,42,55,68,81,94,107,120,133,146,159,172,185,198,211,224,237,250,263 D_0=0.9 R_0=0.4 NN=6
cnh6: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=69 GROUPB=2,3,5,16,29,42,55,68,81,94,107,120,133,146,159,172,185,198,211,224,237,250,263 D_0=0.9 R_0=0.4 NN=6
cnh7: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=82 GROUPB=2,3,5,16,29,42,55,68,81,94,107,120,133,146,159,172,185,198,211,224,237,250,263 D_0=0.9 R_0=0.4 NN=6
cnh8: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=95 GROUPB=2,3,5,16,29,42,55,68,81,94,107,120,133,146,159,172,185,198,211,224,237,250,263 D_0=0.9 R_0=0.4 NN=6
cnh9: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=108 GROUPB=2,3,5,16,29,42,55,68,81,94,107,120,133,146,159,172,185,198,211,224,237,250,263 D_0=0.9 R_0=0.4 NN=6
cnh10: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=121 GROUPB=2,3,5,16,29,42,55,68,81,94,107,120,133,146,159,172,185,198,211,224,237,250,263 D_0=0.9 R_0=0.4 NN=6
cnh11: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=134 GROUPB=2,3,5,16,29,42,55,68,81,94,107,120,133,146,159,172,185,198,211,224,237,250,263 D_0=0.9 R_0=0.4 NN=6
cnh12: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=147 GROUPB=2,3,5,16,29,42,55,68,81,94,107,120,133,146,159,172,185,198,211,224,237,250,263 D_0=0.9 R_0=0.4 NN=6
cnh13: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=160 GROUPB=2,3,5,16,29,42,55,68,81,94,107,120,133,146,159,172,185,198,211,224,237,250,263 D_0=0.9 R_0=0.4 NN=6
cnh14: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=173 GROUPB=2,3,5,16,29,42,55,68,81,94,107,120,133,146,159,172,185,198,211,224,237,250,263 D_0=0.9 R_0=0.4 NN=6
cnh15: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=186 GROUPB=2,3,5,16,29,42,55,68,81,94,107,120,133,146,159,172,185,198,211,224,237,250,263 D_0=0.9 R_0=0.4 NN=6
cnh16: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=199 GROUPB=2,3,5,16,29,42,55,68,81,94,107,120,133,146,159,172,185,198,211,224,237,250,263 D_0=0.9 R_0=0.4 NN=6
cnh17: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=212 GROUPB=2,3,5,16,29,42,55,68,81,94,107,120,133,146,159,172,185,198,211,224,237,250,263 D_0=0.9 R_0=0.4 NN=6
cnh18: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=225 GROUPB=2,3,5,16,29,42,55,68,81,94,107,120,133,146,159,172,185,198,211,224,237,250,263 D_0=0.9 R_0=0.4 NN=6
cnh19: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=238 GROUPB=2,3,5,16,29,42,55,68,81,94,107,120,133,146,159,172,185,198,211,224,237,250,263 D_0=0.9 R_0=0.4 NN=6
cnh20: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=251 GROUPB=2,3,5,16,29,42,55,68,81,94,107,120,133,146,159,172,185,198,211,224,237,250,263 D_0=0.9 R_0=0.4 NN=6
cnh21: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=264 GROUPB=2,3,5,16,29,42,55,68,81,94,107,120,133,146,159,172,185,198,211,224,237,250,263 D_0=0.9 R_0=0.4 NN=6

cnoh11: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=2 GROUPB=9   D_0=0.9 R_0=0.4 NN=6
cnoh12: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=2 GROUPB=17  D_0=0.9 R_0=0.4 NN=6
cnoh13: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=2 GROUPB=30  D_0=0.9 R_0=0.4 NN=6
cnoh14: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=2 GROUPB=43  D_0=0.9 R_0=0.4 NN=6
cnoh15: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=2 GROUPB=56  D_0=0.9 R_0=0.4 NN=6
cnoh16: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=2 GROUPB=69  D_0=0.9 R_0=0.4 NN=6
cnoh17: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=2 GROUPB=82  D_0=0.9 R_0=0.4 NN=6
cnoh18: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=2 GROUPB=95  D_0=0.9 R_0=0.4 NN=6
cnoh19: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=2 GROUPB=108 D_0=0.9 R_0=0.4 NN=6
cnoh110: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=2 GROUPB=121 D_0=0.9 R_0=0.4 NN=6
cnoh111: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=2 GROUPB=134 D_0=0.9 R_0=0.4 NN=6
cnoh112: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=2 GROUPB=147 D_0=0.9 R_0=0.4 NN=6
cnoh113: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=2 GROUPB=160 D_0=0.9 R_0=0.4 NN=6
cnoh114: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=2 GROUPB=173 D_0=0.9 R_0=0.4 NN=6
cnoh115: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=2 GROUPB=186 D_0=0.9 R_0=0.4 NN=6
cnoh116: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=2 GROUPB=199 D_0=0.9 R_0=0.4 NN=6
cnoh117: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=2 GROUPB=212 D_0=0.9 R_0=0.4 NN=6
cnoh118: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=2 GROUPB=225 D_0=0.9 R_0=0.4 NN=6
cnoh119: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=2 GROUPB=238 D_0=0.9 R_0=0.4 NN=6
cnoh120: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=2 GROUPB=251 D_0=0.9 R_0=0.4 NN=6
cnoh121: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=2 GROUPB=264 D_0=0.9 R_0=0.4 NN=6

cnoh21: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=3 GROUPB=9 D_0=0.9 R_0=0.4 NN=6
cnoh22: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=3 GROUPB=17 D_0=0.9 R_0=0.4 NN=6
cnoh23: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=3 GROUPB=30 D_0=0.9 R_0=0.4 NN=6
cnoh24: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=3 GROUPB=43 D_0=0.9 R_0=0.4 NN=6
cnoh25: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=3 GROUPB=56 D_0=0.9 R_0=0.4 NN=6
cnoh26: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=3 GROUPB=69 D_0=0.9 R_0=0.4 NN=6
cnoh27: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=3 GROUPB=82 D_0=0.9 R_0=0.4 NN=6
cnoh28: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=3 GROUPB=95 D_0=0.9 R_0=0.4 NN=6
cnoh29: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=3 GROUPB=108 D_0=0.9 R_0=0.4 NN=6
cnoh210: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=3 GROUPB=121 D_0=0.9 R_0=0.4 NN=6
cnoh211: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=3 GROUPB=134 D_0=0.9 R_0=0.4 NN=6
cnoh212: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=3 GROUPB=147 D_0=0.9 R_0=0.4 NN=6
cnoh213: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=3 GROUPB=160 D_0=0.9 R_0=0.4 NN=6
cnoh214: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=3 GROUPB=173 D_0=0.9 R_0=0.4 NN=6
cnoh215: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=3 GROUPB=186 D_0=0.9 R_0=0.4 NN=6
cnoh216: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=3 GROUPB=199 D_0=0.9 R_0=0.4 NN=6
cnoh217: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=3 GROUPB=212 D_0=0.9 R_0=0.4 NN=6
cnoh218: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=3 GROUPB=225 D_0=0.9 R_0=0.4 NN=6
cnoh219: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=3 GROUPB=238 D_0=0.9 R_0=0.4 NN=6
cnoh220: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=3 GROUPB=251 D_0=0.9 R_0=0.4 NN=6
cnoh221: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=3 GROUPB=264 D_0=0.9 R_0=0.4 NN=6

cnoh31: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=5 GROUPB=9 D_0=0.9 R_0=0.4 NN=6
cnoh32: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=5 GROUPB=17 D_0=0.9 R_0=0.4 NN=6
cnoh33: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=5 GROUPB=30 D_0=0.9 R_0=0.4 NN=6
cnoh34: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=5 GROUPB=43 D_0=0.9 R_0=0.4 NN=6
cnoh35: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=5 GROUPB=56 D_0=0.9 R_0=0.4 NN=6
cnoh36: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=5 GROUPB=69 D_0=0.9 R_0=0.4 NN=6
cnoh37: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=5 GROUPB=82 D_0=0.9 R_0=0.4 NN=6
cnoh38: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=5 GROUPB=95 D_0=0.9 R_0=0.4 NN=6
cnoh39: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=5 GROUPB=108 D_0=0.9 R_0=0.4 NN=6
cnoh310: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=5 GROUPB=121 D_0=0.9 R_0=0.4 NN=6
cnoh311: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=5 GROUPB=134 D_0=0.9 R_0=0.4 NN=6
cnoh312: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=5 GROUPB=147 D_0=0.9 R_0=0.4 NN=6
cnoh313: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=5 GROUPB=160 D_0=0.9 R_0=0.4 NN=6
cnoh314: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=5 GROUPB=173 D_0=0.9 R_0=0.4 NN=6
cnoh315: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=5 GROUPB=186 D_0=0.9 R_0=0.4 NN=6
cnoh316: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=5 GROUPB=199 D_0=0.9 R_0=0.4 NN=6
cnoh317: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=5 GROUPB=212 D_0=0.9 R_0=0.4 NN=6
cnoh318: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=5 GROUPB=225 D_0=0.9 R_0=0.4 NN=6
cnoh319: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=5 GROUPB=238 D_0=0.9 R_0=0.4 NN=6
cnoh320: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=5 GROUPB=251 D_0=0.9 R_0=0.4 NN=6
cnoh321: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=5 GROUPB=264 D_0=0.9 R_0=0.4 NN=6

tcno11: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh11,cnh1 VAR=x,y FUNC=x/y PERIODIC=NO
tcno12: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh12,cnh2 VAR=x,y FUNC=x/y PERIODIC=NO
tcno13: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh13,cnh3 VAR=x,y FUNC=x/y PERIODIC=NO
tcno14: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh14,cnh4 VAR=x,y FUNC=x/y PERIODIC=NO
tcno15: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh15,cnh5 VAR=x,y FUNC=x/y PERIODIC=NO
tcno16: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh16,cnh6 VAR=x,y FUNC=x/y PERIODIC=NO
tcno17: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh17,cnh7 VAR=x,y FUNC=x/y PERIODIC=NO
tcno18: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh18,cnh8 VAR=x,y FUNC=x/y PERIODIC=NO
tcno19: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh19,cnh9 VAR=x,y FUNC=x/y PERIODIC=NO
tcno110: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh110,cnh10 VAR=x,y FUNC=x/y PERIODIC=NO
tcno111: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh111,cnh11 VAR=x,y FUNC=x/y PERIODIC=NO
tcno112: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh112,cnh12 VAR=x,y FUNC=x/y PERIODIC=NO
tcno113: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh113,cnh13 VAR=x,y FUNC=x/y PERIODIC=NO
tcno114: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh114,cnh14 VAR=x,y FUNC=x/y PERIODIC=NO
tcno115: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh115,cnh15 VAR=x,y FUNC=x/y PERIODIC=NO
tcno116: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh116,cnh16 VAR=x,y FUNC=x/y PERIODIC=NO
tcno117: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh117,cnh17 VAR=x,y FUNC=x/y PERIODIC=NO
tcno118: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh118,cnh18 VAR=x,y FUNC=x/y PERIODIC=NO
tcno119: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh119,cnh19 VAR=x,y FUNC=x/y PERIODIC=NO
tcno120: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh120,cnh20 VAR=x,y FUNC=x/y PERIODIC=NO
tcno121: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh121,cnh21 VAR=x,y FUNC=x/y PERIODIC=NO

tcno21: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh21,cnh1 VAR=x,y FUNC=x/y PERIODIC=NO
tcno22: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh22,cnh2 VAR=x,y FUNC=x/y PERIODIC=NO
tcno23: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh23,cnh3 VAR=x,y FUNC=x/y PERIODIC=NO
tcno24: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh24,cnh4 VAR=x,y FUNC=x/y PERIODIC=NO
tcno25: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh25,cnh5 VAR=x,y FUNC=x/y PERIODIC=NO
tcno26: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh26,cnh6 VAR=x,y FUNC=x/y PERIODIC=NO
tcno27: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh27,cnh7 VAR=x,y FUNC=x/y PERIODIC=NO
tcno28: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh28,cnh8 VAR=x,y FUNC=x/y PERIODIC=NO
tcno29: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh29,cnh9 VAR=x,y FUNC=x/y PERIODIC=NO
tcno210: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh210,cnh10 VAR=x,y FUNC=x/y PERIODIC=NO
tcno211: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh211,cnh11 VAR=x,y FUNC=x/y PERIODIC=NO
tcno212: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh212,cnh12 VAR=x,y FUNC=x/y PERIODIC=NO
tcno213: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh213,cnh13 VAR=x,y FUNC=x/y PERIODIC=NO
tcno214: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh214,cnh14 VAR=x,y FUNC=x/y PERIODIC=NO
tcno215: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh215,cnh15 VAR=x,y FUNC=x/y PERIODIC=NO
tcno216: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh216,cnh16 VAR=x,y FUNC=x/y PERIODIC=NO
tcno217: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh217,cnh17 VAR=x,y FUNC=x/y PERIODIC=NO
tcno218: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh218,cnh18 VAR=x,y FUNC=x/y PERIODIC=NO
tcno219: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh219,cnh19 VAR=x,y FUNC=x/y PERIODIC=NO
tcno220: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh220,cnh20 VAR=x,y FUNC=x/y PERIODIC=NO
tcno221: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh221,cnh21 VAR=x,y FUNC=x/y PERIODIC=NO

tcno31: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh31,cnh1 VAR=x,y FUNC=x/y PERIODIC=NO
tcno32: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh32,cnh2 VAR=x,y FUNC=x/y PERIODIC=NO
tcno33: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh33,cnh3 VAR=x,y FUNC=x/y PERIODIC=NO
tcno34: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh34,cnh4 VAR=x,y FUNC=x/y PERIODIC=NO
tcno35: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh35,cnh5 VAR=x,y FUNC=x/y PERIODIC=NO
tcno36: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh36,cnh6 VAR=x,y FUNC=x/y PERIODIC=NO
tcno37: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh37,cnh7 VAR=x,y FUNC=x/y PERIODIC=NO
tcno38: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh38,cnh8 VAR=x,y FUNC=x/y PERIODIC=NO
tcno39: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh39,cnh9 VAR=x,y FUNC=x/y PERIODIC=NO
tcno310: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh310,cnh10 VAR=x,y FUNC=x/y PERIODIC=NO
tcno311: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh311,cnh11 VAR=x,y FUNC=x/y PERIODIC=NO
tcno312: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh312,cnh12 VAR=x,y FUNC=x/y PERIODIC=NO
tcno313: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh313,cnh13 VAR=x,y FUNC=x/y PERIODIC=NO
tcno314: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh314,cnh14 VAR=x,y FUNC=x/y PERIODIC=NO
tcno315: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh315,cnh15 VAR=x,y FUNC=x/y PERIODIC=NO
tcno316: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh316,cnh16 VAR=x,y FUNC=x/y PERIODIC=NO
tcno317: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh317,cnh17 VAR=x,y FUNC=x/y PERIODIC=NO
tcno318: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh318,cnh18 VAR=x,y FUNC=x/y PERIODIC=NO
tcno319: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh319,cnh19 VAR=x,y FUNC=x/y PERIODIC=NO
tcno320: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh320,cnh20 VAR=x,y FUNC=x/y PERIODIC=NO
tcno321: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ARG=cnoh321,cnh21 VAR=x,y FUNC=x/y PERIODIC=NO

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ...
 LABEL=cno1
 ARG=tcno11,tcno12,tcno13,tcno14,tcno15,tcno16,tcno17,tcno18,tcno19,tcno110,tcno111,tcno112,tcno113,tcno114,tcno115,tcno116,tcno117,tcno118,tcno119,tcno120,tcno121
 VAR=x1,x2,x3,x4,x5,x6,x7,x8,x9,x10,x11,x12,x13,x14,x15,x16,x17,x18,x19,x20,x21
 FUNC=x1+x2+x3+x4+x5+x6+x7+x8+x9+x10+x11+x12+x13+x14+x15+x16+x17+x18+x19+x20+x21
 PERIODIC=NO
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ...
 LABEL=cno2
ARG=tcno21,tcno22,tcno23,tcno24,tcno25,tcno26,tcno27,tcno28,tcno29,tcno210,tcno211,tcno212,tcno213,tcno214,tcno215,tcno216,tcno217,tcno218,tcno219,tcno220,tcno221
 VAR=x1,x2,x3,x4,x5,x6,x7,x8,x9,x10,x11,x12,x13,x14,x15,x16,x17,x18,x19,x20,x21
 FUNC=x1+x2+x3+x4+x5+x6+x7+x8+x9+x10+x11+x12+x13+x14+x15+x16+x17+x18+x19+x20+x21
 PERIODIC=NO
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ...
 LABEL=cno3
ARG=tcno31,tcno32,tcno33,tcno34,tcno35,tcno36,tcno37,tcno38,tcno39,tcno310,tcno311,tcno312,tcno313,tcno314,tcno315,tcno316,tcno317,tcno318,tcno319,tcno320,tcno321
 VAR=x1,x2,x3,x4,x5,x6,x7,x8,x9,x10,x11,x12,x13,x14,x15,x16,x17,x18,x19,x20,x21
 FUNC=x1+x2+x3+x4+x5+x6+x7+x8+x9+x10+x11+x12+x13+x14+x15+x16+x17+x18+x19+x20+x21
 PERIODIC=NO
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a> ...
 LABEL=cno_tot
 ARG=cno1,cno2,cno3
 VAR=x1,x2,x3
 FUNC=x1+x2+x3
 PERIODIC=NO
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_u_s_t_o_m.html">CUSTOM</a>

d1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=2,3,5 GROUPB=9,17,30,43,56,69,82,95,108,121,134,147,160,173,186,199,212,215,238,251,264 MIN={BETA=24.}

metad: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=cno_tot,d1.min PACE=12 HEIGHT=0.4 SIGMA=.1,0.2 FILE=./plumed/HILLS BIASFACTOR=3 TEMP=363 

<span style="color:blue">### PRINT STRIDE=1 ARG=cnh1,cnh2,cnh3,cnh4,cnh5,cnh6,cnh7,cnh8,cnh9,cnh10,cnh11,cnh12,cnh13,cnh14,cnh15,cnh16,cnh17,cnh18,cnh19,cnh20,cnh21,cno_tot,metad.bias FILE=./plumed/COLVAR</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=1 ARG=cno_tot,d1.min,metad.bias FILE=./plumed/COLVAR
</pre>{% endraw %}
