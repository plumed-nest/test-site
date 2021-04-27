**Project ID:** [plumID:20.017]({{ '/' | absolute_url }}eggs/20/017/)  
**Source:** ala10/ala10.plumed.dat  
**Originally used with PLUMED version:** 2.7  
**Stable:** [raw zipped stdout](ala10.plumed.dat.plumed.stdout.txt.zip) - [stderr](ala10.plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](ala10.plumed.dat.plumed_master.stdout.txt.zip) - [stderr](ala10.plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> LENGTH=A TIME=fs ENERGY=kcal/mol

b1: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=5
b2: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=95
cas: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=5-100:10

dend: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=b1,b2
rg: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_y_r_a_t_i_o_n.html">GYRATION</a> TYPE=RADIUS ATOMS=cas

<span style="color:blue">#The conversion factor is 69.4786 pN = 1 kcal/mol/Angstrom</span>

<span style="color:blue">#-10 pN to 10 pN</span>
f: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_i_s_s_t.html">FISST</a> MIN_FORCE=-0.144 MAX_FORCE=0.144 PERIOD=200 NINTERPOLATE=31 ARG=dend OUT_RESTART=ala10_pull_fRange_fmin-10_fmax10.restart.txt OUT_OBSERVABLE=ala10_pull_fRange_fmin-10_fmax10.observable.txt OBSERVABLE_FREQ=1000 CENTER=0 RESTART_FMT=%e 

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=dend,rg,f.dend_fbar,f.bias,f.force2 FILE=ala10_pull_fRange_fmin-10_fmax10.colvar.txt STRIDE=1000
</pre>{% endraw %}
