**Project ID:** [plumID:20.028]({{ '/' | absolute_url }}eggs/20/028/)  
**Source:** wild-type/plumed-1.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [raw zipped stdout](plumed-1.dat.plumed.stdout.txt.zip) - [stderr](plumed-1.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed-1.dat.plumed_master.stdout.txt.zip) - [stderr](plumed-1.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_f_i_t__t_o__t_e_m_p_l_a_t_e.html">FIT_TO_TEMPLATE</a> REFERENCE=step5_charmm2gmx-modified-1.pdb
first: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=3006-3053       <span style="color:blue">#  GTP</span>
second: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=2955-3005      <span style="color:blue">#  FAR</span>
last: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=9733-33193:138   <span style="color:blue">#  all P atoms in system--range with a stride 118</span>
gtp: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=first,last COMPONENTS
far: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=second,last COMPONENTS

<span style="color:blue"># Activate metadynamics in phi and psi</span>
<span style="color:blue"># depositing a Gaussian every 500 time steps,</span>
<span style="color:blue"># with height equal to 1.2 kJoule/mol,</span>
<span style="color:blue"># and width 0.35 rad for both CVs. </span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
LABEL=metad
ARG=gtp.z,far.z
PACE=500
HEIGHT=1.2
SIGMA=0.10,0.35
FILE=HILLS2
BIASFACTOR=5.0
TEMP=310.0
GRID_MIN=-15.0,-10.0
GRID_MAX=15.0,10.0
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<span style="color:blue"># monitor the two variables and the metadynamics bias potential</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=200 ARG=gtp.z,far.z,metad.bias FILE=COLVAR2
</pre>{% endraw %}
