**Project ID:** [plumID:19.044]({{ '/' | absolute_url }}eggs/19/044/)  
**Source:** MultithermalMultibaricSimulations/MultithermalMultibaric/Analysis/Reweight-1bar/plumed.dat  
**Originally used with PLUMED version:** 2.4-dev  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>

energy: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_a_d.html">READ</a> FILE=../COLVARtrim VALUES=energy2  IGNORE_TIME
vol: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_a_d.html">READ</a> FILE=../COLVARtrim VALUES=vol  IGNORE_TIME
b1: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_a_d.html">READ</a> FILE=../COLVARtrim VALUES=b1.bias  IGNORE_TIME

rvol: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=vol PARAMETERS=7.8 PERIODIC=NO
renergy: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=energy PARAMETERS=-13250 PERIODIC=NO
weights: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__b_i_a_s.html">REWEIGHT_BIAS</a> TEMP=300 ARG=b1.bias

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=* FILE=COLVAR STRIDE=1 FMT=%16.10f
weights260: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=260 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-260: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights260 CLEAR=10000
avg2-260: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights260 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-260,avg2-260 FILE=COLVAR260 STRIDE=10000 FMT=%16.10f

weights262: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=262 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-262: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights262 CLEAR=10000
avg2-262: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights262 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-262,avg2-262 FILE=COLVAR262 STRIDE=10000 FMT=%16.10f

weights264: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=264 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-264: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights264 CLEAR=10000
avg2-264: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights264 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-264,avg2-264 FILE=COLVAR264 STRIDE=10000 FMT=%16.10f

weights266: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=266 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-266: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights266 CLEAR=10000
avg2-266: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights266 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-266,avg2-266 FILE=COLVAR266 STRIDE=10000 FMT=%16.10f

weights268: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=268 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-268: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights268 CLEAR=10000
avg2-268: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights268 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-268,avg2-268 FILE=COLVAR268 STRIDE=10000 FMT=%16.10f

weights270: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=270 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-270: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights270 CLEAR=10000
avg2-270: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights270 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-270,avg2-270 FILE=COLVAR270 STRIDE=10000 FMT=%16.10f

weights272: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=272 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-272: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights272 CLEAR=10000
avg2-272: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights272 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-272,avg2-272 FILE=COLVAR272 STRIDE=10000 FMT=%16.10f

weights274: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=274 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-274: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights274 CLEAR=10000
avg2-274: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights274 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-274,avg2-274 FILE=COLVAR274 STRIDE=10000 FMT=%16.10f

weights276: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=276 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-276: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights276 CLEAR=10000
avg2-276: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights276 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-276,avg2-276 FILE=COLVAR276 STRIDE=10000 FMT=%16.10f

weights278: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=278 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-278: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights278 CLEAR=10000
avg2-278: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights278 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-278,avg2-278 FILE=COLVAR278 STRIDE=10000 FMT=%16.10f

weights280: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=280 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-280: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights280 CLEAR=10000
avg2-280: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights280 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-280,avg2-280 FILE=COLVAR280 STRIDE=10000 FMT=%16.10f

weights282: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=282 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-282: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights282 CLEAR=10000
avg2-282: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights282 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-282,avg2-282 FILE=COLVAR282 STRIDE=10000 FMT=%16.10f

weights284: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=284 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-284: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights284 CLEAR=10000
avg2-284: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights284 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-284,avg2-284 FILE=COLVAR284 STRIDE=10000 FMT=%16.10f

weights286: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=286 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-286: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights286 CLEAR=10000
avg2-286: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights286 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-286,avg2-286 FILE=COLVAR286 STRIDE=10000 FMT=%16.10f

weights288: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=288 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-288: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights288 CLEAR=10000
avg2-288: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights288 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-288,avg2-288 FILE=COLVAR288 STRIDE=10000 FMT=%16.10f

weights290: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=290 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-290: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights290 CLEAR=10000
avg2-290: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights290 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-290,avg2-290 FILE=COLVAR290 STRIDE=10000 FMT=%16.10f

weights292: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=292 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-292: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights292 CLEAR=10000
avg2-292: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights292 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-292,avg2-292 FILE=COLVAR292 STRIDE=10000 FMT=%16.10f

weights294: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=294 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-294: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights294 CLEAR=10000
avg2-294: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights294 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-294,avg2-294 FILE=COLVAR294 STRIDE=10000 FMT=%16.10f

weights296: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=296 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-296: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights296 CLEAR=10000
avg2-296: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights296 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-296,avg2-296 FILE=COLVAR296 STRIDE=10000 FMT=%16.10f

weights298: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=298 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-298: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights298 CLEAR=10000
avg2-298: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights298 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-298,avg2-298 FILE=COLVAR298 STRIDE=10000 FMT=%16.10f

weights300: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=300 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-300: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights300 CLEAR=10000
avg2-300: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights300 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-300,avg2-300 FILE=COLVAR300 STRIDE=10000 FMT=%16.10f

weights302: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=302 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-302: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights302 CLEAR=10000
avg2-302: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights302 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-302,avg2-302 FILE=COLVAR302 STRIDE=10000 FMT=%16.10f

weights304: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=304 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-304: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights304 CLEAR=10000
avg2-304: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights304 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-304,avg2-304 FILE=COLVAR304 STRIDE=10000 FMT=%16.10f

weights306: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=306 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-306: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights306 CLEAR=10000
avg2-306: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights306 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-306,avg2-306 FILE=COLVAR306 STRIDE=10000 FMT=%16.10f

weights308: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=308 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-308: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights308 CLEAR=10000
avg2-308: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights308 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-308,avg2-308 FILE=COLVAR308 STRIDE=10000 FMT=%16.10f

weights310: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=310 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-310: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights310 CLEAR=10000
avg2-310: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights310 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-310,avg2-310 FILE=COLVAR310 STRIDE=10000 FMT=%16.10f

weights312: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=312 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-312: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights312 CLEAR=10000
avg2-312: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights312 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-312,avg2-312 FILE=COLVAR312 STRIDE=10000 FMT=%16.10f

weights314: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=314 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-314: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights314 CLEAR=10000
avg2-314: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights314 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-314,avg2-314 FILE=COLVAR314 STRIDE=10000 FMT=%16.10f

weights316: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=316 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-316: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights316 CLEAR=10000
avg2-316: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights316 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-316,avg2-316 FILE=COLVAR316 STRIDE=10000 FMT=%16.10f

weights318: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=318 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-318: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights318 CLEAR=10000
avg2-318: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights318 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-318,avg2-318 FILE=COLVAR318 STRIDE=10000 FMT=%16.10f

weights320: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=320 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-320: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights320 CLEAR=10000
avg2-320: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights320 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-320,avg2-320 FILE=COLVAR320 STRIDE=10000 FMT=%16.10f

weights322: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=322 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-322: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights322 CLEAR=10000
avg2-322: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights322 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-322,avg2-322 FILE=COLVAR322 STRIDE=10000 FMT=%16.10f

weights324: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=324 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-324: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights324 CLEAR=10000
avg2-324: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights324 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-324,avg2-324 FILE=COLVAR324 STRIDE=10000 FMT=%16.10f

weights326: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=326 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-326: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights326 CLEAR=10000
avg2-326: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights326 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-326,avg2-326 FILE=COLVAR326 STRIDE=10000 FMT=%16.10f

weights328: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=328 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-328: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights328 CLEAR=10000
avg2-328: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights328 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-328,avg2-328 FILE=COLVAR328 STRIDE=10000 FMT=%16.10f

weights330: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=330 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-330: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights330 CLEAR=10000
avg2-330: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights330 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-330,avg2-330 FILE=COLVAR330 STRIDE=10000 FMT=%16.10f

weights332: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=332 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-332: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights332 CLEAR=10000
avg2-332: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights332 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-332,avg2-332 FILE=COLVAR332 STRIDE=10000 FMT=%16.10f

weights334: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=334 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-334: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights334 CLEAR=10000
avg2-334: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights334 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-334,avg2-334 FILE=COLVAR334 STRIDE=10000 FMT=%16.10f

weights336: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=336 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-336: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights336 CLEAR=10000
avg2-336: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights336 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-336,avg2-336 FILE=COLVAR336 STRIDE=10000 FMT=%16.10f

weights338: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=338 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-338: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights338 CLEAR=10000
avg2-338: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights338 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-338,avg2-338 FILE=COLVAR338 STRIDE=10000 FMT=%16.10f

weights340: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=340 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-340: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights340 CLEAR=10000
avg2-340: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights340 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-340,avg2-340 FILE=COLVAR340 STRIDE=10000 FMT=%16.10f

weights342: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=342 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-342: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights342 CLEAR=10000
avg2-342: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights342 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-342,avg2-342 FILE=COLVAR342 STRIDE=10000 FMT=%16.10f

weights344: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=344 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-344: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights344 CLEAR=10000
avg2-344: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights344 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-344,avg2-344 FILE=COLVAR344 STRIDE=10000 FMT=%16.10f

weights346: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=346 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-346: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights346 CLEAR=10000
avg2-346: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights346 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-346,avg2-346 FILE=COLVAR346 STRIDE=10000 FMT=%16.10f

weights348: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=348 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-348: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights348 CLEAR=10000
avg2-348: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights348 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-348,avg2-348 FILE=COLVAR348 STRIDE=10000 FMT=%16.10f

weights350: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=350 REWEIGHT_PRESSURE=0.06022140857 ENERGY=renergy VOLUME=rvol
avg-350: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights350 CLEAR=10000
avg2-350: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights350 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-350,avg2-350 FILE=COLVAR350 STRIDE=10000 FMT=%16.10f

</pre>{% endraw %}
