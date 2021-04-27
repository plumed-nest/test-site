**Project ID:** [plumID:19.024]({{ '/' | absolute_url }}eggs/19/024/)  
**Source:** INPUTS/plumed-pt-metad-wte.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [raw zipped stdout](plumed-pt-metad-wte.dat.plumed.stdout.txt.zip) - [stderr](plumed-pt-metad-wte.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed-pt-metad-wte.dat.plumed_master.stdout.txt.zip) - [stderr](plumed-pt-metad-wte.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># Groups definition</span>
h:    <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=77,94,118,137,159,178,210,228
o:    <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=92,116,135,157,169,183,219,250
core: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=48,108,188,269

<span style="color:blue"># CVs definition</span>
s_a:  <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=h GROUPB=o PAIR  NN=8 MM=12 R_0=0.25
s_hc: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=core GROUPB=core NN=8 MM=12 R_0=0.50
ene:  <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a>

<span style="color:blue"># MetaD parameters</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
  ARG=s_a,s_hc SIGMA=0.4,0.4 HEIGHT=2.5 PACE=250
  TEMP=300 BIASFACTOR=8 FILE=HILLS
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<span style="color:blue"># WTE bias</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_x_t_e_r_n_a_l.html">EXTERNAL</a> ARG=ene FILE=BIAS
</pre>{% endraw %}
