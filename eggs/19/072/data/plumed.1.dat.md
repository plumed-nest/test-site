**Project ID:** [plumID:19.072]({{ '/' | absolute_url }}eggs/19/072/)  
**Source:** plumed.1.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed.1.dat.plumed.stdout.txt.zip) - [stderr](plumed.1.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.1.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.1.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>
<a href="https://plumed.github.io/doc-master/user-doc/html/_i_n_c_l_u_d_e.html">INCLUDE</a> FILE=<a href="cv.dat.html">cv.dat</a>
<a href="https://plumed.github.io/doc-master/user-doc/html/_i_n_c_l_u_d_e.html">INCLUDE</a> FILE=<a href="plu_maxent_NOE_RECT.dat.html">plu_maxent_NOE_RECT.dat</a>
 
<span style="color:blue">###########################</span>
<span style="color:blue">#### Metadynamics</span>
<span style="color:blue">###########################</span>
 
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=c77 SIGMA=0.25 HEIGHT=0.0720625 PACE=500 BIASFACTOR=1.3459 TEMP=300 GRID_MIN=-pi GRID_MAX=pi FILE=HILLSc77
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=c78 SIGMA=0.25 HEIGHT=0.0720625 PACE=500 BIASFACTOR=1.3459 TEMP=300 GRID_MIN=-pi GRID_MAX=pi FILE=HILLSc78
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=c79 SIGMA=0.25 HEIGHT=0.0720625 PACE=500 BIASFACTOR=1.3459 TEMP=300 GRID_MIN=-pi GRID_MAX=pi FILE=HILLSc79
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=co77 SIGMA=0.05 HEIGHT=0.0720625 PACE=500 BIASFACTOR=1.3459 TEMP=300 GRID_MIN=0 GRID_MAX=30 FILE=HILLSco77
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=co78 SIGMA=0.05 HEIGHT=0.0720625 PACE=500 BIASFACTOR=1.3459 TEMP=300 GRID_MIN=0 GRID_MAX=30 FILE=HILLSco78
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=co79 SIGMA=0.05 HEIGHT=0.0720625 PACE=500 BIASFACTOR=1.3459 TEMP=300 GRID_MIN=0 GRID_MAX=30 FILE=HILLSco79
 
<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=50000
</pre>{% endraw %}
