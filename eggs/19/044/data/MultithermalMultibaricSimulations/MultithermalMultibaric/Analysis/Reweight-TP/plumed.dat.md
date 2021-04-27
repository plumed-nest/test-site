**Project ID:** [plumID:19.044]({{ '/' | absolute_url }}eggs/19/044/)  
**Source:** MultithermalMultibaricSimulations/MultithermalMultibaric/Analysis/Reweight-TP/plumed.dat  
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

weights260-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=260 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-260-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights260-0 CLEAR=10000
avg2-260-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights260-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-260-0,avg2-260-0 FILE=COLVAR260-0 STRIDE=10000 FMT=%16.10f

weights260-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=260 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-260-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights260-5 CLEAR=10000
avg2-260-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights260-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-260-5,avg2-260-5 FILE=COLVAR260-5 STRIDE=10000 FMT=%16.10f

weights260-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=260 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-260-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights260-10 CLEAR=10000
avg2-260-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights260-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-260-10,avg2-260-10 FILE=COLVAR260-10 STRIDE=10000 FMT=%16.10f

weights260-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=260 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-260-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights260-15 CLEAR=10000
avg2-260-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights260-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-260-15,avg2-260-15 FILE=COLVAR260-15 STRIDE=10000 FMT=%16.10f

weights260-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=260 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-260-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights260-20 CLEAR=10000
avg2-260-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights260-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-260-20,avg2-260-20 FILE=COLVAR260-20 STRIDE=10000 FMT=%16.10f

weights260-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=260 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-260-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights260-25 CLEAR=10000
avg2-260-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights260-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-260-25,avg2-260-25 FILE=COLVAR260-25 STRIDE=10000 FMT=%16.10f

weights260-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=260 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-260-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights260-30 CLEAR=10000
avg2-260-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights260-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-260-30,avg2-260-30 FILE=COLVAR260-30 STRIDE=10000 FMT=%16.10f

weights260-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=260 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-260-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights260-35 CLEAR=10000
avg2-260-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights260-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-260-35,avg2-260-35 FILE=COLVAR260-35 STRIDE=10000 FMT=%16.10f

weights260-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=260 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-260-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights260-40 CLEAR=10000
avg2-260-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights260-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-260-40,avg2-260-40 FILE=COLVAR260-40 STRIDE=10000 FMT=%16.10f

weights260-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=260 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-260-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights260-45 CLEAR=10000
avg2-260-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights260-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-260-45,avg2-260-45 FILE=COLVAR260-45 STRIDE=10000 FMT=%16.10f

weights260-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=260 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-260-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights260-50 CLEAR=10000
avg2-260-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights260-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-260-50,avg2-260-50 FILE=COLVAR260-50 STRIDE=10000 FMT=%16.10f

weights260-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=260 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-260-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights260-55 CLEAR=10000
avg2-260-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights260-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-260-55,avg2-260-55 FILE=COLVAR260-55 STRIDE=10000 FMT=%16.10f

weights260-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=260 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-260-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights260-60 CLEAR=10000
avg2-260-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights260-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-260-60,avg2-260-60 FILE=COLVAR260-60 STRIDE=10000 FMT=%16.10f

weights260-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=260 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-260-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights260-65 CLEAR=10000
avg2-260-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights260-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-260-65,avg2-260-65 FILE=COLVAR260-65 STRIDE=10000 FMT=%16.10f

weights260-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=260 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-260-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights260-70 CLEAR=10000
avg2-260-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights260-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-260-70,avg2-260-70 FILE=COLVAR260-70 STRIDE=10000 FMT=%16.10f

weights260-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=260 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-260-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights260-75 CLEAR=10000
avg2-260-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights260-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-260-75,avg2-260-75 FILE=COLVAR260-75 STRIDE=10000 FMT=%16.10f

weights260-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=260 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-260-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights260-80 CLEAR=10000
avg2-260-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights260-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-260-80,avg2-260-80 FILE=COLVAR260-80 STRIDE=10000 FMT=%16.10f

weights260-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=260 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-260-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights260-85 CLEAR=10000
avg2-260-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights260-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-260-85,avg2-260-85 FILE=COLVAR260-85 STRIDE=10000 FMT=%16.10f

weights260-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=260 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-260-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights260-90 CLEAR=10000
avg2-260-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights260-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-260-90,avg2-260-90 FILE=COLVAR260-90 STRIDE=10000 FMT=%16.10f

weights260-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=260 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-260-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights260-95 CLEAR=10000
avg2-260-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights260-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-260-95,avg2-260-95 FILE=COLVAR260-95 STRIDE=10000 FMT=%16.10f

weights260-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=260 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-260-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights260-100 CLEAR=10000
avg2-260-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights260-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-260-100,avg2-260-100 FILE=COLVAR260-100 STRIDE=10000 FMT=%16.10f

weights262-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=262 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-262-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights262-0 CLEAR=10000
avg2-262-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights262-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-262-0,avg2-262-0 FILE=COLVAR262-0 STRIDE=10000 FMT=%16.10f

weights262-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=262 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-262-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights262-5 CLEAR=10000
avg2-262-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights262-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-262-5,avg2-262-5 FILE=COLVAR262-5 STRIDE=10000 FMT=%16.10f

weights262-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=262 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-262-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights262-10 CLEAR=10000
avg2-262-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights262-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-262-10,avg2-262-10 FILE=COLVAR262-10 STRIDE=10000 FMT=%16.10f

weights262-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=262 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-262-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights262-15 CLEAR=10000
avg2-262-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights262-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-262-15,avg2-262-15 FILE=COLVAR262-15 STRIDE=10000 FMT=%16.10f

weights262-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=262 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-262-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights262-20 CLEAR=10000
avg2-262-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights262-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-262-20,avg2-262-20 FILE=COLVAR262-20 STRIDE=10000 FMT=%16.10f

weights262-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=262 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-262-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights262-25 CLEAR=10000
avg2-262-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights262-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-262-25,avg2-262-25 FILE=COLVAR262-25 STRIDE=10000 FMT=%16.10f

weights262-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=262 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-262-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights262-30 CLEAR=10000
avg2-262-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights262-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-262-30,avg2-262-30 FILE=COLVAR262-30 STRIDE=10000 FMT=%16.10f

weights262-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=262 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-262-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights262-35 CLEAR=10000
avg2-262-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights262-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-262-35,avg2-262-35 FILE=COLVAR262-35 STRIDE=10000 FMT=%16.10f

weights262-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=262 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-262-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights262-40 CLEAR=10000
avg2-262-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights262-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-262-40,avg2-262-40 FILE=COLVAR262-40 STRIDE=10000 FMT=%16.10f

weights262-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=262 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-262-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights262-45 CLEAR=10000
avg2-262-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights262-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-262-45,avg2-262-45 FILE=COLVAR262-45 STRIDE=10000 FMT=%16.10f

weights262-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=262 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-262-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights262-50 CLEAR=10000
avg2-262-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights262-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-262-50,avg2-262-50 FILE=COLVAR262-50 STRIDE=10000 FMT=%16.10f

weights262-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=262 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-262-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights262-55 CLEAR=10000
avg2-262-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights262-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-262-55,avg2-262-55 FILE=COLVAR262-55 STRIDE=10000 FMT=%16.10f

weights262-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=262 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-262-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights262-60 CLEAR=10000
avg2-262-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights262-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-262-60,avg2-262-60 FILE=COLVAR262-60 STRIDE=10000 FMT=%16.10f

weights262-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=262 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-262-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights262-65 CLEAR=10000
avg2-262-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights262-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-262-65,avg2-262-65 FILE=COLVAR262-65 STRIDE=10000 FMT=%16.10f

weights262-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=262 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-262-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights262-70 CLEAR=10000
avg2-262-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights262-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-262-70,avg2-262-70 FILE=COLVAR262-70 STRIDE=10000 FMT=%16.10f

weights262-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=262 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-262-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights262-75 CLEAR=10000
avg2-262-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights262-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-262-75,avg2-262-75 FILE=COLVAR262-75 STRIDE=10000 FMT=%16.10f

weights262-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=262 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-262-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights262-80 CLEAR=10000
avg2-262-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights262-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-262-80,avg2-262-80 FILE=COLVAR262-80 STRIDE=10000 FMT=%16.10f

weights262-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=262 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-262-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights262-85 CLEAR=10000
avg2-262-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights262-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-262-85,avg2-262-85 FILE=COLVAR262-85 STRIDE=10000 FMT=%16.10f

weights262-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=262 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-262-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights262-90 CLEAR=10000
avg2-262-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights262-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-262-90,avg2-262-90 FILE=COLVAR262-90 STRIDE=10000 FMT=%16.10f

weights262-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=262 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-262-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights262-95 CLEAR=10000
avg2-262-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights262-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-262-95,avg2-262-95 FILE=COLVAR262-95 STRIDE=10000 FMT=%16.10f

weights262-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=262 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-262-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights262-100 CLEAR=10000
avg2-262-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights262-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-262-100,avg2-262-100 FILE=COLVAR262-100 STRIDE=10000 FMT=%16.10f

weights264-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=264 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-264-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights264-0 CLEAR=10000
avg2-264-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights264-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-264-0,avg2-264-0 FILE=COLVAR264-0 STRIDE=10000 FMT=%16.10f

weights264-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=264 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-264-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights264-5 CLEAR=10000
avg2-264-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights264-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-264-5,avg2-264-5 FILE=COLVAR264-5 STRIDE=10000 FMT=%16.10f

weights264-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=264 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-264-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights264-10 CLEAR=10000
avg2-264-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights264-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-264-10,avg2-264-10 FILE=COLVAR264-10 STRIDE=10000 FMT=%16.10f

weights264-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=264 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-264-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights264-15 CLEAR=10000
avg2-264-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights264-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-264-15,avg2-264-15 FILE=COLVAR264-15 STRIDE=10000 FMT=%16.10f

weights264-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=264 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-264-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights264-20 CLEAR=10000
avg2-264-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights264-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-264-20,avg2-264-20 FILE=COLVAR264-20 STRIDE=10000 FMT=%16.10f

weights264-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=264 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-264-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights264-25 CLEAR=10000
avg2-264-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights264-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-264-25,avg2-264-25 FILE=COLVAR264-25 STRIDE=10000 FMT=%16.10f

weights264-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=264 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-264-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights264-30 CLEAR=10000
avg2-264-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights264-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-264-30,avg2-264-30 FILE=COLVAR264-30 STRIDE=10000 FMT=%16.10f

weights264-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=264 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-264-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights264-35 CLEAR=10000
avg2-264-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights264-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-264-35,avg2-264-35 FILE=COLVAR264-35 STRIDE=10000 FMT=%16.10f

weights264-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=264 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-264-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights264-40 CLEAR=10000
avg2-264-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights264-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-264-40,avg2-264-40 FILE=COLVAR264-40 STRIDE=10000 FMT=%16.10f

weights264-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=264 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-264-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights264-45 CLEAR=10000
avg2-264-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights264-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-264-45,avg2-264-45 FILE=COLVAR264-45 STRIDE=10000 FMT=%16.10f

weights264-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=264 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-264-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights264-50 CLEAR=10000
avg2-264-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights264-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-264-50,avg2-264-50 FILE=COLVAR264-50 STRIDE=10000 FMT=%16.10f

weights264-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=264 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-264-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights264-55 CLEAR=10000
avg2-264-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights264-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-264-55,avg2-264-55 FILE=COLVAR264-55 STRIDE=10000 FMT=%16.10f

weights264-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=264 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-264-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights264-60 CLEAR=10000
avg2-264-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights264-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-264-60,avg2-264-60 FILE=COLVAR264-60 STRIDE=10000 FMT=%16.10f

weights264-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=264 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-264-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights264-65 CLEAR=10000
avg2-264-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights264-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-264-65,avg2-264-65 FILE=COLVAR264-65 STRIDE=10000 FMT=%16.10f

weights264-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=264 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-264-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights264-70 CLEAR=10000
avg2-264-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights264-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-264-70,avg2-264-70 FILE=COLVAR264-70 STRIDE=10000 FMT=%16.10f

weights264-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=264 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-264-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights264-75 CLEAR=10000
avg2-264-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights264-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-264-75,avg2-264-75 FILE=COLVAR264-75 STRIDE=10000 FMT=%16.10f

weights264-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=264 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-264-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights264-80 CLEAR=10000
avg2-264-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights264-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-264-80,avg2-264-80 FILE=COLVAR264-80 STRIDE=10000 FMT=%16.10f

weights264-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=264 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-264-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights264-85 CLEAR=10000
avg2-264-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights264-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-264-85,avg2-264-85 FILE=COLVAR264-85 STRIDE=10000 FMT=%16.10f

weights264-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=264 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-264-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights264-90 CLEAR=10000
avg2-264-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights264-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-264-90,avg2-264-90 FILE=COLVAR264-90 STRIDE=10000 FMT=%16.10f

weights264-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=264 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-264-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights264-95 CLEAR=10000
avg2-264-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights264-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-264-95,avg2-264-95 FILE=COLVAR264-95 STRIDE=10000 FMT=%16.10f

weights264-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=264 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-264-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights264-100 CLEAR=10000
avg2-264-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights264-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-264-100,avg2-264-100 FILE=COLVAR264-100 STRIDE=10000 FMT=%16.10f

weights266-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=266 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-266-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights266-0 CLEAR=10000
avg2-266-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights266-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-266-0,avg2-266-0 FILE=COLVAR266-0 STRIDE=10000 FMT=%16.10f

weights266-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=266 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-266-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights266-5 CLEAR=10000
avg2-266-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights266-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-266-5,avg2-266-5 FILE=COLVAR266-5 STRIDE=10000 FMT=%16.10f

weights266-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=266 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-266-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights266-10 CLEAR=10000
avg2-266-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights266-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-266-10,avg2-266-10 FILE=COLVAR266-10 STRIDE=10000 FMT=%16.10f

weights266-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=266 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-266-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights266-15 CLEAR=10000
avg2-266-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights266-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-266-15,avg2-266-15 FILE=COLVAR266-15 STRIDE=10000 FMT=%16.10f

weights266-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=266 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-266-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights266-20 CLEAR=10000
avg2-266-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights266-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-266-20,avg2-266-20 FILE=COLVAR266-20 STRIDE=10000 FMT=%16.10f

weights266-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=266 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-266-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights266-25 CLEAR=10000
avg2-266-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights266-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-266-25,avg2-266-25 FILE=COLVAR266-25 STRIDE=10000 FMT=%16.10f

weights266-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=266 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-266-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights266-30 CLEAR=10000
avg2-266-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights266-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-266-30,avg2-266-30 FILE=COLVAR266-30 STRIDE=10000 FMT=%16.10f

weights266-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=266 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-266-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights266-35 CLEAR=10000
avg2-266-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights266-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-266-35,avg2-266-35 FILE=COLVAR266-35 STRIDE=10000 FMT=%16.10f

weights266-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=266 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-266-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights266-40 CLEAR=10000
avg2-266-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights266-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-266-40,avg2-266-40 FILE=COLVAR266-40 STRIDE=10000 FMT=%16.10f

weights266-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=266 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-266-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights266-45 CLEAR=10000
avg2-266-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights266-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-266-45,avg2-266-45 FILE=COLVAR266-45 STRIDE=10000 FMT=%16.10f

weights266-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=266 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-266-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights266-50 CLEAR=10000
avg2-266-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights266-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-266-50,avg2-266-50 FILE=COLVAR266-50 STRIDE=10000 FMT=%16.10f

weights266-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=266 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-266-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights266-55 CLEAR=10000
avg2-266-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights266-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-266-55,avg2-266-55 FILE=COLVAR266-55 STRIDE=10000 FMT=%16.10f

weights266-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=266 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-266-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights266-60 CLEAR=10000
avg2-266-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights266-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-266-60,avg2-266-60 FILE=COLVAR266-60 STRIDE=10000 FMT=%16.10f

weights266-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=266 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-266-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights266-65 CLEAR=10000
avg2-266-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights266-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-266-65,avg2-266-65 FILE=COLVAR266-65 STRIDE=10000 FMT=%16.10f

weights266-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=266 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-266-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights266-70 CLEAR=10000
avg2-266-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights266-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-266-70,avg2-266-70 FILE=COLVAR266-70 STRIDE=10000 FMT=%16.10f

weights266-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=266 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-266-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights266-75 CLEAR=10000
avg2-266-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights266-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-266-75,avg2-266-75 FILE=COLVAR266-75 STRIDE=10000 FMT=%16.10f

weights266-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=266 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-266-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights266-80 CLEAR=10000
avg2-266-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights266-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-266-80,avg2-266-80 FILE=COLVAR266-80 STRIDE=10000 FMT=%16.10f

weights266-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=266 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-266-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights266-85 CLEAR=10000
avg2-266-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights266-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-266-85,avg2-266-85 FILE=COLVAR266-85 STRIDE=10000 FMT=%16.10f

weights266-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=266 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-266-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights266-90 CLEAR=10000
avg2-266-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights266-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-266-90,avg2-266-90 FILE=COLVAR266-90 STRIDE=10000 FMT=%16.10f

weights266-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=266 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-266-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights266-95 CLEAR=10000
avg2-266-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights266-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-266-95,avg2-266-95 FILE=COLVAR266-95 STRIDE=10000 FMT=%16.10f

weights266-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=266 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-266-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights266-100 CLEAR=10000
avg2-266-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights266-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-266-100,avg2-266-100 FILE=COLVAR266-100 STRIDE=10000 FMT=%16.10f

weights268-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=268 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-268-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights268-0 CLEAR=10000
avg2-268-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights268-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-268-0,avg2-268-0 FILE=COLVAR268-0 STRIDE=10000 FMT=%16.10f

weights268-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=268 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-268-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights268-5 CLEAR=10000
avg2-268-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights268-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-268-5,avg2-268-5 FILE=COLVAR268-5 STRIDE=10000 FMT=%16.10f

weights268-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=268 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-268-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights268-10 CLEAR=10000
avg2-268-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights268-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-268-10,avg2-268-10 FILE=COLVAR268-10 STRIDE=10000 FMT=%16.10f

weights268-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=268 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-268-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights268-15 CLEAR=10000
avg2-268-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights268-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-268-15,avg2-268-15 FILE=COLVAR268-15 STRIDE=10000 FMT=%16.10f

weights268-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=268 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-268-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights268-20 CLEAR=10000
avg2-268-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights268-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-268-20,avg2-268-20 FILE=COLVAR268-20 STRIDE=10000 FMT=%16.10f

weights268-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=268 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-268-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights268-25 CLEAR=10000
avg2-268-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights268-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-268-25,avg2-268-25 FILE=COLVAR268-25 STRIDE=10000 FMT=%16.10f

weights268-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=268 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-268-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights268-30 CLEAR=10000
avg2-268-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights268-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-268-30,avg2-268-30 FILE=COLVAR268-30 STRIDE=10000 FMT=%16.10f

weights268-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=268 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-268-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights268-35 CLEAR=10000
avg2-268-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights268-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-268-35,avg2-268-35 FILE=COLVAR268-35 STRIDE=10000 FMT=%16.10f

weights268-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=268 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-268-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights268-40 CLEAR=10000
avg2-268-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights268-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-268-40,avg2-268-40 FILE=COLVAR268-40 STRIDE=10000 FMT=%16.10f

weights268-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=268 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-268-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights268-45 CLEAR=10000
avg2-268-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights268-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-268-45,avg2-268-45 FILE=COLVAR268-45 STRIDE=10000 FMT=%16.10f

weights268-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=268 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-268-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights268-50 CLEAR=10000
avg2-268-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights268-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-268-50,avg2-268-50 FILE=COLVAR268-50 STRIDE=10000 FMT=%16.10f

weights268-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=268 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-268-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights268-55 CLEAR=10000
avg2-268-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights268-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-268-55,avg2-268-55 FILE=COLVAR268-55 STRIDE=10000 FMT=%16.10f

weights268-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=268 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-268-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights268-60 CLEAR=10000
avg2-268-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights268-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-268-60,avg2-268-60 FILE=COLVAR268-60 STRIDE=10000 FMT=%16.10f

weights268-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=268 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-268-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights268-65 CLEAR=10000
avg2-268-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights268-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-268-65,avg2-268-65 FILE=COLVAR268-65 STRIDE=10000 FMT=%16.10f

weights268-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=268 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-268-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights268-70 CLEAR=10000
avg2-268-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights268-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-268-70,avg2-268-70 FILE=COLVAR268-70 STRIDE=10000 FMT=%16.10f

weights268-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=268 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-268-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights268-75 CLEAR=10000
avg2-268-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights268-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-268-75,avg2-268-75 FILE=COLVAR268-75 STRIDE=10000 FMT=%16.10f

weights268-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=268 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-268-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights268-80 CLEAR=10000
avg2-268-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights268-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-268-80,avg2-268-80 FILE=COLVAR268-80 STRIDE=10000 FMT=%16.10f

weights268-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=268 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-268-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights268-85 CLEAR=10000
avg2-268-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights268-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-268-85,avg2-268-85 FILE=COLVAR268-85 STRIDE=10000 FMT=%16.10f

weights268-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=268 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-268-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights268-90 CLEAR=10000
avg2-268-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights268-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-268-90,avg2-268-90 FILE=COLVAR268-90 STRIDE=10000 FMT=%16.10f

weights268-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=268 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-268-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights268-95 CLEAR=10000
avg2-268-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights268-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-268-95,avg2-268-95 FILE=COLVAR268-95 STRIDE=10000 FMT=%16.10f

weights268-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=268 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-268-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights268-100 CLEAR=10000
avg2-268-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights268-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-268-100,avg2-268-100 FILE=COLVAR268-100 STRIDE=10000 FMT=%16.10f

weights270-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=270 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-270-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights270-0 CLEAR=10000
avg2-270-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights270-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-270-0,avg2-270-0 FILE=COLVAR270-0 STRIDE=10000 FMT=%16.10f

weights270-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=270 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-270-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights270-5 CLEAR=10000
avg2-270-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights270-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-270-5,avg2-270-5 FILE=COLVAR270-5 STRIDE=10000 FMT=%16.10f

weights270-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=270 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-270-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights270-10 CLEAR=10000
avg2-270-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights270-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-270-10,avg2-270-10 FILE=COLVAR270-10 STRIDE=10000 FMT=%16.10f

weights270-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=270 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-270-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights270-15 CLEAR=10000
avg2-270-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights270-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-270-15,avg2-270-15 FILE=COLVAR270-15 STRIDE=10000 FMT=%16.10f

weights270-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=270 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-270-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights270-20 CLEAR=10000
avg2-270-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights270-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-270-20,avg2-270-20 FILE=COLVAR270-20 STRIDE=10000 FMT=%16.10f

weights270-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=270 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-270-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights270-25 CLEAR=10000
avg2-270-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights270-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-270-25,avg2-270-25 FILE=COLVAR270-25 STRIDE=10000 FMT=%16.10f

weights270-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=270 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-270-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights270-30 CLEAR=10000
avg2-270-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights270-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-270-30,avg2-270-30 FILE=COLVAR270-30 STRIDE=10000 FMT=%16.10f

weights270-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=270 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-270-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights270-35 CLEAR=10000
avg2-270-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights270-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-270-35,avg2-270-35 FILE=COLVAR270-35 STRIDE=10000 FMT=%16.10f

weights270-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=270 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-270-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights270-40 CLEAR=10000
avg2-270-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights270-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-270-40,avg2-270-40 FILE=COLVAR270-40 STRIDE=10000 FMT=%16.10f

weights270-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=270 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-270-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights270-45 CLEAR=10000
avg2-270-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights270-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-270-45,avg2-270-45 FILE=COLVAR270-45 STRIDE=10000 FMT=%16.10f

weights270-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=270 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-270-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights270-50 CLEAR=10000
avg2-270-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights270-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-270-50,avg2-270-50 FILE=COLVAR270-50 STRIDE=10000 FMT=%16.10f

weights270-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=270 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-270-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights270-55 CLEAR=10000
avg2-270-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights270-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-270-55,avg2-270-55 FILE=COLVAR270-55 STRIDE=10000 FMT=%16.10f

weights270-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=270 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-270-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights270-60 CLEAR=10000
avg2-270-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights270-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-270-60,avg2-270-60 FILE=COLVAR270-60 STRIDE=10000 FMT=%16.10f

weights270-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=270 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-270-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights270-65 CLEAR=10000
avg2-270-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights270-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-270-65,avg2-270-65 FILE=COLVAR270-65 STRIDE=10000 FMT=%16.10f

weights270-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=270 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-270-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights270-70 CLEAR=10000
avg2-270-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights270-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-270-70,avg2-270-70 FILE=COLVAR270-70 STRIDE=10000 FMT=%16.10f

weights270-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=270 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-270-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights270-75 CLEAR=10000
avg2-270-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights270-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-270-75,avg2-270-75 FILE=COLVAR270-75 STRIDE=10000 FMT=%16.10f

weights270-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=270 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-270-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights270-80 CLEAR=10000
avg2-270-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights270-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-270-80,avg2-270-80 FILE=COLVAR270-80 STRIDE=10000 FMT=%16.10f

weights270-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=270 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-270-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights270-85 CLEAR=10000
avg2-270-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights270-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-270-85,avg2-270-85 FILE=COLVAR270-85 STRIDE=10000 FMT=%16.10f

weights270-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=270 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-270-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights270-90 CLEAR=10000
avg2-270-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights270-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-270-90,avg2-270-90 FILE=COLVAR270-90 STRIDE=10000 FMT=%16.10f

weights270-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=270 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-270-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights270-95 CLEAR=10000
avg2-270-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights270-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-270-95,avg2-270-95 FILE=COLVAR270-95 STRIDE=10000 FMT=%16.10f

weights270-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=270 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-270-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights270-100 CLEAR=10000
avg2-270-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights270-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-270-100,avg2-270-100 FILE=COLVAR270-100 STRIDE=10000 FMT=%16.10f

weights272-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=272 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-272-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights272-0 CLEAR=10000
avg2-272-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights272-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-272-0,avg2-272-0 FILE=COLVAR272-0 STRIDE=10000 FMT=%16.10f

weights272-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=272 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-272-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights272-5 CLEAR=10000
avg2-272-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights272-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-272-5,avg2-272-5 FILE=COLVAR272-5 STRIDE=10000 FMT=%16.10f

weights272-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=272 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-272-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights272-10 CLEAR=10000
avg2-272-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights272-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-272-10,avg2-272-10 FILE=COLVAR272-10 STRIDE=10000 FMT=%16.10f

weights272-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=272 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-272-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights272-15 CLEAR=10000
avg2-272-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights272-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-272-15,avg2-272-15 FILE=COLVAR272-15 STRIDE=10000 FMT=%16.10f

weights272-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=272 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-272-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights272-20 CLEAR=10000
avg2-272-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights272-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-272-20,avg2-272-20 FILE=COLVAR272-20 STRIDE=10000 FMT=%16.10f

weights272-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=272 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-272-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights272-25 CLEAR=10000
avg2-272-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights272-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-272-25,avg2-272-25 FILE=COLVAR272-25 STRIDE=10000 FMT=%16.10f

weights272-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=272 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-272-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights272-30 CLEAR=10000
avg2-272-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights272-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-272-30,avg2-272-30 FILE=COLVAR272-30 STRIDE=10000 FMT=%16.10f

weights272-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=272 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-272-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights272-35 CLEAR=10000
avg2-272-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights272-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-272-35,avg2-272-35 FILE=COLVAR272-35 STRIDE=10000 FMT=%16.10f

weights272-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=272 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-272-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights272-40 CLEAR=10000
avg2-272-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights272-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-272-40,avg2-272-40 FILE=COLVAR272-40 STRIDE=10000 FMT=%16.10f

weights272-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=272 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-272-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights272-45 CLEAR=10000
avg2-272-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights272-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-272-45,avg2-272-45 FILE=COLVAR272-45 STRIDE=10000 FMT=%16.10f

weights272-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=272 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-272-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights272-50 CLEAR=10000
avg2-272-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights272-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-272-50,avg2-272-50 FILE=COLVAR272-50 STRIDE=10000 FMT=%16.10f

weights272-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=272 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-272-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights272-55 CLEAR=10000
avg2-272-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights272-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-272-55,avg2-272-55 FILE=COLVAR272-55 STRIDE=10000 FMT=%16.10f

weights272-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=272 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-272-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights272-60 CLEAR=10000
avg2-272-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights272-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-272-60,avg2-272-60 FILE=COLVAR272-60 STRIDE=10000 FMT=%16.10f

weights272-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=272 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-272-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights272-65 CLEAR=10000
avg2-272-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights272-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-272-65,avg2-272-65 FILE=COLVAR272-65 STRIDE=10000 FMT=%16.10f

weights272-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=272 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-272-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights272-70 CLEAR=10000
avg2-272-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights272-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-272-70,avg2-272-70 FILE=COLVAR272-70 STRIDE=10000 FMT=%16.10f

weights272-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=272 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-272-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights272-75 CLEAR=10000
avg2-272-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights272-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-272-75,avg2-272-75 FILE=COLVAR272-75 STRIDE=10000 FMT=%16.10f

weights272-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=272 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-272-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights272-80 CLEAR=10000
avg2-272-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights272-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-272-80,avg2-272-80 FILE=COLVAR272-80 STRIDE=10000 FMT=%16.10f

weights272-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=272 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-272-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights272-85 CLEAR=10000
avg2-272-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights272-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-272-85,avg2-272-85 FILE=COLVAR272-85 STRIDE=10000 FMT=%16.10f

weights272-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=272 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-272-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights272-90 CLEAR=10000
avg2-272-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights272-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-272-90,avg2-272-90 FILE=COLVAR272-90 STRIDE=10000 FMT=%16.10f

weights272-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=272 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-272-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights272-95 CLEAR=10000
avg2-272-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights272-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-272-95,avg2-272-95 FILE=COLVAR272-95 STRIDE=10000 FMT=%16.10f

weights272-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=272 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-272-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights272-100 CLEAR=10000
avg2-272-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights272-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-272-100,avg2-272-100 FILE=COLVAR272-100 STRIDE=10000 FMT=%16.10f

weights274-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=274 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-274-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights274-0 CLEAR=10000
avg2-274-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights274-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-274-0,avg2-274-0 FILE=COLVAR274-0 STRIDE=10000 FMT=%16.10f

weights274-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=274 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-274-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights274-5 CLEAR=10000
avg2-274-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights274-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-274-5,avg2-274-5 FILE=COLVAR274-5 STRIDE=10000 FMT=%16.10f

weights274-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=274 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-274-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights274-10 CLEAR=10000
avg2-274-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights274-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-274-10,avg2-274-10 FILE=COLVAR274-10 STRIDE=10000 FMT=%16.10f

weights274-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=274 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-274-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights274-15 CLEAR=10000
avg2-274-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights274-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-274-15,avg2-274-15 FILE=COLVAR274-15 STRIDE=10000 FMT=%16.10f

weights274-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=274 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-274-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights274-20 CLEAR=10000
avg2-274-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights274-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-274-20,avg2-274-20 FILE=COLVAR274-20 STRIDE=10000 FMT=%16.10f

weights274-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=274 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-274-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights274-25 CLEAR=10000
avg2-274-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights274-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-274-25,avg2-274-25 FILE=COLVAR274-25 STRIDE=10000 FMT=%16.10f

weights274-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=274 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-274-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights274-30 CLEAR=10000
avg2-274-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights274-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-274-30,avg2-274-30 FILE=COLVAR274-30 STRIDE=10000 FMT=%16.10f

weights274-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=274 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-274-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights274-35 CLEAR=10000
avg2-274-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights274-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-274-35,avg2-274-35 FILE=COLVAR274-35 STRIDE=10000 FMT=%16.10f

weights274-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=274 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-274-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights274-40 CLEAR=10000
avg2-274-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights274-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-274-40,avg2-274-40 FILE=COLVAR274-40 STRIDE=10000 FMT=%16.10f

weights274-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=274 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-274-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights274-45 CLEAR=10000
avg2-274-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights274-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-274-45,avg2-274-45 FILE=COLVAR274-45 STRIDE=10000 FMT=%16.10f

weights274-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=274 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-274-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights274-50 CLEAR=10000
avg2-274-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights274-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-274-50,avg2-274-50 FILE=COLVAR274-50 STRIDE=10000 FMT=%16.10f

weights274-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=274 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-274-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights274-55 CLEAR=10000
avg2-274-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights274-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-274-55,avg2-274-55 FILE=COLVAR274-55 STRIDE=10000 FMT=%16.10f

weights274-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=274 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-274-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights274-60 CLEAR=10000
avg2-274-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights274-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-274-60,avg2-274-60 FILE=COLVAR274-60 STRIDE=10000 FMT=%16.10f

weights274-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=274 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-274-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights274-65 CLEAR=10000
avg2-274-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights274-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-274-65,avg2-274-65 FILE=COLVAR274-65 STRIDE=10000 FMT=%16.10f

weights274-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=274 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-274-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights274-70 CLEAR=10000
avg2-274-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights274-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-274-70,avg2-274-70 FILE=COLVAR274-70 STRIDE=10000 FMT=%16.10f

weights274-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=274 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-274-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights274-75 CLEAR=10000
avg2-274-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights274-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-274-75,avg2-274-75 FILE=COLVAR274-75 STRIDE=10000 FMT=%16.10f

weights274-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=274 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-274-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights274-80 CLEAR=10000
avg2-274-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights274-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-274-80,avg2-274-80 FILE=COLVAR274-80 STRIDE=10000 FMT=%16.10f

weights274-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=274 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-274-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights274-85 CLEAR=10000
avg2-274-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights274-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-274-85,avg2-274-85 FILE=COLVAR274-85 STRIDE=10000 FMT=%16.10f

weights274-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=274 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-274-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights274-90 CLEAR=10000
avg2-274-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights274-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-274-90,avg2-274-90 FILE=COLVAR274-90 STRIDE=10000 FMT=%16.10f

weights274-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=274 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-274-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights274-95 CLEAR=10000
avg2-274-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights274-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-274-95,avg2-274-95 FILE=COLVAR274-95 STRIDE=10000 FMT=%16.10f

weights274-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=274 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-274-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights274-100 CLEAR=10000
avg2-274-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights274-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-274-100,avg2-274-100 FILE=COLVAR274-100 STRIDE=10000 FMT=%16.10f

weights276-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=276 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-276-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights276-0 CLEAR=10000
avg2-276-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights276-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-276-0,avg2-276-0 FILE=COLVAR276-0 STRIDE=10000 FMT=%16.10f

weights276-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=276 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-276-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights276-5 CLEAR=10000
avg2-276-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights276-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-276-5,avg2-276-5 FILE=COLVAR276-5 STRIDE=10000 FMT=%16.10f

weights276-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=276 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-276-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights276-10 CLEAR=10000
avg2-276-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights276-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-276-10,avg2-276-10 FILE=COLVAR276-10 STRIDE=10000 FMT=%16.10f

weights276-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=276 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-276-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights276-15 CLEAR=10000
avg2-276-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights276-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-276-15,avg2-276-15 FILE=COLVAR276-15 STRIDE=10000 FMT=%16.10f

weights276-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=276 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-276-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights276-20 CLEAR=10000
avg2-276-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights276-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-276-20,avg2-276-20 FILE=COLVAR276-20 STRIDE=10000 FMT=%16.10f

weights276-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=276 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-276-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights276-25 CLEAR=10000
avg2-276-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights276-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-276-25,avg2-276-25 FILE=COLVAR276-25 STRIDE=10000 FMT=%16.10f

weights276-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=276 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-276-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights276-30 CLEAR=10000
avg2-276-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights276-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-276-30,avg2-276-30 FILE=COLVAR276-30 STRIDE=10000 FMT=%16.10f

weights276-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=276 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-276-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights276-35 CLEAR=10000
avg2-276-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights276-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-276-35,avg2-276-35 FILE=COLVAR276-35 STRIDE=10000 FMT=%16.10f

weights276-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=276 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-276-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights276-40 CLEAR=10000
avg2-276-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights276-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-276-40,avg2-276-40 FILE=COLVAR276-40 STRIDE=10000 FMT=%16.10f

weights276-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=276 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-276-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights276-45 CLEAR=10000
avg2-276-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights276-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-276-45,avg2-276-45 FILE=COLVAR276-45 STRIDE=10000 FMT=%16.10f

weights276-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=276 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-276-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights276-50 CLEAR=10000
avg2-276-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights276-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-276-50,avg2-276-50 FILE=COLVAR276-50 STRIDE=10000 FMT=%16.10f

weights276-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=276 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-276-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights276-55 CLEAR=10000
avg2-276-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights276-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-276-55,avg2-276-55 FILE=COLVAR276-55 STRIDE=10000 FMT=%16.10f

weights276-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=276 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-276-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights276-60 CLEAR=10000
avg2-276-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights276-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-276-60,avg2-276-60 FILE=COLVAR276-60 STRIDE=10000 FMT=%16.10f

weights276-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=276 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-276-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights276-65 CLEAR=10000
avg2-276-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights276-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-276-65,avg2-276-65 FILE=COLVAR276-65 STRIDE=10000 FMT=%16.10f

weights276-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=276 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-276-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights276-70 CLEAR=10000
avg2-276-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights276-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-276-70,avg2-276-70 FILE=COLVAR276-70 STRIDE=10000 FMT=%16.10f

weights276-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=276 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-276-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights276-75 CLEAR=10000
avg2-276-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights276-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-276-75,avg2-276-75 FILE=COLVAR276-75 STRIDE=10000 FMT=%16.10f

weights276-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=276 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-276-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights276-80 CLEAR=10000
avg2-276-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights276-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-276-80,avg2-276-80 FILE=COLVAR276-80 STRIDE=10000 FMT=%16.10f

weights276-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=276 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-276-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights276-85 CLEAR=10000
avg2-276-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights276-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-276-85,avg2-276-85 FILE=COLVAR276-85 STRIDE=10000 FMT=%16.10f

weights276-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=276 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-276-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights276-90 CLEAR=10000
avg2-276-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights276-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-276-90,avg2-276-90 FILE=COLVAR276-90 STRIDE=10000 FMT=%16.10f

weights276-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=276 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-276-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights276-95 CLEAR=10000
avg2-276-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights276-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-276-95,avg2-276-95 FILE=COLVAR276-95 STRIDE=10000 FMT=%16.10f

weights276-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=276 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-276-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights276-100 CLEAR=10000
avg2-276-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights276-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-276-100,avg2-276-100 FILE=COLVAR276-100 STRIDE=10000 FMT=%16.10f

weights278-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=278 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-278-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights278-0 CLEAR=10000
avg2-278-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights278-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-278-0,avg2-278-0 FILE=COLVAR278-0 STRIDE=10000 FMT=%16.10f

weights278-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=278 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-278-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights278-5 CLEAR=10000
avg2-278-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights278-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-278-5,avg2-278-5 FILE=COLVAR278-5 STRIDE=10000 FMT=%16.10f

weights278-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=278 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-278-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights278-10 CLEAR=10000
avg2-278-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights278-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-278-10,avg2-278-10 FILE=COLVAR278-10 STRIDE=10000 FMT=%16.10f

weights278-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=278 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-278-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights278-15 CLEAR=10000
avg2-278-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights278-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-278-15,avg2-278-15 FILE=COLVAR278-15 STRIDE=10000 FMT=%16.10f

weights278-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=278 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-278-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights278-20 CLEAR=10000
avg2-278-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights278-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-278-20,avg2-278-20 FILE=COLVAR278-20 STRIDE=10000 FMT=%16.10f

weights278-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=278 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-278-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights278-25 CLEAR=10000
avg2-278-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights278-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-278-25,avg2-278-25 FILE=COLVAR278-25 STRIDE=10000 FMT=%16.10f

weights278-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=278 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-278-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights278-30 CLEAR=10000
avg2-278-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights278-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-278-30,avg2-278-30 FILE=COLVAR278-30 STRIDE=10000 FMT=%16.10f

weights278-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=278 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-278-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights278-35 CLEAR=10000
avg2-278-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights278-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-278-35,avg2-278-35 FILE=COLVAR278-35 STRIDE=10000 FMT=%16.10f

weights278-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=278 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-278-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights278-40 CLEAR=10000
avg2-278-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights278-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-278-40,avg2-278-40 FILE=COLVAR278-40 STRIDE=10000 FMT=%16.10f

weights278-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=278 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-278-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights278-45 CLEAR=10000
avg2-278-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights278-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-278-45,avg2-278-45 FILE=COLVAR278-45 STRIDE=10000 FMT=%16.10f

weights278-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=278 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-278-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights278-50 CLEAR=10000
avg2-278-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights278-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-278-50,avg2-278-50 FILE=COLVAR278-50 STRIDE=10000 FMT=%16.10f

weights278-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=278 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-278-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights278-55 CLEAR=10000
avg2-278-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights278-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-278-55,avg2-278-55 FILE=COLVAR278-55 STRIDE=10000 FMT=%16.10f

weights278-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=278 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-278-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights278-60 CLEAR=10000
avg2-278-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights278-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-278-60,avg2-278-60 FILE=COLVAR278-60 STRIDE=10000 FMT=%16.10f

weights278-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=278 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-278-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights278-65 CLEAR=10000
avg2-278-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights278-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-278-65,avg2-278-65 FILE=COLVAR278-65 STRIDE=10000 FMT=%16.10f

weights278-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=278 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-278-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights278-70 CLEAR=10000
avg2-278-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights278-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-278-70,avg2-278-70 FILE=COLVAR278-70 STRIDE=10000 FMT=%16.10f

weights278-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=278 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-278-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights278-75 CLEAR=10000
avg2-278-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights278-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-278-75,avg2-278-75 FILE=COLVAR278-75 STRIDE=10000 FMT=%16.10f

weights278-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=278 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-278-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights278-80 CLEAR=10000
avg2-278-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights278-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-278-80,avg2-278-80 FILE=COLVAR278-80 STRIDE=10000 FMT=%16.10f

weights278-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=278 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-278-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights278-85 CLEAR=10000
avg2-278-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights278-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-278-85,avg2-278-85 FILE=COLVAR278-85 STRIDE=10000 FMT=%16.10f

weights278-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=278 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-278-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights278-90 CLEAR=10000
avg2-278-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights278-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-278-90,avg2-278-90 FILE=COLVAR278-90 STRIDE=10000 FMT=%16.10f

weights278-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=278 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-278-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights278-95 CLEAR=10000
avg2-278-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights278-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-278-95,avg2-278-95 FILE=COLVAR278-95 STRIDE=10000 FMT=%16.10f

weights278-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=278 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-278-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights278-100 CLEAR=10000
avg2-278-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights278-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-278-100,avg2-278-100 FILE=COLVAR278-100 STRIDE=10000 FMT=%16.10f

weights280-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=280 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-280-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights280-0 CLEAR=10000
avg2-280-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights280-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-280-0,avg2-280-0 FILE=COLVAR280-0 STRIDE=10000 FMT=%16.10f

weights280-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=280 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-280-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights280-5 CLEAR=10000
avg2-280-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights280-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-280-5,avg2-280-5 FILE=COLVAR280-5 STRIDE=10000 FMT=%16.10f

weights280-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=280 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-280-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights280-10 CLEAR=10000
avg2-280-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights280-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-280-10,avg2-280-10 FILE=COLVAR280-10 STRIDE=10000 FMT=%16.10f

weights280-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=280 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-280-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights280-15 CLEAR=10000
avg2-280-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights280-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-280-15,avg2-280-15 FILE=COLVAR280-15 STRIDE=10000 FMT=%16.10f

weights280-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=280 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-280-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights280-20 CLEAR=10000
avg2-280-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights280-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-280-20,avg2-280-20 FILE=COLVAR280-20 STRIDE=10000 FMT=%16.10f

weights280-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=280 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-280-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights280-25 CLEAR=10000
avg2-280-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights280-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-280-25,avg2-280-25 FILE=COLVAR280-25 STRIDE=10000 FMT=%16.10f

weights280-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=280 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-280-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights280-30 CLEAR=10000
avg2-280-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights280-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-280-30,avg2-280-30 FILE=COLVAR280-30 STRIDE=10000 FMT=%16.10f

weights280-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=280 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-280-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights280-35 CLEAR=10000
avg2-280-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights280-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-280-35,avg2-280-35 FILE=COLVAR280-35 STRIDE=10000 FMT=%16.10f

weights280-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=280 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-280-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights280-40 CLEAR=10000
avg2-280-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights280-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-280-40,avg2-280-40 FILE=COLVAR280-40 STRIDE=10000 FMT=%16.10f

weights280-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=280 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-280-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights280-45 CLEAR=10000
avg2-280-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights280-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-280-45,avg2-280-45 FILE=COLVAR280-45 STRIDE=10000 FMT=%16.10f

weights280-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=280 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-280-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights280-50 CLEAR=10000
avg2-280-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights280-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-280-50,avg2-280-50 FILE=COLVAR280-50 STRIDE=10000 FMT=%16.10f

weights280-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=280 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-280-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights280-55 CLEAR=10000
avg2-280-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights280-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-280-55,avg2-280-55 FILE=COLVAR280-55 STRIDE=10000 FMT=%16.10f

weights280-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=280 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-280-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights280-60 CLEAR=10000
avg2-280-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights280-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-280-60,avg2-280-60 FILE=COLVAR280-60 STRIDE=10000 FMT=%16.10f

weights280-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=280 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-280-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights280-65 CLEAR=10000
avg2-280-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights280-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-280-65,avg2-280-65 FILE=COLVAR280-65 STRIDE=10000 FMT=%16.10f

weights280-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=280 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-280-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights280-70 CLEAR=10000
avg2-280-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights280-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-280-70,avg2-280-70 FILE=COLVAR280-70 STRIDE=10000 FMT=%16.10f

weights280-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=280 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-280-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights280-75 CLEAR=10000
avg2-280-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights280-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-280-75,avg2-280-75 FILE=COLVAR280-75 STRIDE=10000 FMT=%16.10f

weights280-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=280 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-280-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights280-80 CLEAR=10000
avg2-280-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights280-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-280-80,avg2-280-80 FILE=COLVAR280-80 STRIDE=10000 FMT=%16.10f

weights280-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=280 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-280-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights280-85 CLEAR=10000
avg2-280-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights280-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-280-85,avg2-280-85 FILE=COLVAR280-85 STRIDE=10000 FMT=%16.10f

weights280-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=280 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-280-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights280-90 CLEAR=10000
avg2-280-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights280-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-280-90,avg2-280-90 FILE=COLVAR280-90 STRIDE=10000 FMT=%16.10f

weights280-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=280 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-280-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights280-95 CLEAR=10000
avg2-280-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights280-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-280-95,avg2-280-95 FILE=COLVAR280-95 STRIDE=10000 FMT=%16.10f

weights280-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=280 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-280-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights280-100 CLEAR=10000
avg2-280-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights280-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-280-100,avg2-280-100 FILE=COLVAR280-100 STRIDE=10000 FMT=%16.10f

weights282-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=282 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-282-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights282-0 CLEAR=10000
avg2-282-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights282-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-282-0,avg2-282-0 FILE=COLVAR282-0 STRIDE=10000 FMT=%16.10f

weights282-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=282 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-282-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights282-5 CLEAR=10000
avg2-282-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights282-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-282-5,avg2-282-5 FILE=COLVAR282-5 STRIDE=10000 FMT=%16.10f

weights282-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=282 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-282-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights282-10 CLEAR=10000
avg2-282-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights282-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-282-10,avg2-282-10 FILE=COLVAR282-10 STRIDE=10000 FMT=%16.10f

weights282-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=282 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-282-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights282-15 CLEAR=10000
avg2-282-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights282-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-282-15,avg2-282-15 FILE=COLVAR282-15 STRIDE=10000 FMT=%16.10f

weights282-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=282 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-282-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights282-20 CLEAR=10000
avg2-282-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights282-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-282-20,avg2-282-20 FILE=COLVAR282-20 STRIDE=10000 FMT=%16.10f

weights282-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=282 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-282-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights282-25 CLEAR=10000
avg2-282-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights282-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-282-25,avg2-282-25 FILE=COLVAR282-25 STRIDE=10000 FMT=%16.10f

weights282-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=282 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-282-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights282-30 CLEAR=10000
avg2-282-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights282-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-282-30,avg2-282-30 FILE=COLVAR282-30 STRIDE=10000 FMT=%16.10f

weights282-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=282 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-282-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights282-35 CLEAR=10000
avg2-282-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights282-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-282-35,avg2-282-35 FILE=COLVAR282-35 STRIDE=10000 FMT=%16.10f

weights282-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=282 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-282-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights282-40 CLEAR=10000
avg2-282-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights282-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-282-40,avg2-282-40 FILE=COLVAR282-40 STRIDE=10000 FMT=%16.10f

weights282-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=282 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-282-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights282-45 CLEAR=10000
avg2-282-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights282-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-282-45,avg2-282-45 FILE=COLVAR282-45 STRIDE=10000 FMT=%16.10f

weights282-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=282 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-282-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights282-50 CLEAR=10000
avg2-282-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights282-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-282-50,avg2-282-50 FILE=COLVAR282-50 STRIDE=10000 FMT=%16.10f

weights282-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=282 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-282-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights282-55 CLEAR=10000
avg2-282-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights282-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-282-55,avg2-282-55 FILE=COLVAR282-55 STRIDE=10000 FMT=%16.10f

weights282-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=282 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-282-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights282-60 CLEAR=10000
avg2-282-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights282-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-282-60,avg2-282-60 FILE=COLVAR282-60 STRIDE=10000 FMT=%16.10f

weights282-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=282 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-282-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights282-65 CLEAR=10000
avg2-282-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights282-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-282-65,avg2-282-65 FILE=COLVAR282-65 STRIDE=10000 FMT=%16.10f

weights282-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=282 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-282-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights282-70 CLEAR=10000
avg2-282-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights282-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-282-70,avg2-282-70 FILE=COLVAR282-70 STRIDE=10000 FMT=%16.10f

weights282-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=282 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-282-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights282-75 CLEAR=10000
avg2-282-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights282-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-282-75,avg2-282-75 FILE=COLVAR282-75 STRIDE=10000 FMT=%16.10f

weights282-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=282 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-282-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights282-80 CLEAR=10000
avg2-282-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights282-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-282-80,avg2-282-80 FILE=COLVAR282-80 STRIDE=10000 FMT=%16.10f

weights282-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=282 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-282-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights282-85 CLEAR=10000
avg2-282-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights282-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-282-85,avg2-282-85 FILE=COLVAR282-85 STRIDE=10000 FMT=%16.10f

weights282-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=282 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-282-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights282-90 CLEAR=10000
avg2-282-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights282-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-282-90,avg2-282-90 FILE=COLVAR282-90 STRIDE=10000 FMT=%16.10f

weights282-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=282 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-282-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights282-95 CLEAR=10000
avg2-282-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights282-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-282-95,avg2-282-95 FILE=COLVAR282-95 STRIDE=10000 FMT=%16.10f

weights282-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=282 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-282-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights282-100 CLEAR=10000
avg2-282-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights282-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-282-100,avg2-282-100 FILE=COLVAR282-100 STRIDE=10000 FMT=%16.10f

weights284-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=284 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-284-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights284-0 CLEAR=10000
avg2-284-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights284-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-284-0,avg2-284-0 FILE=COLVAR284-0 STRIDE=10000 FMT=%16.10f

weights284-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=284 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-284-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights284-5 CLEAR=10000
avg2-284-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights284-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-284-5,avg2-284-5 FILE=COLVAR284-5 STRIDE=10000 FMT=%16.10f

weights284-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=284 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-284-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights284-10 CLEAR=10000
avg2-284-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights284-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-284-10,avg2-284-10 FILE=COLVAR284-10 STRIDE=10000 FMT=%16.10f

weights284-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=284 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-284-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights284-15 CLEAR=10000
avg2-284-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights284-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-284-15,avg2-284-15 FILE=COLVAR284-15 STRIDE=10000 FMT=%16.10f

weights284-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=284 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-284-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights284-20 CLEAR=10000
avg2-284-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights284-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-284-20,avg2-284-20 FILE=COLVAR284-20 STRIDE=10000 FMT=%16.10f

weights284-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=284 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-284-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights284-25 CLEAR=10000
avg2-284-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights284-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-284-25,avg2-284-25 FILE=COLVAR284-25 STRIDE=10000 FMT=%16.10f

weights284-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=284 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-284-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights284-30 CLEAR=10000
avg2-284-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights284-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-284-30,avg2-284-30 FILE=COLVAR284-30 STRIDE=10000 FMT=%16.10f

weights284-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=284 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-284-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights284-35 CLEAR=10000
avg2-284-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights284-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-284-35,avg2-284-35 FILE=COLVAR284-35 STRIDE=10000 FMT=%16.10f

weights284-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=284 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-284-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights284-40 CLEAR=10000
avg2-284-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights284-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-284-40,avg2-284-40 FILE=COLVAR284-40 STRIDE=10000 FMT=%16.10f

weights284-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=284 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-284-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights284-45 CLEAR=10000
avg2-284-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights284-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-284-45,avg2-284-45 FILE=COLVAR284-45 STRIDE=10000 FMT=%16.10f

weights284-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=284 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-284-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights284-50 CLEAR=10000
avg2-284-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights284-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-284-50,avg2-284-50 FILE=COLVAR284-50 STRIDE=10000 FMT=%16.10f

weights284-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=284 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-284-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights284-55 CLEAR=10000
avg2-284-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights284-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-284-55,avg2-284-55 FILE=COLVAR284-55 STRIDE=10000 FMT=%16.10f

weights284-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=284 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-284-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights284-60 CLEAR=10000
avg2-284-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights284-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-284-60,avg2-284-60 FILE=COLVAR284-60 STRIDE=10000 FMT=%16.10f

weights284-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=284 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-284-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights284-65 CLEAR=10000
avg2-284-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights284-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-284-65,avg2-284-65 FILE=COLVAR284-65 STRIDE=10000 FMT=%16.10f

weights284-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=284 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-284-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights284-70 CLEAR=10000
avg2-284-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights284-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-284-70,avg2-284-70 FILE=COLVAR284-70 STRIDE=10000 FMT=%16.10f

weights284-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=284 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-284-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights284-75 CLEAR=10000
avg2-284-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights284-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-284-75,avg2-284-75 FILE=COLVAR284-75 STRIDE=10000 FMT=%16.10f

weights284-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=284 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-284-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights284-80 CLEAR=10000
avg2-284-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights284-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-284-80,avg2-284-80 FILE=COLVAR284-80 STRIDE=10000 FMT=%16.10f

weights284-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=284 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-284-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights284-85 CLEAR=10000
avg2-284-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights284-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-284-85,avg2-284-85 FILE=COLVAR284-85 STRIDE=10000 FMT=%16.10f

weights284-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=284 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-284-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights284-90 CLEAR=10000
avg2-284-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights284-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-284-90,avg2-284-90 FILE=COLVAR284-90 STRIDE=10000 FMT=%16.10f

weights284-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=284 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-284-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights284-95 CLEAR=10000
avg2-284-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights284-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-284-95,avg2-284-95 FILE=COLVAR284-95 STRIDE=10000 FMT=%16.10f

weights284-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=284 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-284-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights284-100 CLEAR=10000
avg2-284-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights284-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-284-100,avg2-284-100 FILE=COLVAR284-100 STRIDE=10000 FMT=%16.10f

weights286-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=286 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-286-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights286-0 CLEAR=10000
avg2-286-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights286-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-286-0,avg2-286-0 FILE=COLVAR286-0 STRIDE=10000 FMT=%16.10f

weights286-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=286 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-286-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights286-5 CLEAR=10000
avg2-286-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights286-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-286-5,avg2-286-5 FILE=COLVAR286-5 STRIDE=10000 FMT=%16.10f

weights286-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=286 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-286-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights286-10 CLEAR=10000
avg2-286-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights286-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-286-10,avg2-286-10 FILE=COLVAR286-10 STRIDE=10000 FMT=%16.10f

weights286-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=286 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-286-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights286-15 CLEAR=10000
avg2-286-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights286-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-286-15,avg2-286-15 FILE=COLVAR286-15 STRIDE=10000 FMT=%16.10f

weights286-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=286 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-286-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights286-20 CLEAR=10000
avg2-286-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights286-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-286-20,avg2-286-20 FILE=COLVAR286-20 STRIDE=10000 FMT=%16.10f

weights286-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=286 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-286-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights286-25 CLEAR=10000
avg2-286-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights286-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-286-25,avg2-286-25 FILE=COLVAR286-25 STRIDE=10000 FMT=%16.10f

weights286-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=286 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-286-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights286-30 CLEAR=10000
avg2-286-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights286-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-286-30,avg2-286-30 FILE=COLVAR286-30 STRIDE=10000 FMT=%16.10f

weights286-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=286 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-286-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights286-35 CLEAR=10000
avg2-286-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights286-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-286-35,avg2-286-35 FILE=COLVAR286-35 STRIDE=10000 FMT=%16.10f

weights286-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=286 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-286-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights286-40 CLEAR=10000
avg2-286-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights286-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-286-40,avg2-286-40 FILE=COLVAR286-40 STRIDE=10000 FMT=%16.10f

weights286-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=286 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-286-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights286-45 CLEAR=10000
avg2-286-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights286-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-286-45,avg2-286-45 FILE=COLVAR286-45 STRIDE=10000 FMT=%16.10f

weights286-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=286 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-286-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights286-50 CLEAR=10000
avg2-286-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights286-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-286-50,avg2-286-50 FILE=COLVAR286-50 STRIDE=10000 FMT=%16.10f

weights286-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=286 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-286-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights286-55 CLEAR=10000
avg2-286-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights286-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-286-55,avg2-286-55 FILE=COLVAR286-55 STRIDE=10000 FMT=%16.10f

weights286-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=286 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-286-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights286-60 CLEAR=10000
avg2-286-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights286-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-286-60,avg2-286-60 FILE=COLVAR286-60 STRIDE=10000 FMT=%16.10f

weights286-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=286 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-286-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights286-65 CLEAR=10000
avg2-286-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights286-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-286-65,avg2-286-65 FILE=COLVAR286-65 STRIDE=10000 FMT=%16.10f

weights286-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=286 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-286-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights286-70 CLEAR=10000
avg2-286-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights286-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-286-70,avg2-286-70 FILE=COLVAR286-70 STRIDE=10000 FMT=%16.10f

weights286-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=286 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-286-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights286-75 CLEAR=10000
avg2-286-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights286-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-286-75,avg2-286-75 FILE=COLVAR286-75 STRIDE=10000 FMT=%16.10f

weights286-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=286 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-286-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights286-80 CLEAR=10000
avg2-286-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights286-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-286-80,avg2-286-80 FILE=COLVAR286-80 STRIDE=10000 FMT=%16.10f

weights286-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=286 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-286-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights286-85 CLEAR=10000
avg2-286-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights286-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-286-85,avg2-286-85 FILE=COLVAR286-85 STRIDE=10000 FMT=%16.10f

weights286-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=286 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-286-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights286-90 CLEAR=10000
avg2-286-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights286-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-286-90,avg2-286-90 FILE=COLVAR286-90 STRIDE=10000 FMT=%16.10f

weights286-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=286 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-286-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights286-95 CLEAR=10000
avg2-286-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights286-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-286-95,avg2-286-95 FILE=COLVAR286-95 STRIDE=10000 FMT=%16.10f

weights286-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=286 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-286-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights286-100 CLEAR=10000
avg2-286-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights286-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-286-100,avg2-286-100 FILE=COLVAR286-100 STRIDE=10000 FMT=%16.10f

weights288-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=288 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-288-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights288-0 CLEAR=10000
avg2-288-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights288-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-288-0,avg2-288-0 FILE=COLVAR288-0 STRIDE=10000 FMT=%16.10f

weights288-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=288 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-288-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights288-5 CLEAR=10000
avg2-288-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights288-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-288-5,avg2-288-5 FILE=COLVAR288-5 STRIDE=10000 FMT=%16.10f

weights288-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=288 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-288-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights288-10 CLEAR=10000
avg2-288-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights288-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-288-10,avg2-288-10 FILE=COLVAR288-10 STRIDE=10000 FMT=%16.10f

weights288-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=288 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-288-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights288-15 CLEAR=10000
avg2-288-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights288-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-288-15,avg2-288-15 FILE=COLVAR288-15 STRIDE=10000 FMT=%16.10f

weights288-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=288 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-288-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights288-20 CLEAR=10000
avg2-288-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights288-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-288-20,avg2-288-20 FILE=COLVAR288-20 STRIDE=10000 FMT=%16.10f

weights288-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=288 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-288-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights288-25 CLEAR=10000
avg2-288-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights288-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-288-25,avg2-288-25 FILE=COLVAR288-25 STRIDE=10000 FMT=%16.10f

weights288-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=288 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-288-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights288-30 CLEAR=10000
avg2-288-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights288-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-288-30,avg2-288-30 FILE=COLVAR288-30 STRIDE=10000 FMT=%16.10f

weights288-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=288 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-288-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights288-35 CLEAR=10000
avg2-288-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights288-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-288-35,avg2-288-35 FILE=COLVAR288-35 STRIDE=10000 FMT=%16.10f

weights288-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=288 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-288-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights288-40 CLEAR=10000
avg2-288-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights288-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-288-40,avg2-288-40 FILE=COLVAR288-40 STRIDE=10000 FMT=%16.10f

weights288-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=288 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-288-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights288-45 CLEAR=10000
avg2-288-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights288-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-288-45,avg2-288-45 FILE=COLVAR288-45 STRIDE=10000 FMT=%16.10f

weights288-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=288 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-288-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights288-50 CLEAR=10000
avg2-288-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights288-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-288-50,avg2-288-50 FILE=COLVAR288-50 STRIDE=10000 FMT=%16.10f

weights288-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=288 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-288-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights288-55 CLEAR=10000
avg2-288-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights288-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-288-55,avg2-288-55 FILE=COLVAR288-55 STRIDE=10000 FMT=%16.10f

weights288-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=288 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-288-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights288-60 CLEAR=10000
avg2-288-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights288-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-288-60,avg2-288-60 FILE=COLVAR288-60 STRIDE=10000 FMT=%16.10f

weights288-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=288 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-288-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights288-65 CLEAR=10000
avg2-288-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights288-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-288-65,avg2-288-65 FILE=COLVAR288-65 STRIDE=10000 FMT=%16.10f

weights288-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=288 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-288-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights288-70 CLEAR=10000
avg2-288-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights288-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-288-70,avg2-288-70 FILE=COLVAR288-70 STRIDE=10000 FMT=%16.10f

weights288-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=288 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-288-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights288-75 CLEAR=10000
avg2-288-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights288-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-288-75,avg2-288-75 FILE=COLVAR288-75 STRIDE=10000 FMT=%16.10f

weights288-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=288 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-288-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights288-80 CLEAR=10000
avg2-288-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights288-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-288-80,avg2-288-80 FILE=COLVAR288-80 STRIDE=10000 FMT=%16.10f

weights288-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=288 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-288-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights288-85 CLEAR=10000
avg2-288-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights288-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-288-85,avg2-288-85 FILE=COLVAR288-85 STRIDE=10000 FMT=%16.10f

weights288-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=288 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-288-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights288-90 CLEAR=10000
avg2-288-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights288-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-288-90,avg2-288-90 FILE=COLVAR288-90 STRIDE=10000 FMT=%16.10f

weights288-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=288 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-288-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights288-95 CLEAR=10000
avg2-288-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights288-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-288-95,avg2-288-95 FILE=COLVAR288-95 STRIDE=10000 FMT=%16.10f

weights288-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=288 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-288-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights288-100 CLEAR=10000
avg2-288-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights288-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-288-100,avg2-288-100 FILE=COLVAR288-100 STRIDE=10000 FMT=%16.10f

weights290-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=290 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-290-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights290-0 CLEAR=10000
avg2-290-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights290-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-290-0,avg2-290-0 FILE=COLVAR290-0 STRIDE=10000 FMT=%16.10f

weights290-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=290 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-290-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights290-5 CLEAR=10000
avg2-290-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights290-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-290-5,avg2-290-5 FILE=COLVAR290-5 STRIDE=10000 FMT=%16.10f

weights290-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=290 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-290-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights290-10 CLEAR=10000
avg2-290-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights290-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-290-10,avg2-290-10 FILE=COLVAR290-10 STRIDE=10000 FMT=%16.10f

weights290-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=290 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-290-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights290-15 CLEAR=10000
avg2-290-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights290-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-290-15,avg2-290-15 FILE=COLVAR290-15 STRIDE=10000 FMT=%16.10f

weights290-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=290 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-290-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights290-20 CLEAR=10000
avg2-290-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights290-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-290-20,avg2-290-20 FILE=COLVAR290-20 STRIDE=10000 FMT=%16.10f

weights290-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=290 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-290-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights290-25 CLEAR=10000
avg2-290-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights290-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-290-25,avg2-290-25 FILE=COLVAR290-25 STRIDE=10000 FMT=%16.10f

weights290-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=290 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-290-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights290-30 CLEAR=10000
avg2-290-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights290-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-290-30,avg2-290-30 FILE=COLVAR290-30 STRIDE=10000 FMT=%16.10f

weights290-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=290 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-290-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights290-35 CLEAR=10000
avg2-290-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights290-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-290-35,avg2-290-35 FILE=COLVAR290-35 STRIDE=10000 FMT=%16.10f

weights290-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=290 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-290-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights290-40 CLEAR=10000
avg2-290-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights290-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-290-40,avg2-290-40 FILE=COLVAR290-40 STRIDE=10000 FMT=%16.10f

weights290-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=290 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-290-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights290-45 CLEAR=10000
avg2-290-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights290-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-290-45,avg2-290-45 FILE=COLVAR290-45 STRIDE=10000 FMT=%16.10f

weights290-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=290 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-290-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights290-50 CLEAR=10000
avg2-290-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights290-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-290-50,avg2-290-50 FILE=COLVAR290-50 STRIDE=10000 FMT=%16.10f

weights290-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=290 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-290-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights290-55 CLEAR=10000
avg2-290-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights290-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-290-55,avg2-290-55 FILE=COLVAR290-55 STRIDE=10000 FMT=%16.10f

weights290-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=290 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-290-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights290-60 CLEAR=10000
avg2-290-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights290-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-290-60,avg2-290-60 FILE=COLVAR290-60 STRIDE=10000 FMT=%16.10f

weights290-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=290 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-290-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights290-65 CLEAR=10000
avg2-290-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights290-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-290-65,avg2-290-65 FILE=COLVAR290-65 STRIDE=10000 FMT=%16.10f

weights290-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=290 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-290-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights290-70 CLEAR=10000
avg2-290-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights290-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-290-70,avg2-290-70 FILE=COLVAR290-70 STRIDE=10000 FMT=%16.10f

weights290-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=290 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-290-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights290-75 CLEAR=10000
avg2-290-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights290-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-290-75,avg2-290-75 FILE=COLVAR290-75 STRIDE=10000 FMT=%16.10f

weights290-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=290 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-290-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights290-80 CLEAR=10000
avg2-290-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights290-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-290-80,avg2-290-80 FILE=COLVAR290-80 STRIDE=10000 FMT=%16.10f

weights290-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=290 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-290-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights290-85 CLEAR=10000
avg2-290-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights290-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-290-85,avg2-290-85 FILE=COLVAR290-85 STRIDE=10000 FMT=%16.10f

weights290-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=290 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-290-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights290-90 CLEAR=10000
avg2-290-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights290-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-290-90,avg2-290-90 FILE=COLVAR290-90 STRIDE=10000 FMT=%16.10f

weights290-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=290 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-290-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights290-95 CLEAR=10000
avg2-290-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights290-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-290-95,avg2-290-95 FILE=COLVAR290-95 STRIDE=10000 FMT=%16.10f

weights290-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=290 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-290-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights290-100 CLEAR=10000
avg2-290-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights290-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-290-100,avg2-290-100 FILE=COLVAR290-100 STRIDE=10000 FMT=%16.10f

weights292-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=292 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-292-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights292-0 CLEAR=10000
avg2-292-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights292-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-292-0,avg2-292-0 FILE=COLVAR292-0 STRIDE=10000 FMT=%16.10f

weights292-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=292 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-292-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights292-5 CLEAR=10000
avg2-292-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights292-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-292-5,avg2-292-5 FILE=COLVAR292-5 STRIDE=10000 FMT=%16.10f

weights292-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=292 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-292-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights292-10 CLEAR=10000
avg2-292-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights292-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-292-10,avg2-292-10 FILE=COLVAR292-10 STRIDE=10000 FMT=%16.10f

weights292-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=292 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-292-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights292-15 CLEAR=10000
avg2-292-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights292-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-292-15,avg2-292-15 FILE=COLVAR292-15 STRIDE=10000 FMT=%16.10f

weights292-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=292 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-292-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights292-20 CLEAR=10000
avg2-292-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights292-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-292-20,avg2-292-20 FILE=COLVAR292-20 STRIDE=10000 FMT=%16.10f

weights292-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=292 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-292-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights292-25 CLEAR=10000
avg2-292-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights292-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-292-25,avg2-292-25 FILE=COLVAR292-25 STRIDE=10000 FMT=%16.10f

weights292-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=292 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-292-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights292-30 CLEAR=10000
avg2-292-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights292-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-292-30,avg2-292-30 FILE=COLVAR292-30 STRIDE=10000 FMT=%16.10f

weights292-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=292 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-292-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights292-35 CLEAR=10000
avg2-292-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights292-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-292-35,avg2-292-35 FILE=COLVAR292-35 STRIDE=10000 FMT=%16.10f

weights292-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=292 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-292-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights292-40 CLEAR=10000
avg2-292-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights292-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-292-40,avg2-292-40 FILE=COLVAR292-40 STRIDE=10000 FMT=%16.10f

weights292-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=292 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-292-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights292-45 CLEAR=10000
avg2-292-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights292-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-292-45,avg2-292-45 FILE=COLVAR292-45 STRIDE=10000 FMT=%16.10f

weights292-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=292 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-292-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights292-50 CLEAR=10000
avg2-292-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights292-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-292-50,avg2-292-50 FILE=COLVAR292-50 STRIDE=10000 FMT=%16.10f

weights292-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=292 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-292-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights292-55 CLEAR=10000
avg2-292-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights292-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-292-55,avg2-292-55 FILE=COLVAR292-55 STRIDE=10000 FMT=%16.10f

weights292-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=292 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-292-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights292-60 CLEAR=10000
avg2-292-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights292-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-292-60,avg2-292-60 FILE=COLVAR292-60 STRIDE=10000 FMT=%16.10f

weights292-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=292 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-292-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights292-65 CLEAR=10000
avg2-292-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights292-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-292-65,avg2-292-65 FILE=COLVAR292-65 STRIDE=10000 FMT=%16.10f

weights292-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=292 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-292-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights292-70 CLEAR=10000
avg2-292-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights292-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-292-70,avg2-292-70 FILE=COLVAR292-70 STRIDE=10000 FMT=%16.10f

weights292-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=292 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-292-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights292-75 CLEAR=10000
avg2-292-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights292-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-292-75,avg2-292-75 FILE=COLVAR292-75 STRIDE=10000 FMT=%16.10f

weights292-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=292 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-292-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights292-80 CLEAR=10000
avg2-292-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights292-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-292-80,avg2-292-80 FILE=COLVAR292-80 STRIDE=10000 FMT=%16.10f

weights292-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=292 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-292-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights292-85 CLEAR=10000
avg2-292-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights292-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-292-85,avg2-292-85 FILE=COLVAR292-85 STRIDE=10000 FMT=%16.10f

weights292-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=292 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-292-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights292-90 CLEAR=10000
avg2-292-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights292-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-292-90,avg2-292-90 FILE=COLVAR292-90 STRIDE=10000 FMT=%16.10f

weights292-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=292 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-292-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights292-95 CLEAR=10000
avg2-292-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights292-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-292-95,avg2-292-95 FILE=COLVAR292-95 STRIDE=10000 FMT=%16.10f

weights292-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=292 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-292-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights292-100 CLEAR=10000
avg2-292-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights292-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-292-100,avg2-292-100 FILE=COLVAR292-100 STRIDE=10000 FMT=%16.10f

weights294-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=294 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-294-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights294-0 CLEAR=10000
avg2-294-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights294-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-294-0,avg2-294-0 FILE=COLVAR294-0 STRIDE=10000 FMT=%16.10f

weights294-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=294 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-294-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights294-5 CLEAR=10000
avg2-294-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights294-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-294-5,avg2-294-5 FILE=COLVAR294-5 STRIDE=10000 FMT=%16.10f

weights294-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=294 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-294-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights294-10 CLEAR=10000
avg2-294-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights294-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-294-10,avg2-294-10 FILE=COLVAR294-10 STRIDE=10000 FMT=%16.10f

weights294-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=294 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-294-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights294-15 CLEAR=10000
avg2-294-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights294-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-294-15,avg2-294-15 FILE=COLVAR294-15 STRIDE=10000 FMT=%16.10f

weights294-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=294 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-294-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights294-20 CLEAR=10000
avg2-294-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights294-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-294-20,avg2-294-20 FILE=COLVAR294-20 STRIDE=10000 FMT=%16.10f

weights294-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=294 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-294-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights294-25 CLEAR=10000
avg2-294-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights294-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-294-25,avg2-294-25 FILE=COLVAR294-25 STRIDE=10000 FMT=%16.10f

weights294-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=294 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-294-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights294-30 CLEAR=10000
avg2-294-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights294-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-294-30,avg2-294-30 FILE=COLVAR294-30 STRIDE=10000 FMT=%16.10f

weights294-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=294 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-294-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights294-35 CLEAR=10000
avg2-294-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights294-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-294-35,avg2-294-35 FILE=COLVAR294-35 STRIDE=10000 FMT=%16.10f

weights294-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=294 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-294-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights294-40 CLEAR=10000
avg2-294-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights294-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-294-40,avg2-294-40 FILE=COLVAR294-40 STRIDE=10000 FMT=%16.10f

weights294-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=294 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-294-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights294-45 CLEAR=10000
avg2-294-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights294-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-294-45,avg2-294-45 FILE=COLVAR294-45 STRIDE=10000 FMT=%16.10f

weights294-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=294 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-294-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights294-50 CLEAR=10000
avg2-294-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights294-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-294-50,avg2-294-50 FILE=COLVAR294-50 STRIDE=10000 FMT=%16.10f

weights294-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=294 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-294-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights294-55 CLEAR=10000
avg2-294-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights294-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-294-55,avg2-294-55 FILE=COLVAR294-55 STRIDE=10000 FMT=%16.10f

weights294-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=294 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-294-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights294-60 CLEAR=10000
avg2-294-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights294-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-294-60,avg2-294-60 FILE=COLVAR294-60 STRIDE=10000 FMT=%16.10f

weights294-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=294 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-294-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights294-65 CLEAR=10000
avg2-294-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights294-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-294-65,avg2-294-65 FILE=COLVAR294-65 STRIDE=10000 FMT=%16.10f

weights294-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=294 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-294-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights294-70 CLEAR=10000
avg2-294-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights294-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-294-70,avg2-294-70 FILE=COLVAR294-70 STRIDE=10000 FMT=%16.10f

weights294-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=294 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-294-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights294-75 CLEAR=10000
avg2-294-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights294-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-294-75,avg2-294-75 FILE=COLVAR294-75 STRIDE=10000 FMT=%16.10f

weights294-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=294 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-294-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights294-80 CLEAR=10000
avg2-294-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights294-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-294-80,avg2-294-80 FILE=COLVAR294-80 STRIDE=10000 FMT=%16.10f

weights294-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=294 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-294-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights294-85 CLEAR=10000
avg2-294-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights294-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-294-85,avg2-294-85 FILE=COLVAR294-85 STRIDE=10000 FMT=%16.10f

weights294-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=294 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-294-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights294-90 CLEAR=10000
avg2-294-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights294-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-294-90,avg2-294-90 FILE=COLVAR294-90 STRIDE=10000 FMT=%16.10f

weights294-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=294 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-294-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights294-95 CLEAR=10000
avg2-294-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights294-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-294-95,avg2-294-95 FILE=COLVAR294-95 STRIDE=10000 FMT=%16.10f

weights294-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=294 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-294-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights294-100 CLEAR=10000
avg2-294-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights294-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-294-100,avg2-294-100 FILE=COLVAR294-100 STRIDE=10000 FMT=%16.10f

weights296-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=296 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-296-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights296-0 CLEAR=10000
avg2-296-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights296-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-296-0,avg2-296-0 FILE=COLVAR296-0 STRIDE=10000 FMT=%16.10f

weights296-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=296 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-296-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights296-5 CLEAR=10000
avg2-296-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights296-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-296-5,avg2-296-5 FILE=COLVAR296-5 STRIDE=10000 FMT=%16.10f

weights296-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=296 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-296-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights296-10 CLEAR=10000
avg2-296-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights296-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-296-10,avg2-296-10 FILE=COLVAR296-10 STRIDE=10000 FMT=%16.10f

weights296-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=296 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-296-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights296-15 CLEAR=10000
avg2-296-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights296-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-296-15,avg2-296-15 FILE=COLVAR296-15 STRIDE=10000 FMT=%16.10f

weights296-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=296 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-296-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights296-20 CLEAR=10000
avg2-296-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights296-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-296-20,avg2-296-20 FILE=COLVAR296-20 STRIDE=10000 FMT=%16.10f

weights296-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=296 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-296-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights296-25 CLEAR=10000
avg2-296-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights296-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-296-25,avg2-296-25 FILE=COLVAR296-25 STRIDE=10000 FMT=%16.10f

weights296-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=296 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-296-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights296-30 CLEAR=10000
avg2-296-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights296-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-296-30,avg2-296-30 FILE=COLVAR296-30 STRIDE=10000 FMT=%16.10f

weights296-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=296 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-296-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights296-35 CLEAR=10000
avg2-296-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights296-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-296-35,avg2-296-35 FILE=COLVAR296-35 STRIDE=10000 FMT=%16.10f

weights296-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=296 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-296-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights296-40 CLEAR=10000
avg2-296-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights296-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-296-40,avg2-296-40 FILE=COLVAR296-40 STRIDE=10000 FMT=%16.10f

weights296-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=296 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-296-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights296-45 CLEAR=10000
avg2-296-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights296-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-296-45,avg2-296-45 FILE=COLVAR296-45 STRIDE=10000 FMT=%16.10f

weights296-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=296 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-296-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights296-50 CLEAR=10000
avg2-296-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights296-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-296-50,avg2-296-50 FILE=COLVAR296-50 STRIDE=10000 FMT=%16.10f

weights296-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=296 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-296-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights296-55 CLEAR=10000
avg2-296-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights296-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-296-55,avg2-296-55 FILE=COLVAR296-55 STRIDE=10000 FMT=%16.10f

weights296-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=296 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-296-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights296-60 CLEAR=10000
avg2-296-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights296-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-296-60,avg2-296-60 FILE=COLVAR296-60 STRIDE=10000 FMT=%16.10f

weights296-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=296 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-296-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights296-65 CLEAR=10000
avg2-296-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights296-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-296-65,avg2-296-65 FILE=COLVAR296-65 STRIDE=10000 FMT=%16.10f

weights296-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=296 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-296-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights296-70 CLEAR=10000
avg2-296-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights296-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-296-70,avg2-296-70 FILE=COLVAR296-70 STRIDE=10000 FMT=%16.10f

weights296-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=296 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-296-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights296-75 CLEAR=10000
avg2-296-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights296-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-296-75,avg2-296-75 FILE=COLVAR296-75 STRIDE=10000 FMT=%16.10f

weights296-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=296 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-296-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights296-80 CLEAR=10000
avg2-296-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights296-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-296-80,avg2-296-80 FILE=COLVAR296-80 STRIDE=10000 FMT=%16.10f

weights296-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=296 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-296-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights296-85 CLEAR=10000
avg2-296-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights296-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-296-85,avg2-296-85 FILE=COLVAR296-85 STRIDE=10000 FMT=%16.10f

weights296-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=296 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-296-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights296-90 CLEAR=10000
avg2-296-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights296-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-296-90,avg2-296-90 FILE=COLVAR296-90 STRIDE=10000 FMT=%16.10f

weights296-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=296 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-296-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights296-95 CLEAR=10000
avg2-296-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights296-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-296-95,avg2-296-95 FILE=COLVAR296-95 STRIDE=10000 FMT=%16.10f

weights296-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=296 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-296-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights296-100 CLEAR=10000
avg2-296-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights296-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-296-100,avg2-296-100 FILE=COLVAR296-100 STRIDE=10000 FMT=%16.10f

weights298-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=298 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-298-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights298-0 CLEAR=10000
avg2-298-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights298-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-298-0,avg2-298-0 FILE=COLVAR298-0 STRIDE=10000 FMT=%16.10f

weights298-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=298 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-298-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights298-5 CLEAR=10000
avg2-298-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights298-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-298-5,avg2-298-5 FILE=COLVAR298-5 STRIDE=10000 FMT=%16.10f

weights298-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=298 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-298-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights298-10 CLEAR=10000
avg2-298-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights298-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-298-10,avg2-298-10 FILE=COLVAR298-10 STRIDE=10000 FMT=%16.10f

weights298-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=298 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-298-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights298-15 CLEAR=10000
avg2-298-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights298-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-298-15,avg2-298-15 FILE=COLVAR298-15 STRIDE=10000 FMT=%16.10f

weights298-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=298 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-298-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights298-20 CLEAR=10000
avg2-298-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights298-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-298-20,avg2-298-20 FILE=COLVAR298-20 STRIDE=10000 FMT=%16.10f

weights298-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=298 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-298-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights298-25 CLEAR=10000
avg2-298-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights298-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-298-25,avg2-298-25 FILE=COLVAR298-25 STRIDE=10000 FMT=%16.10f

weights298-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=298 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-298-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights298-30 CLEAR=10000
avg2-298-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights298-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-298-30,avg2-298-30 FILE=COLVAR298-30 STRIDE=10000 FMT=%16.10f

weights298-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=298 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-298-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights298-35 CLEAR=10000
avg2-298-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights298-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-298-35,avg2-298-35 FILE=COLVAR298-35 STRIDE=10000 FMT=%16.10f

weights298-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=298 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-298-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights298-40 CLEAR=10000
avg2-298-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights298-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-298-40,avg2-298-40 FILE=COLVAR298-40 STRIDE=10000 FMT=%16.10f

weights298-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=298 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-298-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights298-45 CLEAR=10000
avg2-298-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights298-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-298-45,avg2-298-45 FILE=COLVAR298-45 STRIDE=10000 FMT=%16.10f

weights298-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=298 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-298-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights298-50 CLEAR=10000
avg2-298-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights298-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-298-50,avg2-298-50 FILE=COLVAR298-50 STRIDE=10000 FMT=%16.10f

weights298-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=298 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-298-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights298-55 CLEAR=10000
avg2-298-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights298-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-298-55,avg2-298-55 FILE=COLVAR298-55 STRIDE=10000 FMT=%16.10f

weights298-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=298 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-298-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights298-60 CLEAR=10000
avg2-298-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights298-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-298-60,avg2-298-60 FILE=COLVAR298-60 STRIDE=10000 FMT=%16.10f

weights298-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=298 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-298-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights298-65 CLEAR=10000
avg2-298-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights298-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-298-65,avg2-298-65 FILE=COLVAR298-65 STRIDE=10000 FMT=%16.10f

weights298-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=298 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-298-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights298-70 CLEAR=10000
avg2-298-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights298-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-298-70,avg2-298-70 FILE=COLVAR298-70 STRIDE=10000 FMT=%16.10f

weights298-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=298 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-298-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights298-75 CLEAR=10000
avg2-298-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights298-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-298-75,avg2-298-75 FILE=COLVAR298-75 STRIDE=10000 FMT=%16.10f

weights298-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=298 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-298-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights298-80 CLEAR=10000
avg2-298-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights298-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-298-80,avg2-298-80 FILE=COLVAR298-80 STRIDE=10000 FMT=%16.10f

weights298-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=298 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-298-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights298-85 CLEAR=10000
avg2-298-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights298-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-298-85,avg2-298-85 FILE=COLVAR298-85 STRIDE=10000 FMT=%16.10f

weights298-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=298 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-298-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights298-90 CLEAR=10000
avg2-298-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights298-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-298-90,avg2-298-90 FILE=COLVAR298-90 STRIDE=10000 FMT=%16.10f

weights298-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=298 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-298-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights298-95 CLEAR=10000
avg2-298-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights298-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-298-95,avg2-298-95 FILE=COLVAR298-95 STRIDE=10000 FMT=%16.10f

weights298-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=298 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-298-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights298-100 CLEAR=10000
avg2-298-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights298-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-298-100,avg2-298-100 FILE=COLVAR298-100 STRIDE=10000 FMT=%16.10f

weights300-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=300 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-300-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights300-0 CLEAR=10000
avg2-300-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights300-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-300-0,avg2-300-0 FILE=COLVAR300-0 STRIDE=10000 FMT=%16.10f

weights300-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=300 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-300-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights300-5 CLEAR=10000
avg2-300-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights300-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-300-5,avg2-300-5 FILE=COLVAR300-5 STRIDE=10000 FMT=%16.10f

weights300-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=300 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-300-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights300-10 CLEAR=10000
avg2-300-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights300-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-300-10,avg2-300-10 FILE=COLVAR300-10 STRIDE=10000 FMT=%16.10f

weights300-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=300 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-300-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights300-15 CLEAR=10000
avg2-300-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights300-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-300-15,avg2-300-15 FILE=COLVAR300-15 STRIDE=10000 FMT=%16.10f

weights300-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=300 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-300-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights300-20 CLEAR=10000
avg2-300-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights300-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-300-20,avg2-300-20 FILE=COLVAR300-20 STRIDE=10000 FMT=%16.10f

weights300-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=300 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-300-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights300-25 CLEAR=10000
avg2-300-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights300-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-300-25,avg2-300-25 FILE=COLVAR300-25 STRIDE=10000 FMT=%16.10f

weights300-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=300 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-300-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights300-30 CLEAR=10000
avg2-300-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights300-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-300-30,avg2-300-30 FILE=COLVAR300-30 STRIDE=10000 FMT=%16.10f

weights300-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=300 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-300-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights300-35 CLEAR=10000
avg2-300-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights300-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-300-35,avg2-300-35 FILE=COLVAR300-35 STRIDE=10000 FMT=%16.10f

weights300-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=300 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-300-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights300-40 CLEAR=10000
avg2-300-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights300-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-300-40,avg2-300-40 FILE=COLVAR300-40 STRIDE=10000 FMT=%16.10f

weights300-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=300 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-300-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights300-45 CLEAR=10000
avg2-300-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights300-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-300-45,avg2-300-45 FILE=COLVAR300-45 STRIDE=10000 FMT=%16.10f

weights300-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=300 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-300-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights300-50 CLEAR=10000
avg2-300-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights300-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-300-50,avg2-300-50 FILE=COLVAR300-50 STRIDE=10000 FMT=%16.10f

weights300-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=300 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-300-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights300-55 CLEAR=10000
avg2-300-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights300-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-300-55,avg2-300-55 FILE=COLVAR300-55 STRIDE=10000 FMT=%16.10f

weights300-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=300 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-300-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights300-60 CLEAR=10000
avg2-300-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights300-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-300-60,avg2-300-60 FILE=COLVAR300-60 STRIDE=10000 FMT=%16.10f

weights300-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=300 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-300-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights300-65 CLEAR=10000
avg2-300-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights300-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-300-65,avg2-300-65 FILE=COLVAR300-65 STRIDE=10000 FMT=%16.10f

weights300-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=300 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-300-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights300-70 CLEAR=10000
avg2-300-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights300-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-300-70,avg2-300-70 FILE=COLVAR300-70 STRIDE=10000 FMT=%16.10f

weights300-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=300 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-300-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights300-75 CLEAR=10000
avg2-300-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights300-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-300-75,avg2-300-75 FILE=COLVAR300-75 STRIDE=10000 FMT=%16.10f

weights300-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=300 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-300-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights300-80 CLEAR=10000
avg2-300-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights300-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-300-80,avg2-300-80 FILE=COLVAR300-80 STRIDE=10000 FMT=%16.10f

weights300-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=300 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-300-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights300-85 CLEAR=10000
avg2-300-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights300-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-300-85,avg2-300-85 FILE=COLVAR300-85 STRIDE=10000 FMT=%16.10f

weights300-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=300 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-300-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights300-90 CLEAR=10000
avg2-300-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights300-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-300-90,avg2-300-90 FILE=COLVAR300-90 STRIDE=10000 FMT=%16.10f

weights300-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=300 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-300-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights300-95 CLEAR=10000
avg2-300-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights300-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-300-95,avg2-300-95 FILE=COLVAR300-95 STRIDE=10000 FMT=%16.10f

weights300-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=300 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-300-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights300-100 CLEAR=10000
avg2-300-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights300-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-300-100,avg2-300-100 FILE=COLVAR300-100 STRIDE=10000 FMT=%16.10f

weights302-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=302 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-302-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights302-0 CLEAR=10000
avg2-302-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights302-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-302-0,avg2-302-0 FILE=COLVAR302-0 STRIDE=10000 FMT=%16.10f

weights302-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=302 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-302-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights302-5 CLEAR=10000
avg2-302-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights302-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-302-5,avg2-302-5 FILE=COLVAR302-5 STRIDE=10000 FMT=%16.10f

weights302-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=302 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-302-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights302-10 CLEAR=10000
avg2-302-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights302-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-302-10,avg2-302-10 FILE=COLVAR302-10 STRIDE=10000 FMT=%16.10f

weights302-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=302 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-302-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights302-15 CLEAR=10000
avg2-302-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights302-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-302-15,avg2-302-15 FILE=COLVAR302-15 STRIDE=10000 FMT=%16.10f

weights302-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=302 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-302-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights302-20 CLEAR=10000
avg2-302-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights302-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-302-20,avg2-302-20 FILE=COLVAR302-20 STRIDE=10000 FMT=%16.10f

weights302-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=302 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-302-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights302-25 CLEAR=10000
avg2-302-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights302-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-302-25,avg2-302-25 FILE=COLVAR302-25 STRIDE=10000 FMT=%16.10f

weights302-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=302 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-302-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights302-30 CLEAR=10000
avg2-302-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights302-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-302-30,avg2-302-30 FILE=COLVAR302-30 STRIDE=10000 FMT=%16.10f

weights302-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=302 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-302-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights302-35 CLEAR=10000
avg2-302-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights302-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-302-35,avg2-302-35 FILE=COLVAR302-35 STRIDE=10000 FMT=%16.10f

weights302-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=302 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-302-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights302-40 CLEAR=10000
avg2-302-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights302-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-302-40,avg2-302-40 FILE=COLVAR302-40 STRIDE=10000 FMT=%16.10f

weights302-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=302 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-302-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights302-45 CLEAR=10000
avg2-302-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights302-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-302-45,avg2-302-45 FILE=COLVAR302-45 STRIDE=10000 FMT=%16.10f

weights302-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=302 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-302-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights302-50 CLEAR=10000
avg2-302-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights302-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-302-50,avg2-302-50 FILE=COLVAR302-50 STRIDE=10000 FMT=%16.10f

weights302-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=302 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-302-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights302-55 CLEAR=10000
avg2-302-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights302-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-302-55,avg2-302-55 FILE=COLVAR302-55 STRIDE=10000 FMT=%16.10f

weights302-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=302 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-302-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights302-60 CLEAR=10000
avg2-302-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights302-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-302-60,avg2-302-60 FILE=COLVAR302-60 STRIDE=10000 FMT=%16.10f

weights302-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=302 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-302-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights302-65 CLEAR=10000
avg2-302-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights302-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-302-65,avg2-302-65 FILE=COLVAR302-65 STRIDE=10000 FMT=%16.10f

weights302-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=302 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-302-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights302-70 CLEAR=10000
avg2-302-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights302-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-302-70,avg2-302-70 FILE=COLVAR302-70 STRIDE=10000 FMT=%16.10f

weights302-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=302 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-302-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights302-75 CLEAR=10000
avg2-302-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights302-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-302-75,avg2-302-75 FILE=COLVAR302-75 STRIDE=10000 FMT=%16.10f

weights302-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=302 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-302-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights302-80 CLEAR=10000
avg2-302-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights302-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-302-80,avg2-302-80 FILE=COLVAR302-80 STRIDE=10000 FMT=%16.10f

weights302-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=302 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-302-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights302-85 CLEAR=10000
avg2-302-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights302-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-302-85,avg2-302-85 FILE=COLVAR302-85 STRIDE=10000 FMT=%16.10f

weights302-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=302 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-302-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights302-90 CLEAR=10000
avg2-302-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights302-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-302-90,avg2-302-90 FILE=COLVAR302-90 STRIDE=10000 FMT=%16.10f

weights302-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=302 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-302-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights302-95 CLEAR=10000
avg2-302-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights302-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-302-95,avg2-302-95 FILE=COLVAR302-95 STRIDE=10000 FMT=%16.10f

weights302-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=302 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-302-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights302-100 CLEAR=10000
avg2-302-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights302-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-302-100,avg2-302-100 FILE=COLVAR302-100 STRIDE=10000 FMT=%16.10f

weights304-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=304 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-304-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights304-0 CLEAR=10000
avg2-304-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights304-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-304-0,avg2-304-0 FILE=COLVAR304-0 STRIDE=10000 FMT=%16.10f

weights304-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=304 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-304-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights304-5 CLEAR=10000
avg2-304-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights304-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-304-5,avg2-304-5 FILE=COLVAR304-5 STRIDE=10000 FMT=%16.10f

weights304-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=304 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-304-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights304-10 CLEAR=10000
avg2-304-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights304-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-304-10,avg2-304-10 FILE=COLVAR304-10 STRIDE=10000 FMT=%16.10f

weights304-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=304 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-304-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights304-15 CLEAR=10000
avg2-304-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights304-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-304-15,avg2-304-15 FILE=COLVAR304-15 STRIDE=10000 FMT=%16.10f

weights304-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=304 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-304-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights304-20 CLEAR=10000
avg2-304-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights304-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-304-20,avg2-304-20 FILE=COLVAR304-20 STRIDE=10000 FMT=%16.10f

weights304-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=304 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-304-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights304-25 CLEAR=10000
avg2-304-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights304-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-304-25,avg2-304-25 FILE=COLVAR304-25 STRIDE=10000 FMT=%16.10f

weights304-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=304 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-304-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights304-30 CLEAR=10000
avg2-304-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights304-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-304-30,avg2-304-30 FILE=COLVAR304-30 STRIDE=10000 FMT=%16.10f

weights304-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=304 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-304-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights304-35 CLEAR=10000
avg2-304-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights304-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-304-35,avg2-304-35 FILE=COLVAR304-35 STRIDE=10000 FMT=%16.10f

weights304-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=304 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-304-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights304-40 CLEAR=10000
avg2-304-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights304-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-304-40,avg2-304-40 FILE=COLVAR304-40 STRIDE=10000 FMT=%16.10f

weights304-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=304 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-304-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights304-45 CLEAR=10000
avg2-304-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights304-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-304-45,avg2-304-45 FILE=COLVAR304-45 STRIDE=10000 FMT=%16.10f

weights304-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=304 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-304-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights304-50 CLEAR=10000
avg2-304-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights304-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-304-50,avg2-304-50 FILE=COLVAR304-50 STRIDE=10000 FMT=%16.10f

weights304-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=304 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-304-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights304-55 CLEAR=10000
avg2-304-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights304-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-304-55,avg2-304-55 FILE=COLVAR304-55 STRIDE=10000 FMT=%16.10f

weights304-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=304 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-304-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights304-60 CLEAR=10000
avg2-304-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights304-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-304-60,avg2-304-60 FILE=COLVAR304-60 STRIDE=10000 FMT=%16.10f

weights304-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=304 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-304-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights304-65 CLEAR=10000
avg2-304-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights304-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-304-65,avg2-304-65 FILE=COLVAR304-65 STRIDE=10000 FMT=%16.10f

weights304-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=304 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-304-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights304-70 CLEAR=10000
avg2-304-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights304-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-304-70,avg2-304-70 FILE=COLVAR304-70 STRIDE=10000 FMT=%16.10f

weights304-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=304 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-304-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights304-75 CLEAR=10000
avg2-304-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights304-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-304-75,avg2-304-75 FILE=COLVAR304-75 STRIDE=10000 FMT=%16.10f

weights304-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=304 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-304-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights304-80 CLEAR=10000
avg2-304-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights304-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-304-80,avg2-304-80 FILE=COLVAR304-80 STRIDE=10000 FMT=%16.10f

weights304-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=304 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-304-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights304-85 CLEAR=10000
avg2-304-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights304-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-304-85,avg2-304-85 FILE=COLVAR304-85 STRIDE=10000 FMT=%16.10f

weights304-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=304 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-304-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights304-90 CLEAR=10000
avg2-304-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights304-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-304-90,avg2-304-90 FILE=COLVAR304-90 STRIDE=10000 FMT=%16.10f

weights304-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=304 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-304-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights304-95 CLEAR=10000
avg2-304-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights304-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-304-95,avg2-304-95 FILE=COLVAR304-95 STRIDE=10000 FMT=%16.10f

weights304-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=304 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-304-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights304-100 CLEAR=10000
avg2-304-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights304-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-304-100,avg2-304-100 FILE=COLVAR304-100 STRIDE=10000 FMT=%16.10f

weights306-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=306 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-306-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights306-0 CLEAR=10000
avg2-306-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights306-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-306-0,avg2-306-0 FILE=COLVAR306-0 STRIDE=10000 FMT=%16.10f

weights306-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=306 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-306-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights306-5 CLEAR=10000
avg2-306-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights306-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-306-5,avg2-306-5 FILE=COLVAR306-5 STRIDE=10000 FMT=%16.10f

weights306-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=306 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-306-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights306-10 CLEAR=10000
avg2-306-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights306-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-306-10,avg2-306-10 FILE=COLVAR306-10 STRIDE=10000 FMT=%16.10f

weights306-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=306 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-306-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights306-15 CLEAR=10000
avg2-306-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights306-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-306-15,avg2-306-15 FILE=COLVAR306-15 STRIDE=10000 FMT=%16.10f

weights306-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=306 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-306-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights306-20 CLEAR=10000
avg2-306-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights306-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-306-20,avg2-306-20 FILE=COLVAR306-20 STRIDE=10000 FMT=%16.10f

weights306-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=306 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-306-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights306-25 CLEAR=10000
avg2-306-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights306-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-306-25,avg2-306-25 FILE=COLVAR306-25 STRIDE=10000 FMT=%16.10f

weights306-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=306 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-306-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights306-30 CLEAR=10000
avg2-306-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights306-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-306-30,avg2-306-30 FILE=COLVAR306-30 STRIDE=10000 FMT=%16.10f

weights306-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=306 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-306-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights306-35 CLEAR=10000
avg2-306-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights306-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-306-35,avg2-306-35 FILE=COLVAR306-35 STRIDE=10000 FMT=%16.10f

weights306-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=306 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-306-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights306-40 CLEAR=10000
avg2-306-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights306-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-306-40,avg2-306-40 FILE=COLVAR306-40 STRIDE=10000 FMT=%16.10f

weights306-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=306 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-306-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights306-45 CLEAR=10000
avg2-306-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights306-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-306-45,avg2-306-45 FILE=COLVAR306-45 STRIDE=10000 FMT=%16.10f

weights306-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=306 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-306-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights306-50 CLEAR=10000
avg2-306-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights306-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-306-50,avg2-306-50 FILE=COLVAR306-50 STRIDE=10000 FMT=%16.10f

weights306-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=306 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-306-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights306-55 CLEAR=10000
avg2-306-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights306-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-306-55,avg2-306-55 FILE=COLVAR306-55 STRIDE=10000 FMT=%16.10f

weights306-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=306 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-306-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights306-60 CLEAR=10000
avg2-306-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights306-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-306-60,avg2-306-60 FILE=COLVAR306-60 STRIDE=10000 FMT=%16.10f

weights306-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=306 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-306-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights306-65 CLEAR=10000
avg2-306-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights306-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-306-65,avg2-306-65 FILE=COLVAR306-65 STRIDE=10000 FMT=%16.10f

weights306-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=306 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-306-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights306-70 CLEAR=10000
avg2-306-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights306-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-306-70,avg2-306-70 FILE=COLVAR306-70 STRIDE=10000 FMT=%16.10f

weights306-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=306 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-306-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights306-75 CLEAR=10000
avg2-306-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights306-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-306-75,avg2-306-75 FILE=COLVAR306-75 STRIDE=10000 FMT=%16.10f

weights306-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=306 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-306-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights306-80 CLEAR=10000
avg2-306-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights306-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-306-80,avg2-306-80 FILE=COLVAR306-80 STRIDE=10000 FMT=%16.10f

weights306-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=306 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-306-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights306-85 CLEAR=10000
avg2-306-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights306-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-306-85,avg2-306-85 FILE=COLVAR306-85 STRIDE=10000 FMT=%16.10f

weights306-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=306 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-306-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights306-90 CLEAR=10000
avg2-306-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights306-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-306-90,avg2-306-90 FILE=COLVAR306-90 STRIDE=10000 FMT=%16.10f

weights306-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=306 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-306-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights306-95 CLEAR=10000
avg2-306-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights306-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-306-95,avg2-306-95 FILE=COLVAR306-95 STRIDE=10000 FMT=%16.10f

weights306-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=306 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-306-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights306-100 CLEAR=10000
avg2-306-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights306-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-306-100,avg2-306-100 FILE=COLVAR306-100 STRIDE=10000 FMT=%16.10f

weights308-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=308 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-308-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights308-0 CLEAR=10000
avg2-308-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights308-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-308-0,avg2-308-0 FILE=COLVAR308-0 STRIDE=10000 FMT=%16.10f

weights308-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=308 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-308-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights308-5 CLEAR=10000
avg2-308-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights308-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-308-5,avg2-308-5 FILE=COLVAR308-5 STRIDE=10000 FMT=%16.10f

weights308-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=308 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-308-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights308-10 CLEAR=10000
avg2-308-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights308-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-308-10,avg2-308-10 FILE=COLVAR308-10 STRIDE=10000 FMT=%16.10f

weights308-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=308 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-308-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights308-15 CLEAR=10000
avg2-308-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights308-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-308-15,avg2-308-15 FILE=COLVAR308-15 STRIDE=10000 FMT=%16.10f

weights308-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=308 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-308-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights308-20 CLEAR=10000
avg2-308-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights308-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-308-20,avg2-308-20 FILE=COLVAR308-20 STRIDE=10000 FMT=%16.10f

weights308-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=308 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-308-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights308-25 CLEAR=10000
avg2-308-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights308-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-308-25,avg2-308-25 FILE=COLVAR308-25 STRIDE=10000 FMT=%16.10f

weights308-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=308 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-308-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights308-30 CLEAR=10000
avg2-308-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights308-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-308-30,avg2-308-30 FILE=COLVAR308-30 STRIDE=10000 FMT=%16.10f

weights308-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=308 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-308-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights308-35 CLEAR=10000
avg2-308-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights308-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-308-35,avg2-308-35 FILE=COLVAR308-35 STRIDE=10000 FMT=%16.10f

weights308-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=308 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-308-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights308-40 CLEAR=10000
avg2-308-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights308-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-308-40,avg2-308-40 FILE=COLVAR308-40 STRIDE=10000 FMT=%16.10f

weights308-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=308 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-308-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights308-45 CLEAR=10000
avg2-308-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights308-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-308-45,avg2-308-45 FILE=COLVAR308-45 STRIDE=10000 FMT=%16.10f

weights308-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=308 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-308-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights308-50 CLEAR=10000
avg2-308-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights308-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-308-50,avg2-308-50 FILE=COLVAR308-50 STRIDE=10000 FMT=%16.10f

weights308-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=308 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-308-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights308-55 CLEAR=10000
avg2-308-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights308-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-308-55,avg2-308-55 FILE=COLVAR308-55 STRIDE=10000 FMT=%16.10f

weights308-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=308 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-308-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights308-60 CLEAR=10000
avg2-308-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights308-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-308-60,avg2-308-60 FILE=COLVAR308-60 STRIDE=10000 FMT=%16.10f

weights308-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=308 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-308-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights308-65 CLEAR=10000
avg2-308-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights308-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-308-65,avg2-308-65 FILE=COLVAR308-65 STRIDE=10000 FMT=%16.10f

weights308-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=308 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-308-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights308-70 CLEAR=10000
avg2-308-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights308-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-308-70,avg2-308-70 FILE=COLVAR308-70 STRIDE=10000 FMT=%16.10f

weights308-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=308 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-308-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights308-75 CLEAR=10000
avg2-308-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights308-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-308-75,avg2-308-75 FILE=COLVAR308-75 STRIDE=10000 FMT=%16.10f

weights308-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=308 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-308-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights308-80 CLEAR=10000
avg2-308-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights308-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-308-80,avg2-308-80 FILE=COLVAR308-80 STRIDE=10000 FMT=%16.10f

weights308-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=308 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-308-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights308-85 CLEAR=10000
avg2-308-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights308-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-308-85,avg2-308-85 FILE=COLVAR308-85 STRIDE=10000 FMT=%16.10f

weights308-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=308 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-308-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights308-90 CLEAR=10000
avg2-308-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights308-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-308-90,avg2-308-90 FILE=COLVAR308-90 STRIDE=10000 FMT=%16.10f

weights308-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=308 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-308-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights308-95 CLEAR=10000
avg2-308-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights308-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-308-95,avg2-308-95 FILE=COLVAR308-95 STRIDE=10000 FMT=%16.10f

weights308-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=308 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-308-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights308-100 CLEAR=10000
avg2-308-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights308-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-308-100,avg2-308-100 FILE=COLVAR308-100 STRIDE=10000 FMT=%16.10f

weights310-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=310 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-310-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights310-0 CLEAR=10000
avg2-310-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights310-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-310-0,avg2-310-0 FILE=COLVAR310-0 STRIDE=10000 FMT=%16.10f

weights310-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=310 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-310-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights310-5 CLEAR=10000
avg2-310-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights310-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-310-5,avg2-310-5 FILE=COLVAR310-5 STRIDE=10000 FMT=%16.10f

weights310-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=310 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-310-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights310-10 CLEAR=10000
avg2-310-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights310-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-310-10,avg2-310-10 FILE=COLVAR310-10 STRIDE=10000 FMT=%16.10f

weights310-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=310 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-310-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights310-15 CLEAR=10000
avg2-310-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights310-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-310-15,avg2-310-15 FILE=COLVAR310-15 STRIDE=10000 FMT=%16.10f

weights310-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=310 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-310-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights310-20 CLEAR=10000
avg2-310-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights310-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-310-20,avg2-310-20 FILE=COLVAR310-20 STRIDE=10000 FMT=%16.10f

weights310-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=310 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-310-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights310-25 CLEAR=10000
avg2-310-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights310-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-310-25,avg2-310-25 FILE=COLVAR310-25 STRIDE=10000 FMT=%16.10f

weights310-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=310 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-310-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights310-30 CLEAR=10000
avg2-310-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights310-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-310-30,avg2-310-30 FILE=COLVAR310-30 STRIDE=10000 FMT=%16.10f

weights310-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=310 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-310-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights310-35 CLEAR=10000
avg2-310-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights310-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-310-35,avg2-310-35 FILE=COLVAR310-35 STRIDE=10000 FMT=%16.10f

weights310-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=310 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-310-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights310-40 CLEAR=10000
avg2-310-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights310-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-310-40,avg2-310-40 FILE=COLVAR310-40 STRIDE=10000 FMT=%16.10f

weights310-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=310 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-310-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights310-45 CLEAR=10000
avg2-310-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights310-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-310-45,avg2-310-45 FILE=COLVAR310-45 STRIDE=10000 FMT=%16.10f

weights310-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=310 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-310-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights310-50 CLEAR=10000
avg2-310-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights310-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-310-50,avg2-310-50 FILE=COLVAR310-50 STRIDE=10000 FMT=%16.10f

weights310-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=310 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-310-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights310-55 CLEAR=10000
avg2-310-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights310-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-310-55,avg2-310-55 FILE=COLVAR310-55 STRIDE=10000 FMT=%16.10f

weights310-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=310 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-310-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights310-60 CLEAR=10000
avg2-310-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights310-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-310-60,avg2-310-60 FILE=COLVAR310-60 STRIDE=10000 FMT=%16.10f

weights310-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=310 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-310-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights310-65 CLEAR=10000
avg2-310-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights310-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-310-65,avg2-310-65 FILE=COLVAR310-65 STRIDE=10000 FMT=%16.10f

weights310-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=310 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-310-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights310-70 CLEAR=10000
avg2-310-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights310-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-310-70,avg2-310-70 FILE=COLVAR310-70 STRIDE=10000 FMT=%16.10f

weights310-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=310 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-310-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights310-75 CLEAR=10000
avg2-310-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights310-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-310-75,avg2-310-75 FILE=COLVAR310-75 STRIDE=10000 FMT=%16.10f

weights310-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=310 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-310-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights310-80 CLEAR=10000
avg2-310-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights310-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-310-80,avg2-310-80 FILE=COLVAR310-80 STRIDE=10000 FMT=%16.10f

weights310-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=310 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-310-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights310-85 CLEAR=10000
avg2-310-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights310-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-310-85,avg2-310-85 FILE=COLVAR310-85 STRIDE=10000 FMT=%16.10f

weights310-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=310 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-310-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights310-90 CLEAR=10000
avg2-310-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights310-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-310-90,avg2-310-90 FILE=COLVAR310-90 STRIDE=10000 FMT=%16.10f

weights310-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=310 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-310-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights310-95 CLEAR=10000
avg2-310-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights310-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-310-95,avg2-310-95 FILE=COLVAR310-95 STRIDE=10000 FMT=%16.10f

weights310-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=310 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-310-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights310-100 CLEAR=10000
avg2-310-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights310-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-310-100,avg2-310-100 FILE=COLVAR310-100 STRIDE=10000 FMT=%16.10f

weights312-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=312 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-312-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights312-0 CLEAR=10000
avg2-312-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights312-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-312-0,avg2-312-0 FILE=COLVAR312-0 STRIDE=10000 FMT=%16.10f

weights312-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=312 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-312-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights312-5 CLEAR=10000
avg2-312-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights312-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-312-5,avg2-312-5 FILE=COLVAR312-5 STRIDE=10000 FMT=%16.10f

weights312-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=312 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-312-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights312-10 CLEAR=10000
avg2-312-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights312-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-312-10,avg2-312-10 FILE=COLVAR312-10 STRIDE=10000 FMT=%16.10f

weights312-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=312 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-312-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights312-15 CLEAR=10000
avg2-312-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights312-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-312-15,avg2-312-15 FILE=COLVAR312-15 STRIDE=10000 FMT=%16.10f

weights312-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=312 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-312-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights312-20 CLEAR=10000
avg2-312-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights312-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-312-20,avg2-312-20 FILE=COLVAR312-20 STRIDE=10000 FMT=%16.10f

weights312-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=312 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-312-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights312-25 CLEAR=10000
avg2-312-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights312-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-312-25,avg2-312-25 FILE=COLVAR312-25 STRIDE=10000 FMT=%16.10f

weights312-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=312 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-312-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights312-30 CLEAR=10000
avg2-312-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights312-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-312-30,avg2-312-30 FILE=COLVAR312-30 STRIDE=10000 FMT=%16.10f

weights312-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=312 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-312-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights312-35 CLEAR=10000
avg2-312-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights312-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-312-35,avg2-312-35 FILE=COLVAR312-35 STRIDE=10000 FMT=%16.10f

weights312-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=312 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-312-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights312-40 CLEAR=10000
avg2-312-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights312-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-312-40,avg2-312-40 FILE=COLVAR312-40 STRIDE=10000 FMT=%16.10f

weights312-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=312 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-312-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights312-45 CLEAR=10000
avg2-312-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights312-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-312-45,avg2-312-45 FILE=COLVAR312-45 STRIDE=10000 FMT=%16.10f

weights312-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=312 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-312-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights312-50 CLEAR=10000
avg2-312-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights312-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-312-50,avg2-312-50 FILE=COLVAR312-50 STRIDE=10000 FMT=%16.10f

weights312-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=312 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-312-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights312-55 CLEAR=10000
avg2-312-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights312-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-312-55,avg2-312-55 FILE=COLVAR312-55 STRIDE=10000 FMT=%16.10f

weights312-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=312 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-312-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights312-60 CLEAR=10000
avg2-312-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights312-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-312-60,avg2-312-60 FILE=COLVAR312-60 STRIDE=10000 FMT=%16.10f

weights312-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=312 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-312-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights312-65 CLEAR=10000
avg2-312-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights312-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-312-65,avg2-312-65 FILE=COLVAR312-65 STRIDE=10000 FMT=%16.10f

weights312-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=312 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-312-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights312-70 CLEAR=10000
avg2-312-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights312-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-312-70,avg2-312-70 FILE=COLVAR312-70 STRIDE=10000 FMT=%16.10f

weights312-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=312 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-312-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights312-75 CLEAR=10000
avg2-312-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights312-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-312-75,avg2-312-75 FILE=COLVAR312-75 STRIDE=10000 FMT=%16.10f

weights312-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=312 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-312-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights312-80 CLEAR=10000
avg2-312-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights312-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-312-80,avg2-312-80 FILE=COLVAR312-80 STRIDE=10000 FMT=%16.10f

weights312-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=312 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-312-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights312-85 CLEAR=10000
avg2-312-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights312-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-312-85,avg2-312-85 FILE=COLVAR312-85 STRIDE=10000 FMT=%16.10f

weights312-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=312 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-312-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights312-90 CLEAR=10000
avg2-312-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights312-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-312-90,avg2-312-90 FILE=COLVAR312-90 STRIDE=10000 FMT=%16.10f

weights312-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=312 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-312-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights312-95 CLEAR=10000
avg2-312-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights312-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-312-95,avg2-312-95 FILE=COLVAR312-95 STRIDE=10000 FMT=%16.10f

weights312-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=312 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-312-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights312-100 CLEAR=10000
avg2-312-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights312-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-312-100,avg2-312-100 FILE=COLVAR312-100 STRIDE=10000 FMT=%16.10f

weights314-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=314 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-314-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights314-0 CLEAR=10000
avg2-314-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights314-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-314-0,avg2-314-0 FILE=COLVAR314-0 STRIDE=10000 FMT=%16.10f

weights314-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=314 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-314-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights314-5 CLEAR=10000
avg2-314-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights314-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-314-5,avg2-314-5 FILE=COLVAR314-5 STRIDE=10000 FMT=%16.10f

weights314-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=314 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-314-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights314-10 CLEAR=10000
avg2-314-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights314-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-314-10,avg2-314-10 FILE=COLVAR314-10 STRIDE=10000 FMT=%16.10f

weights314-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=314 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-314-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights314-15 CLEAR=10000
avg2-314-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights314-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-314-15,avg2-314-15 FILE=COLVAR314-15 STRIDE=10000 FMT=%16.10f

weights314-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=314 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-314-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights314-20 CLEAR=10000
avg2-314-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights314-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-314-20,avg2-314-20 FILE=COLVAR314-20 STRIDE=10000 FMT=%16.10f

weights314-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=314 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-314-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights314-25 CLEAR=10000
avg2-314-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights314-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-314-25,avg2-314-25 FILE=COLVAR314-25 STRIDE=10000 FMT=%16.10f

weights314-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=314 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-314-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights314-30 CLEAR=10000
avg2-314-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights314-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-314-30,avg2-314-30 FILE=COLVAR314-30 STRIDE=10000 FMT=%16.10f

weights314-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=314 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-314-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights314-35 CLEAR=10000
avg2-314-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights314-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-314-35,avg2-314-35 FILE=COLVAR314-35 STRIDE=10000 FMT=%16.10f

weights314-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=314 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-314-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights314-40 CLEAR=10000
avg2-314-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights314-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-314-40,avg2-314-40 FILE=COLVAR314-40 STRIDE=10000 FMT=%16.10f

weights314-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=314 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-314-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights314-45 CLEAR=10000
avg2-314-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights314-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-314-45,avg2-314-45 FILE=COLVAR314-45 STRIDE=10000 FMT=%16.10f

weights314-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=314 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-314-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights314-50 CLEAR=10000
avg2-314-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights314-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-314-50,avg2-314-50 FILE=COLVAR314-50 STRIDE=10000 FMT=%16.10f

weights314-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=314 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-314-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights314-55 CLEAR=10000
avg2-314-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights314-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-314-55,avg2-314-55 FILE=COLVAR314-55 STRIDE=10000 FMT=%16.10f

weights314-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=314 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-314-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights314-60 CLEAR=10000
avg2-314-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights314-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-314-60,avg2-314-60 FILE=COLVAR314-60 STRIDE=10000 FMT=%16.10f

weights314-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=314 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-314-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights314-65 CLEAR=10000
avg2-314-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights314-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-314-65,avg2-314-65 FILE=COLVAR314-65 STRIDE=10000 FMT=%16.10f

weights314-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=314 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-314-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights314-70 CLEAR=10000
avg2-314-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights314-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-314-70,avg2-314-70 FILE=COLVAR314-70 STRIDE=10000 FMT=%16.10f

weights314-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=314 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-314-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights314-75 CLEAR=10000
avg2-314-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights314-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-314-75,avg2-314-75 FILE=COLVAR314-75 STRIDE=10000 FMT=%16.10f

weights314-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=314 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-314-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights314-80 CLEAR=10000
avg2-314-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights314-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-314-80,avg2-314-80 FILE=COLVAR314-80 STRIDE=10000 FMT=%16.10f

weights314-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=314 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-314-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights314-85 CLEAR=10000
avg2-314-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights314-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-314-85,avg2-314-85 FILE=COLVAR314-85 STRIDE=10000 FMT=%16.10f

weights314-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=314 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-314-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights314-90 CLEAR=10000
avg2-314-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights314-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-314-90,avg2-314-90 FILE=COLVAR314-90 STRIDE=10000 FMT=%16.10f

weights314-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=314 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-314-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights314-95 CLEAR=10000
avg2-314-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights314-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-314-95,avg2-314-95 FILE=COLVAR314-95 STRIDE=10000 FMT=%16.10f

weights314-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=314 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-314-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights314-100 CLEAR=10000
avg2-314-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights314-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-314-100,avg2-314-100 FILE=COLVAR314-100 STRIDE=10000 FMT=%16.10f

weights316-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=316 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-316-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights316-0 CLEAR=10000
avg2-316-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights316-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-316-0,avg2-316-0 FILE=COLVAR316-0 STRIDE=10000 FMT=%16.10f

weights316-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=316 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-316-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights316-5 CLEAR=10000
avg2-316-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights316-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-316-5,avg2-316-5 FILE=COLVAR316-5 STRIDE=10000 FMT=%16.10f

weights316-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=316 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-316-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights316-10 CLEAR=10000
avg2-316-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights316-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-316-10,avg2-316-10 FILE=COLVAR316-10 STRIDE=10000 FMT=%16.10f

weights316-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=316 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-316-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights316-15 CLEAR=10000
avg2-316-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights316-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-316-15,avg2-316-15 FILE=COLVAR316-15 STRIDE=10000 FMT=%16.10f

weights316-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=316 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-316-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights316-20 CLEAR=10000
avg2-316-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights316-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-316-20,avg2-316-20 FILE=COLVAR316-20 STRIDE=10000 FMT=%16.10f

weights316-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=316 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-316-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights316-25 CLEAR=10000
avg2-316-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights316-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-316-25,avg2-316-25 FILE=COLVAR316-25 STRIDE=10000 FMT=%16.10f

weights316-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=316 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-316-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights316-30 CLEAR=10000
avg2-316-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights316-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-316-30,avg2-316-30 FILE=COLVAR316-30 STRIDE=10000 FMT=%16.10f

weights316-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=316 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-316-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights316-35 CLEAR=10000
avg2-316-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights316-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-316-35,avg2-316-35 FILE=COLVAR316-35 STRIDE=10000 FMT=%16.10f

weights316-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=316 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-316-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights316-40 CLEAR=10000
avg2-316-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights316-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-316-40,avg2-316-40 FILE=COLVAR316-40 STRIDE=10000 FMT=%16.10f

weights316-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=316 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-316-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights316-45 CLEAR=10000
avg2-316-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights316-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-316-45,avg2-316-45 FILE=COLVAR316-45 STRIDE=10000 FMT=%16.10f

weights316-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=316 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-316-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights316-50 CLEAR=10000
avg2-316-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights316-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-316-50,avg2-316-50 FILE=COLVAR316-50 STRIDE=10000 FMT=%16.10f

weights316-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=316 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-316-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights316-55 CLEAR=10000
avg2-316-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights316-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-316-55,avg2-316-55 FILE=COLVAR316-55 STRIDE=10000 FMT=%16.10f

weights316-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=316 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-316-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights316-60 CLEAR=10000
avg2-316-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights316-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-316-60,avg2-316-60 FILE=COLVAR316-60 STRIDE=10000 FMT=%16.10f

weights316-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=316 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-316-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights316-65 CLEAR=10000
avg2-316-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights316-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-316-65,avg2-316-65 FILE=COLVAR316-65 STRIDE=10000 FMT=%16.10f

weights316-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=316 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-316-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights316-70 CLEAR=10000
avg2-316-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights316-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-316-70,avg2-316-70 FILE=COLVAR316-70 STRIDE=10000 FMT=%16.10f

weights316-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=316 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-316-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights316-75 CLEAR=10000
avg2-316-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights316-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-316-75,avg2-316-75 FILE=COLVAR316-75 STRIDE=10000 FMT=%16.10f

weights316-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=316 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-316-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights316-80 CLEAR=10000
avg2-316-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights316-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-316-80,avg2-316-80 FILE=COLVAR316-80 STRIDE=10000 FMT=%16.10f

weights316-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=316 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-316-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights316-85 CLEAR=10000
avg2-316-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights316-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-316-85,avg2-316-85 FILE=COLVAR316-85 STRIDE=10000 FMT=%16.10f

weights316-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=316 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-316-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights316-90 CLEAR=10000
avg2-316-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights316-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-316-90,avg2-316-90 FILE=COLVAR316-90 STRIDE=10000 FMT=%16.10f

weights316-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=316 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-316-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights316-95 CLEAR=10000
avg2-316-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights316-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-316-95,avg2-316-95 FILE=COLVAR316-95 STRIDE=10000 FMT=%16.10f

weights316-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=316 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-316-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights316-100 CLEAR=10000
avg2-316-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights316-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-316-100,avg2-316-100 FILE=COLVAR316-100 STRIDE=10000 FMT=%16.10f

weights318-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=318 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-318-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights318-0 CLEAR=10000
avg2-318-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights318-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-318-0,avg2-318-0 FILE=COLVAR318-0 STRIDE=10000 FMT=%16.10f

weights318-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=318 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-318-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights318-5 CLEAR=10000
avg2-318-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights318-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-318-5,avg2-318-5 FILE=COLVAR318-5 STRIDE=10000 FMT=%16.10f

weights318-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=318 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-318-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights318-10 CLEAR=10000
avg2-318-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights318-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-318-10,avg2-318-10 FILE=COLVAR318-10 STRIDE=10000 FMT=%16.10f

weights318-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=318 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-318-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights318-15 CLEAR=10000
avg2-318-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights318-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-318-15,avg2-318-15 FILE=COLVAR318-15 STRIDE=10000 FMT=%16.10f

weights318-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=318 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-318-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights318-20 CLEAR=10000
avg2-318-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights318-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-318-20,avg2-318-20 FILE=COLVAR318-20 STRIDE=10000 FMT=%16.10f

weights318-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=318 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-318-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights318-25 CLEAR=10000
avg2-318-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights318-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-318-25,avg2-318-25 FILE=COLVAR318-25 STRIDE=10000 FMT=%16.10f

weights318-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=318 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-318-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights318-30 CLEAR=10000
avg2-318-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights318-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-318-30,avg2-318-30 FILE=COLVAR318-30 STRIDE=10000 FMT=%16.10f

weights318-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=318 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-318-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights318-35 CLEAR=10000
avg2-318-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights318-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-318-35,avg2-318-35 FILE=COLVAR318-35 STRIDE=10000 FMT=%16.10f

weights318-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=318 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-318-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights318-40 CLEAR=10000
avg2-318-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights318-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-318-40,avg2-318-40 FILE=COLVAR318-40 STRIDE=10000 FMT=%16.10f

weights318-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=318 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-318-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights318-45 CLEAR=10000
avg2-318-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights318-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-318-45,avg2-318-45 FILE=COLVAR318-45 STRIDE=10000 FMT=%16.10f

weights318-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=318 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-318-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights318-50 CLEAR=10000
avg2-318-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights318-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-318-50,avg2-318-50 FILE=COLVAR318-50 STRIDE=10000 FMT=%16.10f

weights318-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=318 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-318-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights318-55 CLEAR=10000
avg2-318-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights318-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-318-55,avg2-318-55 FILE=COLVAR318-55 STRIDE=10000 FMT=%16.10f

weights318-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=318 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-318-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights318-60 CLEAR=10000
avg2-318-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights318-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-318-60,avg2-318-60 FILE=COLVAR318-60 STRIDE=10000 FMT=%16.10f

weights318-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=318 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-318-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights318-65 CLEAR=10000
avg2-318-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights318-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-318-65,avg2-318-65 FILE=COLVAR318-65 STRIDE=10000 FMT=%16.10f

weights318-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=318 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-318-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights318-70 CLEAR=10000
avg2-318-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights318-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-318-70,avg2-318-70 FILE=COLVAR318-70 STRIDE=10000 FMT=%16.10f

weights318-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=318 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-318-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights318-75 CLEAR=10000
avg2-318-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights318-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-318-75,avg2-318-75 FILE=COLVAR318-75 STRIDE=10000 FMT=%16.10f

weights318-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=318 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-318-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights318-80 CLEAR=10000
avg2-318-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights318-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-318-80,avg2-318-80 FILE=COLVAR318-80 STRIDE=10000 FMT=%16.10f

weights318-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=318 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-318-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights318-85 CLEAR=10000
avg2-318-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights318-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-318-85,avg2-318-85 FILE=COLVAR318-85 STRIDE=10000 FMT=%16.10f

weights318-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=318 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-318-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights318-90 CLEAR=10000
avg2-318-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights318-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-318-90,avg2-318-90 FILE=COLVAR318-90 STRIDE=10000 FMT=%16.10f

weights318-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=318 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-318-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights318-95 CLEAR=10000
avg2-318-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights318-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-318-95,avg2-318-95 FILE=COLVAR318-95 STRIDE=10000 FMT=%16.10f

weights318-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=318 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-318-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights318-100 CLEAR=10000
avg2-318-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights318-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-318-100,avg2-318-100 FILE=COLVAR318-100 STRIDE=10000 FMT=%16.10f

weights320-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=320 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-320-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights320-0 CLEAR=10000
avg2-320-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights320-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-320-0,avg2-320-0 FILE=COLVAR320-0 STRIDE=10000 FMT=%16.10f

weights320-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=320 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-320-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights320-5 CLEAR=10000
avg2-320-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights320-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-320-5,avg2-320-5 FILE=COLVAR320-5 STRIDE=10000 FMT=%16.10f

weights320-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=320 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-320-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights320-10 CLEAR=10000
avg2-320-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights320-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-320-10,avg2-320-10 FILE=COLVAR320-10 STRIDE=10000 FMT=%16.10f

weights320-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=320 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-320-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights320-15 CLEAR=10000
avg2-320-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights320-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-320-15,avg2-320-15 FILE=COLVAR320-15 STRIDE=10000 FMT=%16.10f

weights320-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=320 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-320-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights320-20 CLEAR=10000
avg2-320-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights320-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-320-20,avg2-320-20 FILE=COLVAR320-20 STRIDE=10000 FMT=%16.10f

weights320-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=320 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-320-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights320-25 CLEAR=10000
avg2-320-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights320-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-320-25,avg2-320-25 FILE=COLVAR320-25 STRIDE=10000 FMT=%16.10f

weights320-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=320 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-320-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights320-30 CLEAR=10000
avg2-320-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights320-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-320-30,avg2-320-30 FILE=COLVAR320-30 STRIDE=10000 FMT=%16.10f

weights320-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=320 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-320-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights320-35 CLEAR=10000
avg2-320-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights320-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-320-35,avg2-320-35 FILE=COLVAR320-35 STRIDE=10000 FMT=%16.10f

weights320-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=320 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-320-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights320-40 CLEAR=10000
avg2-320-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights320-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-320-40,avg2-320-40 FILE=COLVAR320-40 STRIDE=10000 FMT=%16.10f

weights320-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=320 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-320-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights320-45 CLEAR=10000
avg2-320-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights320-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-320-45,avg2-320-45 FILE=COLVAR320-45 STRIDE=10000 FMT=%16.10f

weights320-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=320 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-320-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights320-50 CLEAR=10000
avg2-320-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights320-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-320-50,avg2-320-50 FILE=COLVAR320-50 STRIDE=10000 FMT=%16.10f

weights320-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=320 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-320-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights320-55 CLEAR=10000
avg2-320-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights320-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-320-55,avg2-320-55 FILE=COLVAR320-55 STRIDE=10000 FMT=%16.10f

weights320-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=320 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-320-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights320-60 CLEAR=10000
avg2-320-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights320-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-320-60,avg2-320-60 FILE=COLVAR320-60 STRIDE=10000 FMT=%16.10f

weights320-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=320 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-320-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights320-65 CLEAR=10000
avg2-320-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights320-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-320-65,avg2-320-65 FILE=COLVAR320-65 STRIDE=10000 FMT=%16.10f

weights320-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=320 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-320-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights320-70 CLEAR=10000
avg2-320-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights320-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-320-70,avg2-320-70 FILE=COLVAR320-70 STRIDE=10000 FMT=%16.10f

weights320-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=320 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-320-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights320-75 CLEAR=10000
avg2-320-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights320-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-320-75,avg2-320-75 FILE=COLVAR320-75 STRIDE=10000 FMT=%16.10f

weights320-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=320 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-320-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights320-80 CLEAR=10000
avg2-320-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights320-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-320-80,avg2-320-80 FILE=COLVAR320-80 STRIDE=10000 FMT=%16.10f

weights320-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=320 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-320-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights320-85 CLEAR=10000
avg2-320-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights320-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-320-85,avg2-320-85 FILE=COLVAR320-85 STRIDE=10000 FMT=%16.10f

weights320-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=320 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-320-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights320-90 CLEAR=10000
avg2-320-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights320-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-320-90,avg2-320-90 FILE=COLVAR320-90 STRIDE=10000 FMT=%16.10f

weights320-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=320 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-320-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights320-95 CLEAR=10000
avg2-320-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights320-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-320-95,avg2-320-95 FILE=COLVAR320-95 STRIDE=10000 FMT=%16.10f

weights320-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=320 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-320-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights320-100 CLEAR=10000
avg2-320-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights320-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-320-100,avg2-320-100 FILE=COLVAR320-100 STRIDE=10000 FMT=%16.10f

weights322-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=322 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-322-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights322-0 CLEAR=10000
avg2-322-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights322-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-322-0,avg2-322-0 FILE=COLVAR322-0 STRIDE=10000 FMT=%16.10f

weights322-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=322 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-322-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights322-5 CLEAR=10000
avg2-322-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights322-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-322-5,avg2-322-5 FILE=COLVAR322-5 STRIDE=10000 FMT=%16.10f

weights322-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=322 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-322-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights322-10 CLEAR=10000
avg2-322-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights322-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-322-10,avg2-322-10 FILE=COLVAR322-10 STRIDE=10000 FMT=%16.10f

weights322-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=322 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-322-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights322-15 CLEAR=10000
avg2-322-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights322-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-322-15,avg2-322-15 FILE=COLVAR322-15 STRIDE=10000 FMT=%16.10f

weights322-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=322 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-322-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights322-20 CLEAR=10000
avg2-322-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights322-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-322-20,avg2-322-20 FILE=COLVAR322-20 STRIDE=10000 FMT=%16.10f

weights322-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=322 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-322-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights322-25 CLEAR=10000
avg2-322-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights322-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-322-25,avg2-322-25 FILE=COLVAR322-25 STRIDE=10000 FMT=%16.10f

weights322-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=322 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-322-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights322-30 CLEAR=10000
avg2-322-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights322-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-322-30,avg2-322-30 FILE=COLVAR322-30 STRIDE=10000 FMT=%16.10f

weights322-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=322 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-322-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights322-35 CLEAR=10000
avg2-322-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights322-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-322-35,avg2-322-35 FILE=COLVAR322-35 STRIDE=10000 FMT=%16.10f

weights322-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=322 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-322-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights322-40 CLEAR=10000
avg2-322-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights322-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-322-40,avg2-322-40 FILE=COLVAR322-40 STRIDE=10000 FMT=%16.10f

weights322-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=322 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-322-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights322-45 CLEAR=10000
avg2-322-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights322-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-322-45,avg2-322-45 FILE=COLVAR322-45 STRIDE=10000 FMT=%16.10f

weights322-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=322 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-322-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights322-50 CLEAR=10000
avg2-322-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights322-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-322-50,avg2-322-50 FILE=COLVAR322-50 STRIDE=10000 FMT=%16.10f

weights322-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=322 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-322-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights322-55 CLEAR=10000
avg2-322-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights322-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-322-55,avg2-322-55 FILE=COLVAR322-55 STRIDE=10000 FMT=%16.10f

weights322-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=322 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-322-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights322-60 CLEAR=10000
avg2-322-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights322-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-322-60,avg2-322-60 FILE=COLVAR322-60 STRIDE=10000 FMT=%16.10f

weights322-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=322 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-322-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights322-65 CLEAR=10000
avg2-322-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights322-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-322-65,avg2-322-65 FILE=COLVAR322-65 STRIDE=10000 FMT=%16.10f

weights322-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=322 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-322-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights322-70 CLEAR=10000
avg2-322-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights322-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-322-70,avg2-322-70 FILE=COLVAR322-70 STRIDE=10000 FMT=%16.10f

weights322-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=322 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-322-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights322-75 CLEAR=10000
avg2-322-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights322-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-322-75,avg2-322-75 FILE=COLVAR322-75 STRIDE=10000 FMT=%16.10f

weights322-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=322 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-322-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights322-80 CLEAR=10000
avg2-322-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights322-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-322-80,avg2-322-80 FILE=COLVAR322-80 STRIDE=10000 FMT=%16.10f

weights322-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=322 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-322-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights322-85 CLEAR=10000
avg2-322-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights322-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-322-85,avg2-322-85 FILE=COLVAR322-85 STRIDE=10000 FMT=%16.10f

weights322-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=322 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-322-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights322-90 CLEAR=10000
avg2-322-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights322-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-322-90,avg2-322-90 FILE=COLVAR322-90 STRIDE=10000 FMT=%16.10f

weights322-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=322 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-322-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights322-95 CLEAR=10000
avg2-322-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights322-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-322-95,avg2-322-95 FILE=COLVAR322-95 STRIDE=10000 FMT=%16.10f

weights322-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=322 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-322-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights322-100 CLEAR=10000
avg2-322-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights322-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-322-100,avg2-322-100 FILE=COLVAR322-100 STRIDE=10000 FMT=%16.10f

weights324-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=324 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-324-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights324-0 CLEAR=10000
avg2-324-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights324-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-324-0,avg2-324-0 FILE=COLVAR324-0 STRIDE=10000 FMT=%16.10f

weights324-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=324 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-324-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights324-5 CLEAR=10000
avg2-324-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights324-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-324-5,avg2-324-5 FILE=COLVAR324-5 STRIDE=10000 FMT=%16.10f

weights324-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=324 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-324-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights324-10 CLEAR=10000
avg2-324-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights324-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-324-10,avg2-324-10 FILE=COLVAR324-10 STRIDE=10000 FMT=%16.10f

weights324-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=324 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-324-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights324-15 CLEAR=10000
avg2-324-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights324-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-324-15,avg2-324-15 FILE=COLVAR324-15 STRIDE=10000 FMT=%16.10f

weights324-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=324 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-324-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights324-20 CLEAR=10000
avg2-324-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights324-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-324-20,avg2-324-20 FILE=COLVAR324-20 STRIDE=10000 FMT=%16.10f

weights324-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=324 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-324-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights324-25 CLEAR=10000
avg2-324-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights324-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-324-25,avg2-324-25 FILE=COLVAR324-25 STRIDE=10000 FMT=%16.10f

weights324-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=324 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-324-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights324-30 CLEAR=10000
avg2-324-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights324-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-324-30,avg2-324-30 FILE=COLVAR324-30 STRIDE=10000 FMT=%16.10f

weights324-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=324 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-324-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights324-35 CLEAR=10000
avg2-324-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights324-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-324-35,avg2-324-35 FILE=COLVAR324-35 STRIDE=10000 FMT=%16.10f

weights324-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=324 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-324-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights324-40 CLEAR=10000
avg2-324-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights324-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-324-40,avg2-324-40 FILE=COLVAR324-40 STRIDE=10000 FMT=%16.10f

weights324-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=324 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-324-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights324-45 CLEAR=10000
avg2-324-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights324-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-324-45,avg2-324-45 FILE=COLVAR324-45 STRIDE=10000 FMT=%16.10f

weights324-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=324 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-324-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights324-50 CLEAR=10000
avg2-324-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights324-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-324-50,avg2-324-50 FILE=COLVAR324-50 STRIDE=10000 FMT=%16.10f

weights324-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=324 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-324-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights324-55 CLEAR=10000
avg2-324-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights324-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-324-55,avg2-324-55 FILE=COLVAR324-55 STRIDE=10000 FMT=%16.10f

weights324-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=324 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-324-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights324-60 CLEAR=10000
avg2-324-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights324-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-324-60,avg2-324-60 FILE=COLVAR324-60 STRIDE=10000 FMT=%16.10f

weights324-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=324 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-324-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights324-65 CLEAR=10000
avg2-324-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights324-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-324-65,avg2-324-65 FILE=COLVAR324-65 STRIDE=10000 FMT=%16.10f

weights324-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=324 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-324-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights324-70 CLEAR=10000
avg2-324-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights324-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-324-70,avg2-324-70 FILE=COLVAR324-70 STRIDE=10000 FMT=%16.10f

weights324-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=324 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-324-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights324-75 CLEAR=10000
avg2-324-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights324-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-324-75,avg2-324-75 FILE=COLVAR324-75 STRIDE=10000 FMT=%16.10f

weights324-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=324 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-324-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights324-80 CLEAR=10000
avg2-324-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights324-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-324-80,avg2-324-80 FILE=COLVAR324-80 STRIDE=10000 FMT=%16.10f

weights324-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=324 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-324-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights324-85 CLEAR=10000
avg2-324-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights324-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-324-85,avg2-324-85 FILE=COLVAR324-85 STRIDE=10000 FMT=%16.10f

weights324-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=324 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-324-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights324-90 CLEAR=10000
avg2-324-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights324-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-324-90,avg2-324-90 FILE=COLVAR324-90 STRIDE=10000 FMT=%16.10f

weights324-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=324 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-324-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights324-95 CLEAR=10000
avg2-324-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights324-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-324-95,avg2-324-95 FILE=COLVAR324-95 STRIDE=10000 FMT=%16.10f

weights324-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=324 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-324-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights324-100 CLEAR=10000
avg2-324-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights324-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-324-100,avg2-324-100 FILE=COLVAR324-100 STRIDE=10000 FMT=%16.10f

weights326-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=326 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-326-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights326-0 CLEAR=10000
avg2-326-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights326-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-326-0,avg2-326-0 FILE=COLVAR326-0 STRIDE=10000 FMT=%16.10f

weights326-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=326 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-326-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights326-5 CLEAR=10000
avg2-326-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights326-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-326-5,avg2-326-5 FILE=COLVAR326-5 STRIDE=10000 FMT=%16.10f

weights326-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=326 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-326-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights326-10 CLEAR=10000
avg2-326-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights326-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-326-10,avg2-326-10 FILE=COLVAR326-10 STRIDE=10000 FMT=%16.10f

weights326-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=326 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-326-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights326-15 CLEAR=10000
avg2-326-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights326-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-326-15,avg2-326-15 FILE=COLVAR326-15 STRIDE=10000 FMT=%16.10f

weights326-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=326 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-326-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights326-20 CLEAR=10000
avg2-326-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights326-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-326-20,avg2-326-20 FILE=COLVAR326-20 STRIDE=10000 FMT=%16.10f

weights326-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=326 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-326-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights326-25 CLEAR=10000
avg2-326-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights326-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-326-25,avg2-326-25 FILE=COLVAR326-25 STRIDE=10000 FMT=%16.10f

weights326-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=326 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-326-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights326-30 CLEAR=10000
avg2-326-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights326-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-326-30,avg2-326-30 FILE=COLVAR326-30 STRIDE=10000 FMT=%16.10f

weights326-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=326 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-326-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights326-35 CLEAR=10000
avg2-326-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights326-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-326-35,avg2-326-35 FILE=COLVAR326-35 STRIDE=10000 FMT=%16.10f

weights326-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=326 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-326-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights326-40 CLEAR=10000
avg2-326-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights326-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-326-40,avg2-326-40 FILE=COLVAR326-40 STRIDE=10000 FMT=%16.10f

weights326-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=326 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-326-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights326-45 CLEAR=10000
avg2-326-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights326-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-326-45,avg2-326-45 FILE=COLVAR326-45 STRIDE=10000 FMT=%16.10f

weights326-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=326 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-326-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights326-50 CLEAR=10000
avg2-326-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights326-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-326-50,avg2-326-50 FILE=COLVAR326-50 STRIDE=10000 FMT=%16.10f

weights326-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=326 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-326-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights326-55 CLEAR=10000
avg2-326-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights326-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-326-55,avg2-326-55 FILE=COLVAR326-55 STRIDE=10000 FMT=%16.10f

weights326-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=326 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-326-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights326-60 CLEAR=10000
avg2-326-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights326-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-326-60,avg2-326-60 FILE=COLVAR326-60 STRIDE=10000 FMT=%16.10f

weights326-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=326 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-326-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights326-65 CLEAR=10000
avg2-326-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights326-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-326-65,avg2-326-65 FILE=COLVAR326-65 STRIDE=10000 FMT=%16.10f

weights326-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=326 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-326-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights326-70 CLEAR=10000
avg2-326-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights326-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-326-70,avg2-326-70 FILE=COLVAR326-70 STRIDE=10000 FMT=%16.10f

weights326-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=326 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-326-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights326-75 CLEAR=10000
avg2-326-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights326-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-326-75,avg2-326-75 FILE=COLVAR326-75 STRIDE=10000 FMT=%16.10f

weights326-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=326 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-326-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights326-80 CLEAR=10000
avg2-326-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights326-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-326-80,avg2-326-80 FILE=COLVAR326-80 STRIDE=10000 FMT=%16.10f

weights326-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=326 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-326-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights326-85 CLEAR=10000
avg2-326-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights326-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-326-85,avg2-326-85 FILE=COLVAR326-85 STRIDE=10000 FMT=%16.10f

weights326-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=326 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-326-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights326-90 CLEAR=10000
avg2-326-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights326-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-326-90,avg2-326-90 FILE=COLVAR326-90 STRIDE=10000 FMT=%16.10f

weights326-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=326 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-326-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights326-95 CLEAR=10000
avg2-326-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights326-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-326-95,avg2-326-95 FILE=COLVAR326-95 STRIDE=10000 FMT=%16.10f

weights326-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=326 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-326-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights326-100 CLEAR=10000
avg2-326-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights326-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-326-100,avg2-326-100 FILE=COLVAR326-100 STRIDE=10000 FMT=%16.10f

weights328-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=328 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-328-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights328-0 CLEAR=10000
avg2-328-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights328-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-328-0,avg2-328-0 FILE=COLVAR328-0 STRIDE=10000 FMT=%16.10f

weights328-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=328 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-328-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights328-5 CLEAR=10000
avg2-328-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights328-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-328-5,avg2-328-5 FILE=COLVAR328-5 STRIDE=10000 FMT=%16.10f

weights328-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=328 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-328-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights328-10 CLEAR=10000
avg2-328-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights328-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-328-10,avg2-328-10 FILE=COLVAR328-10 STRIDE=10000 FMT=%16.10f

weights328-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=328 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-328-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights328-15 CLEAR=10000
avg2-328-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights328-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-328-15,avg2-328-15 FILE=COLVAR328-15 STRIDE=10000 FMT=%16.10f

weights328-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=328 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-328-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights328-20 CLEAR=10000
avg2-328-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights328-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-328-20,avg2-328-20 FILE=COLVAR328-20 STRIDE=10000 FMT=%16.10f

weights328-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=328 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-328-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights328-25 CLEAR=10000
avg2-328-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights328-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-328-25,avg2-328-25 FILE=COLVAR328-25 STRIDE=10000 FMT=%16.10f

weights328-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=328 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-328-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights328-30 CLEAR=10000
avg2-328-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights328-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-328-30,avg2-328-30 FILE=COLVAR328-30 STRIDE=10000 FMT=%16.10f

weights328-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=328 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-328-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights328-35 CLEAR=10000
avg2-328-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights328-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-328-35,avg2-328-35 FILE=COLVAR328-35 STRIDE=10000 FMT=%16.10f

weights328-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=328 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-328-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights328-40 CLEAR=10000
avg2-328-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights328-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-328-40,avg2-328-40 FILE=COLVAR328-40 STRIDE=10000 FMT=%16.10f

weights328-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=328 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-328-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights328-45 CLEAR=10000
avg2-328-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights328-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-328-45,avg2-328-45 FILE=COLVAR328-45 STRIDE=10000 FMT=%16.10f

weights328-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=328 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-328-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights328-50 CLEAR=10000
avg2-328-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights328-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-328-50,avg2-328-50 FILE=COLVAR328-50 STRIDE=10000 FMT=%16.10f

weights328-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=328 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-328-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights328-55 CLEAR=10000
avg2-328-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights328-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-328-55,avg2-328-55 FILE=COLVAR328-55 STRIDE=10000 FMT=%16.10f

weights328-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=328 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-328-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights328-60 CLEAR=10000
avg2-328-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights328-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-328-60,avg2-328-60 FILE=COLVAR328-60 STRIDE=10000 FMT=%16.10f

weights328-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=328 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-328-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights328-65 CLEAR=10000
avg2-328-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights328-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-328-65,avg2-328-65 FILE=COLVAR328-65 STRIDE=10000 FMT=%16.10f

weights328-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=328 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-328-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights328-70 CLEAR=10000
avg2-328-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights328-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-328-70,avg2-328-70 FILE=COLVAR328-70 STRIDE=10000 FMT=%16.10f

weights328-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=328 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-328-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights328-75 CLEAR=10000
avg2-328-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights328-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-328-75,avg2-328-75 FILE=COLVAR328-75 STRIDE=10000 FMT=%16.10f

weights328-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=328 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-328-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights328-80 CLEAR=10000
avg2-328-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights328-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-328-80,avg2-328-80 FILE=COLVAR328-80 STRIDE=10000 FMT=%16.10f

weights328-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=328 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-328-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights328-85 CLEAR=10000
avg2-328-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights328-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-328-85,avg2-328-85 FILE=COLVAR328-85 STRIDE=10000 FMT=%16.10f

weights328-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=328 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-328-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights328-90 CLEAR=10000
avg2-328-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights328-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-328-90,avg2-328-90 FILE=COLVAR328-90 STRIDE=10000 FMT=%16.10f

weights328-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=328 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-328-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights328-95 CLEAR=10000
avg2-328-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights328-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-328-95,avg2-328-95 FILE=COLVAR328-95 STRIDE=10000 FMT=%16.10f

weights328-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=328 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-328-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights328-100 CLEAR=10000
avg2-328-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights328-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-328-100,avg2-328-100 FILE=COLVAR328-100 STRIDE=10000 FMT=%16.10f

weights330-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=330 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-330-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights330-0 CLEAR=10000
avg2-330-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights330-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-330-0,avg2-330-0 FILE=COLVAR330-0 STRIDE=10000 FMT=%16.10f

weights330-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=330 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-330-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights330-5 CLEAR=10000
avg2-330-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights330-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-330-5,avg2-330-5 FILE=COLVAR330-5 STRIDE=10000 FMT=%16.10f

weights330-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=330 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-330-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights330-10 CLEAR=10000
avg2-330-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights330-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-330-10,avg2-330-10 FILE=COLVAR330-10 STRIDE=10000 FMT=%16.10f

weights330-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=330 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-330-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights330-15 CLEAR=10000
avg2-330-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights330-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-330-15,avg2-330-15 FILE=COLVAR330-15 STRIDE=10000 FMT=%16.10f

weights330-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=330 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-330-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights330-20 CLEAR=10000
avg2-330-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights330-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-330-20,avg2-330-20 FILE=COLVAR330-20 STRIDE=10000 FMT=%16.10f

weights330-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=330 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-330-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights330-25 CLEAR=10000
avg2-330-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights330-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-330-25,avg2-330-25 FILE=COLVAR330-25 STRIDE=10000 FMT=%16.10f

weights330-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=330 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-330-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights330-30 CLEAR=10000
avg2-330-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights330-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-330-30,avg2-330-30 FILE=COLVAR330-30 STRIDE=10000 FMT=%16.10f

weights330-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=330 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-330-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights330-35 CLEAR=10000
avg2-330-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights330-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-330-35,avg2-330-35 FILE=COLVAR330-35 STRIDE=10000 FMT=%16.10f

weights330-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=330 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-330-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights330-40 CLEAR=10000
avg2-330-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights330-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-330-40,avg2-330-40 FILE=COLVAR330-40 STRIDE=10000 FMT=%16.10f

weights330-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=330 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-330-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights330-45 CLEAR=10000
avg2-330-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights330-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-330-45,avg2-330-45 FILE=COLVAR330-45 STRIDE=10000 FMT=%16.10f

weights330-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=330 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-330-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights330-50 CLEAR=10000
avg2-330-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights330-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-330-50,avg2-330-50 FILE=COLVAR330-50 STRIDE=10000 FMT=%16.10f

weights330-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=330 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-330-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights330-55 CLEAR=10000
avg2-330-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights330-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-330-55,avg2-330-55 FILE=COLVAR330-55 STRIDE=10000 FMT=%16.10f

weights330-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=330 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-330-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights330-60 CLEAR=10000
avg2-330-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights330-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-330-60,avg2-330-60 FILE=COLVAR330-60 STRIDE=10000 FMT=%16.10f

weights330-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=330 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-330-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights330-65 CLEAR=10000
avg2-330-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights330-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-330-65,avg2-330-65 FILE=COLVAR330-65 STRIDE=10000 FMT=%16.10f

weights330-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=330 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-330-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights330-70 CLEAR=10000
avg2-330-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights330-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-330-70,avg2-330-70 FILE=COLVAR330-70 STRIDE=10000 FMT=%16.10f

weights330-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=330 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-330-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights330-75 CLEAR=10000
avg2-330-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights330-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-330-75,avg2-330-75 FILE=COLVAR330-75 STRIDE=10000 FMT=%16.10f

weights330-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=330 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-330-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights330-80 CLEAR=10000
avg2-330-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights330-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-330-80,avg2-330-80 FILE=COLVAR330-80 STRIDE=10000 FMT=%16.10f

weights330-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=330 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-330-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights330-85 CLEAR=10000
avg2-330-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights330-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-330-85,avg2-330-85 FILE=COLVAR330-85 STRIDE=10000 FMT=%16.10f

weights330-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=330 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-330-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights330-90 CLEAR=10000
avg2-330-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights330-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-330-90,avg2-330-90 FILE=COLVAR330-90 STRIDE=10000 FMT=%16.10f

weights330-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=330 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-330-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights330-95 CLEAR=10000
avg2-330-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights330-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-330-95,avg2-330-95 FILE=COLVAR330-95 STRIDE=10000 FMT=%16.10f

weights330-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=330 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-330-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights330-100 CLEAR=10000
avg2-330-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights330-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-330-100,avg2-330-100 FILE=COLVAR330-100 STRIDE=10000 FMT=%16.10f

weights332-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=332 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-332-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights332-0 CLEAR=10000
avg2-332-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights332-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-332-0,avg2-332-0 FILE=COLVAR332-0 STRIDE=10000 FMT=%16.10f

weights332-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=332 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-332-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights332-5 CLEAR=10000
avg2-332-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights332-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-332-5,avg2-332-5 FILE=COLVAR332-5 STRIDE=10000 FMT=%16.10f

weights332-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=332 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-332-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights332-10 CLEAR=10000
avg2-332-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights332-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-332-10,avg2-332-10 FILE=COLVAR332-10 STRIDE=10000 FMT=%16.10f

weights332-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=332 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-332-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights332-15 CLEAR=10000
avg2-332-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights332-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-332-15,avg2-332-15 FILE=COLVAR332-15 STRIDE=10000 FMT=%16.10f

weights332-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=332 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-332-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights332-20 CLEAR=10000
avg2-332-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights332-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-332-20,avg2-332-20 FILE=COLVAR332-20 STRIDE=10000 FMT=%16.10f

weights332-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=332 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-332-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights332-25 CLEAR=10000
avg2-332-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights332-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-332-25,avg2-332-25 FILE=COLVAR332-25 STRIDE=10000 FMT=%16.10f

weights332-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=332 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-332-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights332-30 CLEAR=10000
avg2-332-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights332-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-332-30,avg2-332-30 FILE=COLVAR332-30 STRIDE=10000 FMT=%16.10f

weights332-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=332 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-332-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights332-35 CLEAR=10000
avg2-332-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights332-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-332-35,avg2-332-35 FILE=COLVAR332-35 STRIDE=10000 FMT=%16.10f

weights332-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=332 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-332-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights332-40 CLEAR=10000
avg2-332-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights332-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-332-40,avg2-332-40 FILE=COLVAR332-40 STRIDE=10000 FMT=%16.10f

weights332-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=332 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-332-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights332-45 CLEAR=10000
avg2-332-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights332-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-332-45,avg2-332-45 FILE=COLVAR332-45 STRIDE=10000 FMT=%16.10f

weights332-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=332 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-332-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights332-50 CLEAR=10000
avg2-332-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights332-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-332-50,avg2-332-50 FILE=COLVAR332-50 STRIDE=10000 FMT=%16.10f

weights332-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=332 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-332-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights332-55 CLEAR=10000
avg2-332-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights332-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-332-55,avg2-332-55 FILE=COLVAR332-55 STRIDE=10000 FMT=%16.10f

weights332-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=332 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-332-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights332-60 CLEAR=10000
avg2-332-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights332-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-332-60,avg2-332-60 FILE=COLVAR332-60 STRIDE=10000 FMT=%16.10f

weights332-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=332 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-332-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights332-65 CLEAR=10000
avg2-332-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights332-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-332-65,avg2-332-65 FILE=COLVAR332-65 STRIDE=10000 FMT=%16.10f

weights332-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=332 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-332-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights332-70 CLEAR=10000
avg2-332-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights332-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-332-70,avg2-332-70 FILE=COLVAR332-70 STRIDE=10000 FMT=%16.10f

weights332-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=332 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-332-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights332-75 CLEAR=10000
avg2-332-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights332-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-332-75,avg2-332-75 FILE=COLVAR332-75 STRIDE=10000 FMT=%16.10f

weights332-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=332 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-332-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights332-80 CLEAR=10000
avg2-332-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights332-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-332-80,avg2-332-80 FILE=COLVAR332-80 STRIDE=10000 FMT=%16.10f

weights332-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=332 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-332-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights332-85 CLEAR=10000
avg2-332-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights332-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-332-85,avg2-332-85 FILE=COLVAR332-85 STRIDE=10000 FMT=%16.10f

weights332-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=332 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-332-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights332-90 CLEAR=10000
avg2-332-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights332-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-332-90,avg2-332-90 FILE=COLVAR332-90 STRIDE=10000 FMT=%16.10f

weights332-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=332 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-332-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights332-95 CLEAR=10000
avg2-332-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights332-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-332-95,avg2-332-95 FILE=COLVAR332-95 STRIDE=10000 FMT=%16.10f

weights332-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=332 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-332-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights332-100 CLEAR=10000
avg2-332-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights332-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-332-100,avg2-332-100 FILE=COLVAR332-100 STRIDE=10000 FMT=%16.10f

weights334-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=334 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-334-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights334-0 CLEAR=10000
avg2-334-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights334-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-334-0,avg2-334-0 FILE=COLVAR334-0 STRIDE=10000 FMT=%16.10f

weights334-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=334 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-334-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights334-5 CLEAR=10000
avg2-334-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights334-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-334-5,avg2-334-5 FILE=COLVAR334-5 STRIDE=10000 FMT=%16.10f

weights334-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=334 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-334-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights334-10 CLEAR=10000
avg2-334-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights334-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-334-10,avg2-334-10 FILE=COLVAR334-10 STRIDE=10000 FMT=%16.10f

weights334-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=334 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-334-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights334-15 CLEAR=10000
avg2-334-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights334-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-334-15,avg2-334-15 FILE=COLVAR334-15 STRIDE=10000 FMT=%16.10f

weights334-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=334 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-334-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights334-20 CLEAR=10000
avg2-334-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights334-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-334-20,avg2-334-20 FILE=COLVAR334-20 STRIDE=10000 FMT=%16.10f

weights334-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=334 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-334-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights334-25 CLEAR=10000
avg2-334-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights334-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-334-25,avg2-334-25 FILE=COLVAR334-25 STRIDE=10000 FMT=%16.10f

weights334-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=334 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-334-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights334-30 CLEAR=10000
avg2-334-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights334-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-334-30,avg2-334-30 FILE=COLVAR334-30 STRIDE=10000 FMT=%16.10f

weights334-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=334 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-334-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights334-35 CLEAR=10000
avg2-334-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights334-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-334-35,avg2-334-35 FILE=COLVAR334-35 STRIDE=10000 FMT=%16.10f

weights334-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=334 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-334-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights334-40 CLEAR=10000
avg2-334-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights334-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-334-40,avg2-334-40 FILE=COLVAR334-40 STRIDE=10000 FMT=%16.10f

weights334-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=334 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-334-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights334-45 CLEAR=10000
avg2-334-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights334-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-334-45,avg2-334-45 FILE=COLVAR334-45 STRIDE=10000 FMT=%16.10f

weights334-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=334 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-334-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights334-50 CLEAR=10000
avg2-334-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights334-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-334-50,avg2-334-50 FILE=COLVAR334-50 STRIDE=10000 FMT=%16.10f

weights334-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=334 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-334-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights334-55 CLEAR=10000
avg2-334-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights334-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-334-55,avg2-334-55 FILE=COLVAR334-55 STRIDE=10000 FMT=%16.10f

weights334-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=334 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-334-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights334-60 CLEAR=10000
avg2-334-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights334-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-334-60,avg2-334-60 FILE=COLVAR334-60 STRIDE=10000 FMT=%16.10f

weights334-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=334 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-334-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights334-65 CLEAR=10000
avg2-334-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights334-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-334-65,avg2-334-65 FILE=COLVAR334-65 STRIDE=10000 FMT=%16.10f

weights334-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=334 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-334-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights334-70 CLEAR=10000
avg2-334-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights334-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-334-70,avg2-334-70 FILE=COLVAR334-70 STRIDE=10000 FMT=%16.10f

weights334-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=334 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-334-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights334-75 CLEAR=10000
avg2-334-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights334-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-334-75,avg2-334-75 FILE=COLVAR334-75 STRIDE=10000 FMT=%16.10f

weights334-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=334 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-334-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights334-80 CLEAR=10000
avg2-334-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights334-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-334-80,avg2-334-80 FILE=COLVAR334-80 STRIDE=10000 FMT=%16.10f

weights334-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=334 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-334-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights334-85 CLEAR=10000
avg2-334-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights334-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-334-85,avg2-334-85 FILE=COLVAR334-85 STRIDE=10000 FMT=%16.10f

weights334-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=334 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-334-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights334-90 CLEAR=10000
avg2-334-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights334-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-334-90,avg2-334-90 FILE=COLVAR334-90 STRIDE=10000 FMT=%16.10f

weights334-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=334 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-334-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights334-95 CLEAR=10000
avg2-334-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights334-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-334-95,avg2-334-95 FILE=COLVAR334-95 STRIDE=10000 FMT=%16.10f

weights334-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=334 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-334-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights334-100 CLEAR=10000
avg2-334-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights334-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-334-100,avg2-334-100 FILE=COLVAR334-100 STRIDE=10000 FMT=%16.10f

weights336-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=336 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-336-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights336-0 CLEAR=10000
avg2-336-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights336-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-336-0,avg2-336-0 FILE=COLVAR336-0 STRIDE=10000 FMT=%16.10f

weights336-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=336 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-336-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights336-5 CLEAR=10000
avg2-336-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights336-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-336-5,avg2-336-5 FILE=COLVAR336-5 STRIDE=10000 FMT=%16.10f

weights336-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=336 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-336-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights336-10 CLEAR=10000
avg2-336-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights336-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-336-10,avg2-336-10 FILE=COLVAR336-10 STRIDE=10000 FMT=%16.10f

weights336-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=336 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-336-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights336-15 CLEAR=10000
avg2-336-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights336-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-336-15,avg2-336-15 FILE=COLVAR336-15 STRIDE=10000 FMT=%16.10f

weights336-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=336 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-336-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights336-20 CLEAR=10000
avg2-336-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights336-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-336-20,avg2-336-20 FILE=COLVAR336-20 STRIDE=10000 FMT=%16.10f

weights336-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=336 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-336-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights336-25 CLEAR=10000
avg2-336-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights336-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-336-25,avg2-336-25 FILE=COLVAR336-25 STRIDE=10000 FMT=%16.10f

weights336-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=336 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-336-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights336-30 CLEAR=10000
avg2-336-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights336-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-336-30,avg2-336-30 FILE=COLVAR336-30 STRIDE=10000 FMT=%16.10f

weights336-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=336 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-336-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights336-35 CLEAR=10000
avg2-336-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights336-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-336-35,avg2-336-35 FILE=COLVAR336-35 STRIDE=10000 FMT=%16.10f

weights336-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=336 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-336-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights336-40 CLEAR=10000
avg2-336-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights336-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-336-40,avg2-336-40 FILE=COLVAR336-40 STRIDE=10000 FMT=%16.10f

weights336-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=336 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-336-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights336-45 CLEAR=10000
avg2-336-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights336-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-336-45,avg2-336-45 FILE=COLVAR336-45 STRIDE=10000 FMT=%16.10f

weights336-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=336 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-336-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights336-50 CLEAR=10000
avg2-336-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights336-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-336-50,avg2-336-50 FILE=COLVAR336-50 STRIDE=10000 FMT=%16.10f

weights336-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=336 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-336-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights336-55 CLEAR=10000
avg2-336-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights336-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-336-55,avg2-336-55 FILE=COLVAR336-55 STRIDE=10000 FMT=%16.10f

weights336-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=336 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-336-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights336-60 CLEAR=10000
avg2-336-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights336-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-336-60,avg2-336-60 FILE=COLVAR336-60 STRIDE=10000 FMT=%16.10f

weights336-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=336 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-336-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights336-65 CLEAR=10000
avg2-336-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights336-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-336-65,avg2-336-65 FILE=COLVAR336-65 STRIDE=10000 FMT=%16.10f

weights336-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=336 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-336-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights336-70 CLEAR=10000
avg2-336-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights336-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-336-70,avg2-336-70 FILE=COLVAR336-70 STRIDE=10000 FMT=%16.10f

weights336-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=336 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-336-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights336-75 CLEAR=10000
avg2-336-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights336-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-336-75,avg2-336-75 FILE=COLVAR336-75 STRIDE=10000 FMT=%16.10f

weights336-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=336 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-336-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights336-80 CLEAR=10000
avg2-336-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights336-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-336-80,avg2-336-80 FILE=COLVAR336-80 STRIDE=10000 FMT=%16.10f

weights336-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=336 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-336-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights336-85 CLEAR=10000
avg2-336-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights336-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-336-85,avg2-336-85 FILE=COLVAR336-85 STRIDE=10000 FMT=%16.10f

weights336-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=336 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-336-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights336-90 CLEAR=10000
avg2-336-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights336-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-336-90,avg2-336-90 FILE=COLVAR336-90 STRIDE=10000 FMT=%16.10f

weights336-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=336 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-336-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights336-95 CLEAR=10000
avg2-336-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights336-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-336-95,avg2-336-95 FILE=COLVAR336-95 STRIDE=10000 FMT=%16.10f

weights336-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=336 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-336-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights336-100 CLEAR=10000
avg2-336-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights336-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-336-100,avg2-336-100 FILE=COLVAR336-100 STRIDE=10000 FMT=%16.10f

weights338-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=338 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-338-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights338-0 CLEAR=10000
avg2-338-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights338-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-338-0,avg2-338-0 FILE=COLVAR338-0 STRIDE=10000 FMT=%16.10f

weights338-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=338 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-338-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights338-5 CLEAR=10000
avg2-338-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights338-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-338-5,avg2-338-5 FILE=COLVAR338-5 STRIDE=10000 FMT=%16.10f

weights338-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=338 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-338-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights338-10 CLEAR=10000
avg2-338-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights338-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-338-10,avg2-338-10 FILE=COLVAR338-10 STRIDE=10000 FMT=%16.10f

weights338-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=338 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-338-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights338-15 CLEAR=10000
avg2-338-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights338-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-338-15,avg2-338-15 FILE=COLVAR338-15 STRIDE=10000 FMT=%16.10f

weights338-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=338 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-338-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights338-20 CLEAR=10000
avg2-338-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights338-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-338-20,avg2-338-20 FILE=COLVAR338-20 STRIDE=10000 FMT=%16.10f

weights338-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=338 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-338-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights338-25 CLEAR=10000
avg2-338-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights338-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-338-25,avg2-338-25 FILE=COLVAR338-25 STRIDE=10000 FMT=%16.10f

weights338-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=338 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-338-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights338-30 CLEAR=10000
avg2-338-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights338-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-338-30,avg2-338-30 FILE=COLVAR338-30 STRIDE=10000 FMT=%16.10f

weights338-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=338 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-338-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights338-35 CLEAR=10000
avg2-338-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights338-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-338-35,avg2-338-35 FILE=COLVAR338-35 STRIDE=10000 FMT=%16.10f

weights338-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=338 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-338-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights338-40 CLEAR=10000
avg2-338-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights338-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-338-40,avg2-338-40 FILE=COLVAR338-40 STRIDE=10000 FMT=%16.10f

weights338-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=338 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-338-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights338-45 CLEAR=10000
avg2-338-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights338-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-338-45,avg2-338-45 FILE=COLVAR338-45 STRIDE=10000 FMT=%16.10f

weights338-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=338 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-338-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights338-50 CLEAR=10000
avg2-338-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights338-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-338-50,avg2-338-50 FILE=COLVAR338-50 STRIDE=10000 FMT=%16.10f

weights338-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=338 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-338-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights338-55 CLEAR=10000
avg2-338-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights338-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-338-55,avg2-338-55 FILE=COLVAR338-55 STRIDE=10000 FMT=%16.10f

weights338-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=338 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-338-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights338-60 CLEAR=10000
avg2-338-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights338-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-338-60,avg2-338-60 FILE=COLVAR338-60 STRIDE=10000 FMT=%16.10f

weights338-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=338 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-338-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights338-65 CLEAR=10000
avg2-338-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights338-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-338-65,avg2-338-65 FILE=COLVAR338-65 STRIDE=10000 FMT=%16.10f

weights338-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=338 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-338-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights338-70 CLEAR=10000
avg2-338-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights338-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-338-70,avg2-338-70 FILE=COLVAR338-70 STRIDE=10000 FMT=%16.10f

weights338-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=338 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-338-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights338-75 CLEAR=10000
avg2-338-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights338-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-338-75,avg2-338-75 FILE=COLVAR338-75 STRIDE=10000 FMT=%16.10f

weights338-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=338 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-338-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights338-80 CLEAR=10000
avg2-338-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights338-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-338-80,avg2-338-80 FILE=COLVAR338-80 STRIDE=10000 FMT=%16.10f

weights338-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=338 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-338-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights338-85 CLEAR=10000
avg2-338-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights338-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-338-85,avg2-338-85 FILE=COLVAR338-85 STRIDE=10000 FMT=%16.10f

weights338-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=338 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-338-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights338-90 CLEAR=10000
avg2-338-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights338-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-338-90,avg2-338-90 FILE=COLVAR338-90 STRIDE=10000 FMT=%16.10f

weights338-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=338 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-338-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights338-95 CLEAR=10000
avg2-338-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights338-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-338-95,avg2-338-95 FILE=COLVAR338-95 STRIDE=10000 FMT=%16.10f

weights338-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=338 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-338-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights338-100 CLEAR=10000
avg2-338-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights338-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-338-100,avg2-338-100 FILE=COLVAR338-100 STRIDE=10000 FMT=%16.10f

weights340-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=340 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-340-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights340-0 CLEAR=10000
avg2-340-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights340-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-340-0,avg2-340-0 FILE=COLVAR340-0 STRIDE=10000 FMT=%16.10f

weights340-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=340 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-340-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights340-5 CLEAR=10000
avg2-340-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights340-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-340-5,avg2-340-5 FILE=COLVAR340-5 STRIDE=10000 FMT=%16.10f

weights340-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=340 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-340-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights340-10 CLEAR=10000
avg2-340-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights340-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-340-10,avg2-340-10 FILE=COLVAR340-10 STRIDE=10000 FMT=%16.10f

weights340-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=340 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-340-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights340-15 CLEAR=10000
avg2-340-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights340-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-340-15,avg2-340-15 FILE=COLVAR340-15 STRIDE=10000 FMT=%16.10f

weights340-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=340 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-340-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights340-20 CLEAR=10000
avg2-340-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights340-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-340-20,avg2-340-20 FILE=COLVAR340-20 STRIDE=10000 FMT=%16.10f

weights340-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=340 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-340-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights340-25 CLEAR=10000
avg2-340-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights340-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-340-25,avg2-340-25 FILE=COLVAR340-25 STRIDE=10000 FMT=%16.10f

weights340-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=340 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-340-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights340-30 CLEAR=10000
avg2-340-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights340-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-340-30,avg2-340-30 FILE=COLVAR340-30 STRIDE=10000 FMT=%16.10f

weights340-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=340 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-340-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights340-35 CLEAR=10000
avg2-340-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights340-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-340-35,avg2-340-35 FILE=COLVAR340-35 STRIDE=10000 FMT=%16.10f

weights340-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=340 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-340-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights340-40 CLEAR=10000
avg2-340-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights340-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-340-40,avg2-340-40 FILE=COLVAR340-40 STRIDE=10000 FMT=%16.10f

weights340-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=340 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-340-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights340-45 CLEAR=10000
avg2-340-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights340-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-340-45,avg2-340-45 FILE=COLVAR340-45 STRIDE=10000 FMT=%16.10f

weights340-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=340 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-340-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights340-50 CLEAR=10000
avg2-340-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights340-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-340-50,avg2-340-50 FILE=COLVAR340-50 STRIDE=10000 FMT=%16.10f

weights340-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=340 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-340-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights340-55 CLEAR=10000
avg2-340-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights340-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-340-55,avg2-340-55 FILE=COLVAR340-55 STRIDE=10000 FMT=%16.10f

weights340-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=340 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-340-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights340-60 CLEAR=10000
avg2-340-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights340-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-340-60,avg2-340-60 FILE=COLVAR340-60 STRIDE=10000 FMT=%16.10f

weights340-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=340 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-340-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights340-65 CLEAR=10000
avg2-340-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights340-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-340-65,avg2-340-65 FILE=COLVAR340-65 STRIDE=10000 FMT=%16.10f

weights340-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=340 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-340-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights340-70 CLEAR=10000
avg2-340-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights340-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-340-70,avg2-340-70 FILE=COLVAR340-70 STRIDE=10000 FMT=%16.10f

weights340-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=340 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-340-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights340-75 CLEAR=10000
avg2-340-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights340-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-340-75,avg2-340-75 FILE=COLVAR340-75 STRIDE=10000 FMT=%16.10f

weights340-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=340 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-340-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights340-80 CLEAR=10000
avg2-340-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights340-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-340-80,avg2-340-80 FILE=COLVAR340-80 STRIDE=10000 FMT=%16.10f

weights340-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=340 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-340-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights340-85 CLEAR=10000
avg2-340-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights340-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-340-85,avg2-340-85 FILE=COLVAR340-85 STRIDE=10000 FMT=%16.10f

weights340-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=340 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-340-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights340-90 CLEAR=10000
avg2-340-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights340-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-340-90,avg2-340-90 FILE=COLVAR340-90 STRIDE=10000 FMT=%16.10f

weights340-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=340 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-340-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights340-95 CLEAR=10000
avg2-340-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights340-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-340-95,avg2-340-95 FILE=COLVAR340-95 STRIDE=10000 FMT=%16.10f

weights340-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=340 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-340-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights340-100 CLEAR=10000
avg2-340-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights340-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-340-100,avg2-340-100 FILE=COLVAR340-100 STRIDE=10000 FMT=%16.10f

weights342-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=342 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-342-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights342-0 CLEAR=10000
avg2-342-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights342-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-342-0,avg2-342-0 FILE=COLVAR342-0 STRIDE=10000 FMT=%16.10f

weights342-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=342 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-342-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights342-5 CLEAR=10000
avg2-342-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights342-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-342-5,avg2-342-5 FILE=COLVAR342-5 STRIDE=10000 FMT=%16.10f

weights342-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=342 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-342-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights342-10 CLEAR=10000
avg2-342-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights342-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-342-10,avg2-342-10 FILE=COLVAR342-10 STRIDE=10000 FMT=%16.10f

weights342-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=342 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-342-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights342-15 CLEAR=10000
avg2-342-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights342-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-342-15,avg2-342-15 FILE=COLVAR342-15 STRIDE=10000 FMT=%16.10f

weights342-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=342 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-342-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights342-20 CLEAR=10000
avg2-342-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights342-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-342-20,avg2-342-20 FILE=COLVAR342-20 STRIDE=10000 FMT=%16.10f

weights342-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=342 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-342-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights342-25 CLEAR=10000
avg2-342-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights342-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-342-25,avg2-342-25 FILE=COLVAR342-25 STRIDE=10000 FMT=%16.10f

weights342-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=342 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-342-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights342-30 CLEAR=10000
avg2-342-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights342-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-342-30,avg2-342-30 FILE=COLVAR342-30 STRIDE=10000 FMT=%16.10f

weights342-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=342 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-342-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights342-35 CLEAR=10000
avg2-342-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights342-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-342-35,avg2-342-35 FILE=COLVAR342-35 STRIDE=10000 FMT=%16.10f

weights342-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=342 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-342-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights342-40 CLEAR=10000
avg2-342-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights342-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-342-40,avg2-342-40 FILE=COLVAR342-40 STRIDE=10000 FMT=%16.10f

weights342-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=342 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-342-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights342-45 CLEAR=10000
avg2-342-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights342-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-342-45,avg2-342-45 FILE=COLVAR342-45 STRIDE=10000 FMT=%16.10f

weights342-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=342 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-342-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights342-50 CLEAR=10000
avg2-342-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights342-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-342-50,avg2-342-50 FILE=COLVAR342-50 STRIDE=10000 FMT=%16.10f

weights342-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=342 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-342-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights342-55 CLEAR=10000
avg2-342-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights342-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-342-55,avg2-342-55 FILE=COLVAR342-55 STRIDE=10000 FMT=%16.10f

weights342-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=342 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-342-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights342-60 CLEAR=10000
avg2-342-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights342-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-342-60,avg2-342-60 FILE=COLVAR342-60 STRIDE=10000 FMT=%16.10f

weights342-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=342 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-342-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights342-65 CLEAR=10000
avg2-342-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights342-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-342-65,avg2-342-65 FILE=COLVAR342-65 STRIDE=10000 FMT=%16.10f

weights342-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=342 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-342-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights342-70 CLEAR=10000
avg2-342-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights342-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-342-70,avg2-342-70 FILE=COLVAR342-70 STRIDE=10000 FMT=%16.10f

weights342-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=342 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-342-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights342-75 CLEAR=10000
avg2-342-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights342-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-342-75,avg2-342-75 FILE=COLVAR342-75 STRIDE=10000 FMT=%16.10f

weights342-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=342 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-342-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights342-80 CLEAR=10000
avg2-342-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights342-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-342-80,avg2-342-80 FILE=COLVAR342-80 STRIDE=10000 FMT=%16.10f

weights342-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=342 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-342-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights342-85 CLEAR=10000
avg2-342-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights342-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-342-85,avg2-342-85 FILE=COLVAR342-85 STRIDE=10000 FMT=%16.10f

weights342-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=342 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-342-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights342-90 CLEAR=10000
avg2-342-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights342-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-342-90,avg2-342-90 FILE=COLVAR342-90 STRIDE=10000 FMT=%16.10f

weights342-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=342 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-342-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights342-95 CLEAR=10000
avg2-342-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights342-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-342-95,avg2-342-95 FILE=COLVAR342-95 STRIDE=10000 FMT=%16.10f

weights342-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=342 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-342-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights342-100 CLEAR=10000
avg2-342-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights342-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-342-100,avg2-342-100 FILE=COLVAR342-100 STRIDE=10000 FMT=%16.10f

weights344-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=344 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-344-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights344-0 CLEAR=10000
avg2-344-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights344-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-344-0,avg2-344-0 FILE=COLVAR344-0 STRIDE=10000 FMT=%16.10f

weights344-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=344 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-344-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights344-5 CLEAR=10000
avg2-344-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights344-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-344-5,avg2-344-5 FILE=COLVAR344-5 STRIDE=10000 FMT=%16.10f

weights344-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=344 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-344-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights344-10 CLEAR=10000
avg2-344-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights344-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-344-10,avg2-344-10 FILE=COLVAR344-10 STRIDE=10000 FMT=%16.10f

weights344-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=344 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-344-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights344-15 CLEAR=10000
avg2-344-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights344-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-344-15,avg2-344-15 FILE=COLVAR344-15 STRIDE=10000 FMT=%16.10f

weights344-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=344 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-344-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights344-20 CLEAR=10000
avg2-344-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights344-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-344-20,avg2-344-20 FILE=COLVAR344-20 STRIDE=10000 FMT=%16.10f

weights344-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=344 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-344-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights344-25 CLEAR=10000
avg2-344-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights344-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-344-25,avg2-344-25 FILE=COLVAR344-25 STRIDE=10000 FMT=%16.10f

weights344-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=344 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-344-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights344-30 CLEAR=10000
avg2-344-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights344-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-344-30,avg2-344-30 FILE=COLVAR344-30 STRIDE=10000 FMT=%16.10f

weights344-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=344 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-344-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights344-35 CLEAR=10000
avg2-344-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights344-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-344-35,avg2-344-35 FILE=COLVAR344-35 STRIDE=10000 FMT=%16.10f

weights344-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=344 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-344-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights344-40 CLEAR=10000
avg2-344-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights344-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-344-40,avg2-344-40 FILE=COLVAR344-40 STRIDE=10000 FMT=%16.10f

weights344-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=344 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-344-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights344-45 CLEAR=10000
avg2-344-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights344-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-344-45,avg2-344-45 FILE=COLVAR344-45 STRIDE=10000 FMT=%16.10f

weights344-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=344 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-344-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights344-50 CLEAR=10000
avg2-344-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights344-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-344-50,avg2-344-50 FILE=COLVAR344-50 STRIDE=10000 FMT=%16.10f

weights344-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=344 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-344-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights344-55 CLEAR=10000
avg2-344-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights344-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-344-55,avg2-344-55 FILE=COLVAR344-55 STRIDE=10000 FMT=%16.10f

weights344-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=344 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-344-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights344-60 CLEAR=10000
avg2-344-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights344-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-344-60,avg2-344-60 FILE=COLVAR344-60 STRIDE=10000 FMT=%16.10f

weights344-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=344 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-344-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights344-65 CLEAR=10000
avg2-344-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights344-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-344-65,avg2-344-65 FILE=COLVAR344-65 STRIDE=10000 FMT=%16.10f

weights344-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=344 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-344-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights344-70 CLEAR=10000
avg2-344-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights344-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-344-70,avg2-344-70 FILE=COLVAR344-70 STRIDE=10000 FMT=%16.10f

weights344-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=344 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-344-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights344-75 CLEAR=10000
avg2-344-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights344-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-344-75,avg2-344-75 FILE=COLVAR344-75 STRIDE=10000 FMT=%16.10f

weights344-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=344 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-344-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights344-80 CLEAR=10000
avg2-344-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights344-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-344-80,avg2-344-80 FILE=COLVAR344-80 STRIDE=10000 FMT=%16.10f

weights344-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=344 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-344-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights344-85 CLEAR=10000
avg2-344-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights344-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-344-85,avg2-344-85 FILE=COLVAR344-85 STRIDE=10000 FMT=%16.10f

weights344-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=344 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-344-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights344-90 CLEAR=10000
avg2-344-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights344-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-344-90,avg2-344-90 FILE=COLVAR344-90 STRIDE=10000 FMT=%16.10f

weights344-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=344 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-344-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights344-95 CLEAR=10000
avg2-344-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights344-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-344-95,avg2-344-95 FILE=COLVAR344-95 STRIDE=10000 FMT=%16.10f

weights344-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=344 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-344-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights344-100 CLEAR=10000
avg2-344-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights344-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-344-100,avg2-344-100 FILE=COLVAR344-100 STRIDE=10000 FMT=%16.10f

weights346-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=346 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-346-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights346-0 CLEAR=10000
avg2-346-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights346-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-346-0,avg2-346-0 FILE=COLVAR346-0 STRIDE=10000 FMT=%16.10f

weights346-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=346 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-346-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights346-5 CLEAR=10000
avg2-346-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights346-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-346-5,avg2-346-5 FILE=COLVAR346-5 STRIDE=10000 FMT=%16.10f

weights346-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=346 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-346-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights346-10 CLEAR=10000
avg2-346-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights346-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-346-10,avg2-346-10 FILE=COLVAR346-10 STRIDE=10000 FMT=%16.10f

weights346-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=346 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-346-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights346-15 CLEAR=10000
avg2-346-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights346-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-346-15,avg2-346-15 FILE=COLVAR346-15 STRIDE=10000 FMT=%16.10f

weights346-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=346 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-346-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights346-20 CLEAR=10000
avg2-346-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights346-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-346-20,avg2-346-20 FILE=COLVAR346-20 STRIDE=10000 FMT=%16.10f

weights346-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=346 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-346-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights346-25 CLEAR=10000
avg2-346-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights346-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-346-25,avg2-346-25 FILE=COLVAR346-25 STRIDE=10000 FMT=%16.10f

weights346-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=346 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-346-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights346-30 CLEAR=10000
avg2-346-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights346-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-346-30,avg2-346-30 FILE=COLVAR346-30 STRIDE=10000 FMT=%16.10f

weights346-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=346 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-346-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights346-35 CLEAR=10000
avg2-346-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights346-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-346-35,avg2-346-35 FILE=COLVAR346-35 STRIDE=10000 FMT=%16.10f

weights346-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=346 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-346-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights346-40 CLEAR=10000
avg2-346-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights346-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-346-40,avg2-346-40 FILE=COLVAR346-40 STRIDE=10000 FMT=%16.10f

weights346-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=346 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-346-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights346-45 CLEAR=10000
avg2-346-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights346-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-346-45,avg2-346-45 FILE=COLVAR346-45 STRIDE=10000 FMT=%16.10f

weights346-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=346 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-346-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights346-50 CLEAR=10000
avg2-346-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights346-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-346-50,avg2-346-50 FILE=COLVAR346-50 STRIDE=10000 FMT=%16.10f

weights346-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=346 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-346-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights346-55 CLEAR=10000
avg2-346-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights346-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-346-55,avg2-346-55 FILE=COLVAR346-55 STRIDE=10000 FMT=%16.10f

weights346-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=346 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-346-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights346-60 CLEAR=10000
avg2-346-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights346-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-346-60,avg2-346-60 FILE=COLVAR346-60 STRIDE=10000 FMT=%16.10f

weights346-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=346 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-346-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights346-65 CLEAR=10000
avg2-346-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights346-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-346-65,avg2-346-65 FILE=COLVAR346-65 STRIDE=10000 FMT=%16.10f

weights346-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=346 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-346-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights346-70 CLEAR=10000
avg2-346-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights346-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-346-70,avg2-346-70 FILE=COLVAR346-70 STRIDE=10000 FMT=%16.10f

weights346-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=346 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-346-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights346-75 CLEAR=10000
avg2-346-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights346-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-346-75,avg2-346-75 FILE=COLVAR346-75 STRIDE=10000 FMT=%16.10f

weights346-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=346 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-346-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights346-80 CLEAR=10000
avg2-346-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights346-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-346-80,avg2-346-80 FILE=COLVAR346-80 STRIDE=10000 FMT=%16.10f

weights346-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=346 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-346-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights346-85 CLEAR=10000
avg2-346-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights346-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-346-85,avg2-346-85 FILE=COLVAR346-85 STRIDE=10000 FMT=%16.10f

weights346-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=346 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-346-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights346-90 CLEAR=10000
avg2-346-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights346-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-346-90,avg2-346-90 FILE=COLVAR346-90 STRIDE=10000 FMT=%16.10f

weights346-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=346 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-346-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights346-95 CLEAR=10000
avg2-346-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights346-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-346-95,avg2-346-95 FILE=COLVAR346-95 STRIDE=10000 FMT=%16.10f

weights346-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=346 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-346-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights346-100 CLEAR=10000
avg2-346-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights346-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-346-100,avg2-346-100 FILE=COLVAR346-100 STRIDE=10000 FMT=%16.10f

weights348-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=348 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-348-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights348-0 CLEAR=10000
avg2-348-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights348-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-348-0,avg2-348-0 FILE=COLVAR348-0 STRIDE=10000 FMT=%16.10f

weights348-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=348 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-348-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights348-5 CLEAR=10000
avg2-348-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights348-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-348-5,avg2-348-5 FILE=COLVAR348-5 STRIDE=10000 FMT=%16.10f

weights348-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=348 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-348-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights348-10 CLEAR=10000
avg2-348-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights348-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-348-10,avg2-348-10 FILE=COLVAR348-10 STRIDE=10000 FMT=%16.10f

weights348-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=348 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-348-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights348-15 CLEAR=10000
avg2-348-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights348-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-348-15,avg2-348-15 FILE=COLVAR348-15 STRIDE=10000 FMT=%16.10f

weights348-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=348 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-348-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights348-20 CLEAR=10000
avg2-348-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights348-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-348-20,avg2-348-20 FILE=COLVAR348-20 STRIDE=10000 FMT=%16.10f

weights348-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=348 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-348-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights348-25 CLEAR=10000
avg2-348-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights348-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-348-25,avg2-348-25 FILE=COLVAR348-25 STRIDE=10000 FMT=%16.10f

weights348-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=348 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-348-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights348-30 CLEAR=10000
avg2-348-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights348-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-348-30,avg2-348-30 FILE=COLVAR348-30 STRIDE=10000 FMT=%16.10f

weights348-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=348 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-348-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights348-35 CLEAR=10000
avg2-348-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights348-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-348-35,avg2-348-35 FILE=COLVAR348-35 STRIDE=10000 FMT=%16.10f

weights348-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=348 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-348-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights348-40 CLEAR=10000
avg2-348-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights348-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-348-40,avg2-348-40 FILE=COLVAR348-40 STRIDE=10000 FMT=%16.10f

weights348-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=348 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-348-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights348-45 CLEAR=10000
avg2-348-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights348-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-348-45,avg2-348-45 FILE=COLVAR348-45 STRIDE=10000 FMT=%16.10f

weights348-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=348 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-348-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights348-50 CLEAR=10000
avg2-348-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights348-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-348-50,avg2-348-50 FILE=COLVAR348-50 STRIDE=10000 FMT=%16.10f

weights348-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=348 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-348-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights348-55 CLEAR=10000
avg2-348-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights348-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-348-55,avg2-348-55 FILE=COLVAR348-55 STRIDE=10000 FMT=%16.10f

weights348-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=348 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-348-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights348-60 CLEAR=10000
avg2-348-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights348-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-348-60,avg2-348-60 FILE=COLVAR348-60 STRIDE=10000 FMT=%16.10f

weights348-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=348 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-348-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights348-65 CLEAR=10000
avg2-348-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights348-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-348-65,avg2-348-65 FILE=COLVAR348-65 STRIDE=10000 FMT=%16.10f

weights348-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=348 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-348-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights348-70 CLEAR=10000
avg2-348-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights348-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-348-70,avg2-348-70 FILE=COLVAR348-70 STRIDE=10000 FMT=%16.10f

weights348-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=348 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-348-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights348-75 CLEAR=10000
avg2-348-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights348-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-348-75,avg2-348-75 FILE=COLVAR348-75 STRIDE=10000 FMT=%16.10f

weights348-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=348 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-348-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights348-80 CLEAR=10000
avg2-348-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights348-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-348-80,avg2-348-80 FILE=COLVAR348-80 STRIDE=10000 FMT=%16.10f

weights348-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=348 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-348-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights348-85 CLEAR=10000
avg2-348-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights348-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-348-85,avg2-348-85 FILE=COLVAR348-85 STRIDE=10000 FMT=%16.10f

weights348-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=348 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-348-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights348-90 CLEAR=10000
avg2-348-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights348-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-348-90,avg2-348-90 FILE=COLVAR348-90 STRIDE=10000 FMT=%16.10f

weights348-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=348 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-348-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights348-95 CLEAR=10000
avg2-348-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights348-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-348-95,avg2-348-95 FILE=COLVAR348-95 STRIDE=10000 FMT=%16.10f

weights348-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=348 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-348-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights348-100 CLEAR=10000
avg2-348-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights348-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-348-100,avg2-348-100 FILE=COLVAR348-100 STRIDE=10000 FMT=%16.10f

weights350-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=350 REWEIGHT_PRESSURE=0.0 ENERGY=renergy VOLUME=rvol
avg-350-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights350-0 CLEAR=10000
avg2-350-0: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights350-0 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-350-0,avg2-350-0 FILE=COLVAR350-0 STRIDE=10000 FMT=%16.10f

weights350-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=350 REWEIGHT_PRESSURE=3.0110704285 ENERGY=renergy VOLUME=rvol
avg-350-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights350-5 CLEAR=10000
avg2-350-5: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights350-5 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-350-5,avg2-350-5 FILE=COLVAR350-5 STRIDE=10000 FMT=%16.10f

weights350-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=350 REWEIGHT_PRESSURE=6.022140857 ENERGY=renergy VOLUME=rvol
avg-350-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights350-10 CLEAR=10000
avg2-350-10: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights350-10 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-350-10,avg2-350-10 FILE=COLVAR350-10 STRIDE=10000 FMT=%16.10f

weights350-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=350 REWEIGHT_PRESSURE=9.0332112855 ENERGY=renergy VOLUME=rvol
avg-350-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights350-15 CLEAR=10000
avg2-350-15: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights350-15 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-350-15,avg2-350-15 FILE=COLVAR350-15 STRIDE=10000 FMT=%16.10f

weights350-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=350 REWEIGHT_PRESSURE=12.044281714 ENERGY=renergy VOLUME=rvol
avg-350-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights350-20 CLEAR=10000
avg2-350-20: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights350-20 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-350-20,avg2-350-20 FILE=COLVAR350-20 STRIDE=10000 FMT=%16.10f

weights350-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=350 REWEIGHT_PRESSURE=15.0553521425 ENERGY=renergy VOLUME=rvol
avg-350-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights350-25 CLEAR=10000
avg2-350-25: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights350-25 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-350-25,avg2-350-25 FILE=COLVAR350-25 STRIDE=10000 FMT=%16.10f

weights350-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=350 REWEIGHT_PRESSURE=18.066422571 ENERGY=renergy VOLUME=rvol
avg-350-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights350-30 CLEAR=10000
avg2-350-30: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights350-30 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-350-30,avg2-350-30 FILE=COLVAR350-30 STRIDE=10000 FMT=%16.10f

weights350-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=350 REWEIGHT_PRESSURE=21.0774929995 ENERGY=renergy VOLUME=rvol
avg-350-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights350-35 CLEAR=10000
avg2-350-35: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights350-35 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-350-35,avg2-350-35 FILE=COLVAR350-35 STRIDE=10000 FMT=%16.10f

weights350-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=350 REWEIGHT_PRESSURE=24.088563428 ENERGY=renergy VOLUME=rvol
avg-350-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights350-40 CLEAR=10000
avg2-350-40: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights350-40 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-350-40,avg2-350-40 FILE=COLVAR350-40 STRIDE=10000 FMT=%16.10f

weights350-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=350 REWEIGHT_PRESSURE=27.0996338565 ENERGY=renergy VOLUME=rvol
avg-350-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights350-45 CLEAR=10000
avg2-350-45: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights350-45 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-350-45,avg2-350-45 FILE=COLVAR350-45 STRIDE=10000 FMT=%16.10f

weights350-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=350 REWEIGHT_PRESSURE=30.110704285 ENERGY=renergy VOLUME=rvol
avg-350-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights350-50 CLEAR=10000
avg2-350-50: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights350-50 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-350-50,avg2-350-50 FILE=COLVAR350-50 STRIDE=10000 FMT=%16.10f

weights350-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=350 REWEIGHT_PRESSURE=33.1217747135 ENERGY=renergy VOLUME=rvol
avg-350-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights350-55 CLEAR=10000
avg2-350-55: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights350-55 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-350-55,avg2-350-55 FILE=COLVAR350-55 STRIDE=10000 FMT=%16.10f

weights350-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=350 REWEIGHT_PRESSURE=36.132845142 ENERGY=renergy VOLUME=rvol
avg-350-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights350-60 CLEAR=10000
avg2-350-60: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights350-60 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-350-60,avg2-350-60 FILE=COLVAR350-60 STRIDE=10000 FMT=%16.10f

weights350-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=350 REWEIGHT_PRESSURE=39.1439155705 ENERGY=renergy VOLUME=rvol
avg-350-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights350-65 CLEAR=10000
avg2-350-65: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights350-65 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-350-65,avg2-350-65 FILE=COLVAR350-65 STRIDE=10000 FMT=%16.10f

weights350-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=350 REWEIGHT_PRESSURE=42.154985999 ENERGY=renergy VOLUME=rvol
avg-350-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights350-70 CLEAR=10000
avg2-350-70: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights350-70 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-350-70,avg2-350-70 FILE=COLVAR350-70 STRIDE=10000 FMT=%16.10f

weights350-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=350 REWEIGHT_PRESSURE=45.1660564275 ENERGY=renergy VOLUME=rvol
avg-350-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights350-75 CLEAR=10000
avg2-350-75: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights350-75 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-350-75,avg2-350-75 FILE=COLVAR350-75 STRIDE=10000 FMT=%16.10f

weights350-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=350 REWEIGHT_PRESSURE=48.177126856 ENERGY=renergy VOLUME=rvol
avg-350-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights350-80 CLEAR=10000
avg2-350-80: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights350-80 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-350-80,avg2-350-80 FILE=COLVAR350-80 STRIDE=10000 FMT=%16.10f

weights350-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=350 REWEIGHT_PRESSURE=51.1881972845 ENERGY=renergy VOLUME=rvol
avg-350-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights350-85 CLEAR=10000
avg2-350-85: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights350-85 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-350-85,avg2-350-85 FILE=COLVAR350-85 STRIDE=10000 FMT=%16.10f

weights350-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=350 REWEIGHT_PRESSURE=54.199267713 ENERGY=renergy VOLUME=rvol
avg-350-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights350-90 CLEAR=10000
avg2-350-90: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights350-90 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-350-90,avg2-350-90 FILE=COLVAR350-90 STRIDE=10000 FMT=%16.10f

weights350-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=350 REWEIGHT_PRESSURE=57.2103381415 ENERGY=renergy VOLUME=rvol
avg-350-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights350-95 CLEAR=10000
avg2-350-95: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights350-95 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-350-95,avg2-350-95 FILE=COLVAR350-95 STRIDE=10000 FMT=%16.10f

weights350-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__t_e_m_p__p_r_e_s_s.html">REWEIGHT_TEMP_PRESS</a> TEMP=300 PRESSURE=0.06022140857 REWEIGHT_TEMP=350 REWEIGHT_PRESSURE=60.22140857 ENERGY=renergy VOLUME=rvol
avg-350-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=vol LOGWEIGHTS=weights,weights350-100 CLEAR=10000
avg2-350-100: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_v_e_r_a_g_e.html">AVERAGE</a> ARG=energy LOGWEIGHTS=weights,weights350-100 CLEAR=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=avg-350-100,avg2-350-100 FILE=COLVAR350-100 STRIDE=10000 FMT=%16.10f

</pre>{% endraw %}
