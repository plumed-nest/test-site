**Project ID:** [plumID:20.020]({{ '/' | absolute_url }}eggs/20/020/)  
**Source:** plumed.dat  
**Originally used with PLUMED version:** 2.2  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># include definition of CVs</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_i_n_c_l_u_d_e.html">INCLUDE</a> FILE=<a href="plumed_cv.dat.html">plumed_cv.dat</a>

<span style="color:blue"># Parallel-bias metadynamics</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_b_m_e_t_a_d.html">PBMETAD</a> ...
ARG=rg,hb,hc,helix,beta,dih
PACE=500 BIASFACTOR=8.0 HEIGHT=1.2 TEMP=300.0
SIGMA=0.01,0.6,0.3,0.4,0.3,0.6
GRID_MIN=0.4,0.0,0.0,0.0,0.0,0.0
GRID_MAX=2.0,100.0,25.0,40.0,40.0,40.0
FILE=HILLS_rg,HILLS_hb,HILLS_hc,HILLS_helix,HILLS_beta,HILLS_dih LABEL=metad
... <a href="https://plumed.github.io/doc-master/user-doc/html/_p_b_m_e_t_a_d.html">PBMETAD</a>
</pre>{% endraw %}
