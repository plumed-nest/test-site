**Project ID:** [plumID:20.017]({{ '/' | absolute_url }}eggs/20/017/)  
**Source:** beaded-helix/helix_fisst_fmin-2.0_fmax8.0_eps7.5_10000000.plumed.dat  
**Originally used with PLUMED version:** 2.7  
**Stable:** [raw zipped stdout](helix_fisst_fmin-2.0_fmax8.0_eps7.5_10000000.plumed.dat.plumed.stdout.txt.zip) - [stderr](helix_fisst_fmin-2.0_fmax8.0_eps7.5_10000000.plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](helix_fisst_fmin-2.0_fmax8.0_eps7.5_10000000.plumed.dat.plumed_master.stdout.txt.zip) - [stderr](helix_fisst_fmin-2.0_fmax8.0_eps7.5_10000000.plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue">#UNITS LENGTH=A TIME=fs ENERGY=kcal/mol</span>

b1: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=1
b2: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=12
cas: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=1-12

dend: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=b1,b2
rg: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_y_r_a_t_i_o_n.html">GYRATION</a> TYPE=RADIUS ATOMS=cas
en: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a> 

<span style="color:blue">#The conversion factor is 69.4786 pN = 1 kcal/mol/Angstrom</span>

<span style="color:blue">#0 pN to 100 pN</span>
f: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_i_s_s_t.html">FISST</a> MIN_FORCE=-2.0 MAX_FORCE=8.0 PERIOD=200 NINTERPOLATE=31 ARG=dend OUT_RESTART=helix_fisst_fmin-2.0_fmax8.0_eps7.5_10000000.restart.txt OUT_OBSERVABLE=helix_fisst_fmin-2.0_fmax8.0_eps7.5_10000000.observable.txt OBSERVABLE_FREQ=1000 CENTER=0 KBT=1

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=dend,rg,en,f.dend_fbar,f.bias,f.force2 FILE=helix_fisst_fmin-2.0_fmax8.0_eps7.5_10000000.en.colvar.txt STRIDE=5000
</pre>{% endraw %}
