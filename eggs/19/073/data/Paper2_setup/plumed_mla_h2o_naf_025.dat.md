**Project ID:** [plumID:19.073]({{ '/' | absolute_url }}eggs/19/073/)  
**Source:** Paper2_setup/plumed_mla_h2o_naf_025.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed_mla_h2o_naf_025.dat.plumed.stdout.txt.zip) - [stderr](plumed_mla_h2o_naf_025.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_mla_h2o_naf_025.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_mla_h2o_naf_025.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_g_y_r_a_t_i_o_n.html">GYRATION</a> LABEL=gyr ATOMS=1-60 MASS_WEIGHTED

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
ARG=gyr SIGMA=0.01 HEIGHT=2.5 PACE=500
LABEL=metad TEMP=298 BIASFACTOR=50 FILE=hills_mla_h2o_naf_025
GRID_MIN=-0.05 GRID_MAX=1.0 GRID_SPACING=0.002 GRID_SPARSE
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=100 ARG=gyr,metad.bias FILE=colvar_mla_h2o_naf_025.dat

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
