**Project ID:** [plumID:19.078]({{ '/' | absolute_url }}eggs/19/078/)  
**Source:** meta_reweigthing/LJ-38/plumed.dat  
**Originally used with PLUMED version:** 2.5-mod  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># plumed input file</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> NATURAL
nsa: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIES=1-38 SWITCH={CUBIC D_0=1.25 D_MAX=1.5} 

ns: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=nsa FUNC=exp(-(x-6)*(x-6)/(2*0.5*0.5)) PERIODIC=NO
ne: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=nsa FUNC=exp(-(x-8)*(x-8)/(2*0.5*0.5)) PERIODIC=NO

mt: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
ARG=ns,ne 
PACE=500 
SIGMA=0.5,0.5 
BIASFACTOR=4 HEIGHT=0.2 TEMP=0.168 
GRID_MIN=0.,0. GRID_MAX=25,20 GRID_BIN=300,300
CALC_RCT
...

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=ns,ne,mt.bias,mt.rct,mt.rbias FMT=%8.4f FILE=colvar STRIDE=500
</pre>{% endraw %}
