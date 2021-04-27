**Project ID:** [plumID:19.027]({{ '/' | absolute_url }}eggs/19/027/)  
**Source:** MulticanonicalSimulations/Multicanonical/Analysis/Reweight/plumed.dat  
**Originally used with PLUMED version:** 2.4-dev  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>

energy: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_a_d.html">READ</a> FILE=../COLVARtrim VALUES=energy  IGNORE_TIME
b1: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_a_d.html">READ</a> FILE=../COLVARtrim VALUES=b1.bias  IGNORE_TIME

energyshift: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=energy PARAMETERS=-24300 PERIODIC=NO
weights: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__b_i_a_s.html">REWEIGHT_BIAS</a> TEMP=500 ARG=b1.bias

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=* FILE=COLVAR STRIDE=1 FMT=%16.10f

weights400: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=400 ENERGY=energyshift
avg-400: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights400 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-400,weights,weights400 FILE=COLVAR400 STRIDE=2000 FMT=%16.10f

weights405: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=405 ENERGY=energyshift
avg-405: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights405 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-405,weights,weights405 FILE=COLVAR405 STRIDE=2000 FMT=%16.10f

weights410: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=410 ENERGY=energyshift
avg-410: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights410 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-410,weights,weights410 FILE=COLVAR410 STRIDE=2000 FMT=%16.10f

weights415: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=415 ENERGY=energyshift
avg-415: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights415 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-415,weights,weights415 FILE=COLVAR415 STRIDE=2000 FMT=%16.10f

weights420: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=420 ENERGY=energyshift
avg-420: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights420 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-420,weights,weights420 FILE=COLVAR420 STRIDE=2000 FMT=%16.10f

weights425: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=425 ENERGY=energyshift
avg-425: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights425 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-425,weights,weights425 FILE=COLVAR425 STRIDE=2000 FMT=%16.10f

weights430: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=430 ENERGY=energyshift
avg-430: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights430 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-430,weights,weights430 FILE=COLVAR430 STRIDE=2000 FMT=%16.10f

weights435: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=435 ENERGY=energyshift
avg-435: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights435 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-435,weights,weights435 FILE=COLVAR435 STRIDE=2000 FMT=%16.10f

weights440: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=440 ENERGY=energyshift
avg-440: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights440 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-440,weights,weights440 FILE=COLVAR440 STRIDE=2000 FMT=%16.10f

weights445: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=445 ENERGY=energyshift
avg-445: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights445 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-445,weights,weights445 FILE=COLVAR445 STRIDE=2000 FMT=%16.10f

weights450: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=450 ENERGY=energyshift
avg-450: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights450 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-450,weights,weights450 FILE=COLVAR450 STRIDE=2000 FMT=%16.10f

weights455: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=455 ENERGY=energyshift
avg-455: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights455 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-455,weights,weights455 FILE=COLVAR455 STRIDE=2000 FMT=%16.10f

weights460: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=460 ENERGY=energyshift
avg-460: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights460 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-460,weights,weights460 FILE=COLVAR460 STRIDE=2000 FMT=%16.10f

weights465: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=465 ENERGY=energyshift
avg-465: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights465 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-465,weights,weights465 FILE=COLVAR465 STRIDE=2000 FMT=%16.10f

weights470: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=470 ENERGY=energyshift
avg-470: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights470 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-470,weights,weights470 FILE=COLVAR470 STRIDE=2000 FMT=%16.10f

weights475: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=475 ENERGY=energyshift
avg-475: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights475 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-475,weights,weights475 FILE=COLVAR475 STRIDE=2000 FMT=%16.10f

weights480: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=480 ENERGY=energyshift
avg-480: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights480 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-480,weights,weights480 FILE=COLVAR480 STRIDE=2000 FMT=%16.10f

weights485: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=485 ENERGY=energyshift
avg-485: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights485 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-485,weights,weights485 FILE=COLVAR485 STRIDE=2000 FMT=%16.10f

weights490: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=490 ENERGY=energyshift
avg-490: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights490 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-490,weights,weights490 FILE=COLVAR490 STRIDE=2000 FMT=%16.10f

weights495: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=495 ENERGY=energyshift
avg-495: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights495 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-495,weights,weights495 FILE=COLVAR495 STRIDE=2000 FMT=%16.10f

weights500: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=500 ENERGY=energyshift
avg-500: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights500 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-500,weights,weights500 FILE=COLVAR500 STRIDE=2000 FMT=%16.10f

weights505: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=505 ENERGY=energyshift
avg-505: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights505 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-505,weights,weights505 FILE=COLVAR505 STRIDE=2000 FMT=%16.10f

weights510: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=510 ENERGY=energyshift
avg-510: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights510 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-510,weights,weights510 FILE=COLVAR510 STRIDE=2000 FMT=%16.10f

weights515: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=515 ENERGY=energyshift
avg-515: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights515 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-515,weights,weights515 FILE=COLVAR515 STRIDE=2000 FMT=%16.10f

weights520: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=520 ENERGY=energyshift
avg-520: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights520 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-520,weights,weights520 FILE=COLVAR520 STRIDE=2000 FMT=%16.10f

weights525: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=525 ENERGY=energyshift
avg-525: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights525 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-525,weights,weights525 FILE=COLVAR525 STRIDE=2000 FMT=%16.10f

weights530: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=530 ENERGY=energyshift
avg-530: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights530 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-530,weights,weights530 FILE=COLVAR530 STRIDE=2000 FMT=%16.10f

weights535: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=535 ENERGY=energyshift
avg-535: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights535 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-535,weights,weights535 FILE=COLVAR535 STRIDE=2000 FMT=%16.10f

weights540: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=540 ENERGY=energyshift
avg-540: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights540 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-540,weights,weights540 FILE=COLVAR540 STRIDE=2000 FMT=%16.10f

weights545: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=545 ENERGY=energyshift
avg-545: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights545 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-545,weights,weights545 FILE=COLVAR545 STRIDE=2000 FMT=%16.10f

weights550: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=550 ENERGY=energyshift
avg-550: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights550 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-550,weights,weights550 FILE=COLVAR550 STRIDE=2000 FMT=%16.10f

weights555: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=555 ENERGY=energyshift
avg-555: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights555 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-555,weights,weights555 FILE=COLVAR555 STRIDE=2000 FMT=%16.10f

weights560: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=560 ENERGY=energyshift
avg-560: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights560 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-560,weights,weights560 FILE=COLVAR560 STRIDE=2000 FMT=%16.10f

weights565: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=565 ENERGY=energyshift
avg-565: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights565 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-565,weights,weights565 FILE=COLVAR565 STRIDE=2000 FMT=%16.10f

weights570: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=570 ENERGY=energyshift
avg-570: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights570 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-570,weights,weights570 FILE=COLVAR570 STRIDE=2000 FMT=%16.10f

weights575: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=575 ENERGY=energyshift
avg-575: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights575 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-575,weights,weights575 FILE=COLVAR575 STRIDE=2000 FMT=%16.10f

weights580: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=580 ENERGY=energyshift
avg-580: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights580 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-580,weights,weights580 FILE=COLVAR580 STRIDE=2000 FMT=%16.10f

weights585: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=585 ENERGY=energyshift
avg-585: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights585 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-585,weights,weights585 FILE=COLVAR585 STRIDE=2000 FMT=%16.10f

weights590: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=590 ENERGY=energyshift
avg-590: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights590 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-590,weights,weights590 FILE=COLVAR590 STRIDE=2000 FMT=%16.10f

weights595: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=595 ENERGY=energyshift
avg-595: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights595 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-595,weights,weights595 FILE=COLVAR595 STRIDE=2000 FMT=%16.10f

weights600: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=500 REWEIGHT_TEMP=600 ENERGY=energyshift
avg-600: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights600 CLEAR=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-600,weights,weights600 FILE=COLVAR600 STRIDE=2000 FMT=%16.10f

</pre>{% endraw %}
