**Project ID:** [plumID:19.071]({{ '/' | absolute_url }}eggs/19/071/)  
**Source:** MFI_paper_scripts/reweighting/plumed_FB.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed_FB.dat.plumed.stdout.txt.zip) - [stderr](plumed_FB.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_FB.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_FB.dat.plumed_master.stderr)  

{% raw %}<pre>
p: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_a_d.html">READ</a>  FILE=./position  VALUES=p.x IGNORE_FORCES IGNORE_TIME

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ... 
ARG=p.x
SIGMA=0.05 
HEIGHT=0.1 
PACE=500 
BIASFACTOR=5 
LABEL=metad 
TEMP=120
GRID_MIN=-2.7
GRID_MAX=2.7
GRID_BIN=500
GRID_WSTRIDE=100000
GRID_WFILE=grid.dat
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>


</pre>{% endraw %}
