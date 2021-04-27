**Project ID:** [plumID:19.079]({{ '/' | absolute_url }}eggs/19/079/)  
**Source:** tio2_glu/plumed.dat  
**Originally used with PLUMED version:** 2.4.2  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim: ft=plumed</a></span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>

<span style="color:blue"># Ref atom on surf</span>
ref: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=2572

<span style="color:blue"># Entire peptide COM to surface</span>
c: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=1-27
d: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=ref,c COMPONENTS NOPBC

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
LABEL=mtd
ARG=d.z 
PACE=1000
BIASFACTOR=10
HEIGHT=2.0
SIGMA=0.01
FILE=HILLS
GRID_MIN=-1
GRID_MAX=10
WALKERS_MPI
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<span style="color:blue">## wall </span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=d.z AT=3.0 KAPPA=50000 LABEL=uwall

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=* STRIDE=1000 FILE=COLVAR

</pre>{% endraw %}
