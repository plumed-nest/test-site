**Project ID:** [plumID:19.041]({{ '/' | absolute_url }}eggs/19/041/)  
**Source:** DDD_SIO/plumed.dat  
**Originally used with PLUMED version:** 2.4.0-dev  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a> LABEL=energy

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=1-48 LABEL=c

<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1893,c LABEL=d COMPONENTS NOPBC

<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=d.z AT=1.8 KAPPA=1000000 LABEL=uwall  

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
ARG=d.z SIGMA=0.021 FILE=HILLS_MTD HEIGHT=2.0 PACE=1000 BIASFACTOR=12 TEMP=300.0 LABEL=cv
GRID_MIN=-2
GRID_MAX=2
WALKERS_MPI
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>


<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=* STRIDE=250 FILE=COLVAR
</pre>{% endraw %}
