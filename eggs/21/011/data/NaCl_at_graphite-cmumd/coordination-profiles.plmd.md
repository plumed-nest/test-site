**Project ID:** [plumID:21.011]({{ '/' | absolute_url }}eggs/21/011/)  
**Source:** NaCl_at_graphite-cmumd/coordination-profiles.plmd  
**Originally used with PLUMED version:** 2.5.1  
**Stable:** [raw zipped stdout](coordination-profiles.plmd.plumed.stdout.txt.zip) - [stderr](coordination-profiles.plmd.plumed.stderr)  
**Master:** [raw zipped stdout](coordination-profiles.plmd.plumed_master.stdout.txt.zip) - [stderr](coordination-profiles.plmd.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># Define atom groups</span>
gra: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=1-9152:1 
wat: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=9153-43319:3
sod: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=43320-43737:1
chl: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=43738-44155:1
slt: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=43320-44155:1
sln: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=9153-44155:1 

<span style="color:blue"># Set a virtual atom at the origin and in the 'bulk'</span>
p0: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_i_x_e_d_a_t_o_m.html">FIXEDATOM</a> AT=2.696525,2.75872,7.403535
p1: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_i_x_e_d_a_t_o_m.html">FIXEDATOM</a> AT=2.696525,2.75872,11.403535

<span style="color:blue"># Get the coordination number distributions</span>
cn0:  <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIESA=sod SPECIESB=chl SWITCH={RATIONAL R_0=0.355 NN=32 MM=64}
cn1:  <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIESA=sod SPECIESB=wat SWITCH={RATIONAL R_0=0.325 NN=32 MM=64}
cn2:  <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIESA=chl SPECIESB=wat SWITCH={RATIONAL R_0=0.385 NN=32 MM=64}
cn3:  <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIESA=sod SPECIESB=gra SWITCH={RATIONAL R_0=0.365 NN=32 MM=64}
ips: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_f_i_l_t_e_r__m_o_r_e.html">MFILTER_MORE</a> DATA=cn0 SWITCH={GAUSSIAN D_0=0.9999 R_0=0.00001}

densnacl: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_u_l_t_i_c_o_l_v_a_r_d_e_n_s.html">MULTICOLVARDENS</a> DATA=cn0 ORIGIN=p0 DIR=z NBINS=1480 KERNEL=GAUSSIAN BANDWIDTH=0.03 NORMALIZATION=true STRIDE=1
densnaow: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_u_l_t_i_c_o_l_v_a_r_d_e_n_s.html">MULTICOLVARDENS</a> DATA=cn1 ORIGIN=p0 DIR=z NBINS=1480 KERNEL=GAUSSIAN BANDWIDTH=0.03 NORMALIZATION=true STRIDE=1
densclow: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_u_l_t_i_c_o_l_v_a_r_d_e_n_s.html">MULTICOLVARDENS</a> DATA=cn2 ORIGIN=p0 DIR=z NBINS=1480 KERNEL=GAUSSIAN BANDWIDTH=0.03 NORMALIZATION=true STRIDE=1
densnagra: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_u_l_t_i_c_o_l_v_a_r_d_e_n_s.html">MULTICOLVARDENS</a> DATA=cn3 ORIGIN=p0 DIR=z NBINS=1480 KERNEL=GAUSSIAN BANDWIDTH=0.03 NORMALIZATION=true STRIDE=1
densips: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_u_l_t_i_c_o_l_v_a_r_d_e_n_s.html">MULTICOLVARDENS</a> DATA=ips ORIGIN=p0 DIR=z NBINS=1480 KERNEL=GAUSSIAN BANDWIDTH=0.03 NORMALIZATION=true STRIDE=1

<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=densnacl FILE=DENSna-cl.dat
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=densnaow FILE=DENSna-ow.dat
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=densclow FILE=DENScl-ow.dat
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=densnagra FILE=DENSna-gra.dat
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=densips FILE=DENSips.dat

</pre>{% endraw %}
