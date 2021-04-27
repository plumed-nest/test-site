**Project ID:** [plumID:20.017]({{ '/' | absolute_url }}eggs/20/017/)  
**Source:** beaded-helix/helix_sf_f-4.5_eps7.5_10000000.plumed.dat  
**Originally used with PLUMED version:** 2.7  
**Stable:** [raw zipped stdout](helix_sf_f-4.5_eps7.5_10000000.plumed.dat.plumed.stdout.txt.zip) - [stderr](helix_sf_f-4.5_eps7.5_10000000.plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](helix_sf_f-4.5_eps7.5_10000000.plumed.dat.plumed_master.stdout.txt.zip) - [stderr](helix_sf_f-4.5_eps7.5_10000000.plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue">#UNITS LENGTH=A TIME=fs ENERGY=kcal/mol</span>

b1: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=1
b2: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=12
cas: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=1-12

dend: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=b1,b2
rg: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_y_r_a_t_i_o_n.html">GYRATION</a> TYPE=RADIUS ATOMS=cas
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a> LABEL=en

<span style="color:blue">#The conversion factor is 69.4786 pN = 1 kcal/mol/Angstrom</span>
<span style="color:blue">#100pN = 1.4425 kcal/mol/A</span>
p: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ...
    ARG=dend
    AT=0
    SLOPE=-4.5
    KAPPA=0
... p:

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=dend,en,p.bias,p.force2 STRIDE=1000 FILE=helix_sf_f-4.5_eps7.5_10000000.en.colvars.dat FMT=%8.4f
</pre>{% endraw %}
