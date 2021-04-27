**Project ID:** [plumID:19.014]({{ '/' | absolute_url }}eggs/19/014/)  
**Source:** mil-101_paper_setup/plumed_files/plumed_coordination.dat  
**Originally used with PLUMED version:** 2.2  
**Stable:** [raw zipped stdout](plumed_coordination.dat.plumed.stdout.txt.zip) - [stderr](plumed_coordination.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_coordination.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_coordination.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> LABEL=cn SPECIESA=1-3,61-63 SPECIESB=23,24,39,40,55,56,83,84,99,100,115,116 R_0=0.25 MORE_THAN={RATIONAL R_0=0.5 NN=2 MM=4 D_0=0}

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
ARG=cn.morethan SIGMA=0.01 HEIGHT=2.5 PACE=500
LABEL=metad TEMP=298 BIASFACTOR=50 FILE=hills
GRID_MIN=-0.5 GRID_MAX=6 GRID_SPACING=0.002 GRID_SPARSE
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=100 ARG=cn.morethan,metad.bias FILE=colvar

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
