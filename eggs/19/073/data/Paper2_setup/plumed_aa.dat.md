**Project ID:** [plumID:19.073]({{ '/' | absolute_url }}eggs/19/073/)  
**Source:** Paper2_setup/plumed_aa.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed_aa.dat.plumed.stdout.txt.zip) - [stderr](plumed_aa.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_aa.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_aa.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> LABEL=d1 GROUPA=1-3,61-63  GROUPB=82,98,114,22,38,54 LOWEST LOWMEM
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> LABEL=d2 GROUPA=1-3        GROUPB=61-63              LOWEST LOWMEM
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> LABEL=cv1 SPECIESA=1-3,61-63 SPECIESB=23,24,39,40,55,56,83,84,99,100,115,116 R_0=0.25 MORE_THAN={RATIONAL R_0=0.5 NN=2 MM=4 D_0=0}
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a> LABEL=ene

<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=d1.lowest AT=0.35 KAPPA=150 EXP=2 EPS=1 OFFSET=0 LABEL=uwall
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=d1.lowest AT=0.15 KAPPA=150 EXP=2 EPS=1 OFFSET=0 LABEL=lwall

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
ARG=cv1.morethan,ene SIGMA=0.01,200 HEIGHT=2.5 PACE=500
LABEL=metad TEMP=298 BIASFACTOR=100 FILE=hills_aa
GRID_MIN=-0.5,-200000 GRID_MAX=6,-120000 GRID_BIN=526,350 GRID_SPARSE
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=100 ARG=* FILE=colvar_aa.dat

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
