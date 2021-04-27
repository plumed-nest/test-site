**Project ID:** [plumID:19.014]({{ '/' | absolute_url }}eggs/19/014/)  
**Source:** mil-101_paper_setup/plumed_files/plumed_gyration.dat  
**Originally used with PLUMED version:** 2.2  
**Stable:** [raw zipped stdout](plumed_gyration.dat.plumed.stdout.txt.zip) - [stderr](plumed_gyration.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_gyration.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_gyration.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_g_y_r_a_t_i_o_n.html">GYRATION</a> LABEL=gyr ATOMS=1-60 MASS_WEIGHTED

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
ARG=gyr SIGMA=0.01 HEIGHT=2.5 PACE=500
LABEL=metad TEMP=298 BIASFACTOR=10 FILE=hills
GRID_MIN=-0.05 GRID_MAX=1.0 GRID_SPACING=0.002 GRID_SPARSE
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=100 ARG=gyr,metad.bias FILE=colvar
</pre>{% endraw %}
