**Project ID:** [plumID:19.078]({{ '/' | absolute_url }}eggs/19/078/)  
**Source:** meta_reweigthing/2_D/plumed_reweight.dat  
**Originally used with PLUMED version:** 2.5-mod  
**Stable:** [raw zipped stdout](plumed_reweight.dat.plumed.stdout.txt.zip) - [stderr](plumed_reweight.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_reweight.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_reweight.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># plumed input file for reweighting</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> NATURAL
d1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1,2 COMPONENTS

ff: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=d1.x,d1.y VAR=x0,x1 PERIODIC=NO FUNC=30.0*exp(-4.0*(x0-1)^2-4.0*(x1-1)^2)+30.0*exp(-4.0*(x0-1)^2-4.0*(x1+1)^2)+30.0*exp(-4.0*(x0+1)^2-4.0*(x1+1)^2)+30.0/(1.0/((5.0*x0+5.0)^2+(5.0*x1+5.0)^2+1)+1.0/((5.0*x0-5.0)^2+(5.0*x1+5.0)^2+1)+1.0/((5.0*x0-5.0)^2+(5.0*x1-5.0)^2+1)+1.0/((-3.5355339059*x0+3.5355339059*x1)^2+(0.500000000834386*x0+0.500000000834386*x1)^8)+1.0/(1.0*x1^8+(5.0*x0-5.0)^2)+1.0/(1.0*x0^8+(5.0*x1+5.0)^2))

bb: <a href="https://plumed.github.io/doc-master/user-doc/html/_b_i_a_s_v_a_l_u_e.html">BIASVALUE</a> ARG=ff

mt: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
ARG=d1.x,d1.y PACE=1
GRID_MIN=-1.5,-1.5 GRID_MAX=1.5,1.5 GRID_BIN=150,150
HEIGHT=2.0 SIGMA=0.1,0.1 BIASFACTOR=5 TEMP=1
...

rw: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__b_i_a_s.html">REWEIGHT_BIAS</a> ARG=mt.bias TEMP=1  <span style="color:blue"># This is the inverse of boltzmann's constant in kJ mol-1</span>
cc: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_l_l_e_c_t__f_r_a_m_e_s.html">COLLECT_FRAMES</a> ARG=d1.x,d1.y LOGWEIGHTS=rw STRIDE=100
it: <a href="https://plumed.github.io/doc-master/user-doc/html/_i_t_r_e.html">ITRE</a> ARG=cc.logweights TEMP=1 MAXITER=20
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=it FILE=c_t.dat FMT=%8.4f
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=mt.bias FILE=bias.reweight STRIDE=10
</pre>{% endraw %}
