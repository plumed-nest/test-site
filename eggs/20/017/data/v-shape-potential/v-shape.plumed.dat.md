**Project ID:** [plumID:20.017]({{ '/' | absolute_url }}eggs/20/017/)  
**Source:** v-shape-potential/v-shape.plumed.dat  
**Originally used with PLUMED version:** 2.7  
**Stable:** [raw zipped stdout](v-shape.plumed.dat.plumed.stdout.txt.zip) - [stderr](v-shape.plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](v-shape.plumed.dat.plumed_master.stdout.txt.zip) - [stderr](v-shape.plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
d1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1,2 COMPONENTS
ff: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=d1.x,d1.y PERIODIC=NO FUNC=-8*log((exp(-(y-exp(-x))^2/2)+exp(-(y+exp(-x))^2/2))*exp(-x^2/2))
bb: <a href="https://plumed.github.io/doc-master/user-doc/html/_b_i_a_s_v_a_l_u_e.html">BIASVALUE</a> ARG=ff

f: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_i_s_s_t.html">FISST</a> MIN_FORCE=-15 MAX_FORCE=15.0 PERIOD=200 NINTERPOLATE=41 ARG=d1.x KBT=1.0 OUT_RESTART=v-shape_fisst-15_15_scale8_seed1.restart.txt OUT_OBSERVABLE=v-shape_fisst-15_15_scale8_seed1.observable.txt OBSERVABLE_FREQ=100 CENTER=0

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=d1.x,d1.y,bb.bias,f.d1.x_fbar,f.bias,f.force2 FILE=v-shape_fisst-15_15_scale8_seed1.colvar.txt STRIDE=100
</pre>{% endraw %}
