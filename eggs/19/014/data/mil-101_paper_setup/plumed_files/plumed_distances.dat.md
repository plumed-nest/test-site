**Project ID:** [plumID:19.014]({{ '/' | absolute_url }}eggs/19/014/)  
**Source:** mil-101_paper_setup/plumed_files/plumed_distances.dat  
**Originally used with PLUMED version:** 2.2  
**Stable:** [raw zipped stdout](plumed_distances.dat.plumed.stdout.txt.zip) - [stderr](plumed_distances.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_distances.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_distances.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> LABEL=d1 GROUPA=1-3,61-63  GROUPB=82,98,114,22,38,54 LOWEST LOWMEM
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> LABEL=d2 GROUPA=1-3        GROUPB=61-63              LOWEST LOWMEM

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
ARG=d1.lowest,d2.lowest SIGMA=0.01,0.01 HEIGHT=2.5
PACE=500 LABEL=metad TEMP=298 BIASFACTOR=30 FILE=hills
GRID_MIN=-0.1,-0.1 GRID_MAX=6.0,6.0     
GRID_SPACING=0.005,0.005 GRID_SPARSE
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=100 ARG=d1.lowest,d2.lowest,metad.bias FILE=colvar

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
