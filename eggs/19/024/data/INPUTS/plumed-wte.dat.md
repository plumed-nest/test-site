**Project ID:** [plumID:19.024]({{ '/' | absolute_url }}eggs/19/024/)  
**Source:** INPUTS/plumed-wte.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [raw zipped stdout](plumed-wte.dat.plumed.stdout.txt.zip) - [stderr](plumed-wte.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed-wte.dat.plumed_master.stdout.txt.zip) - [stderr](plumed-wte.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># CV definition</span>
ene: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a>

<span style="color:blue"># MetaD parameters</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
  ARG=ene SIGMA=500 HEIGHT=2.0 PACE=125
  TEMP=300 BIASFACTOR=24 FILE=HILLS
  GRID_MIN=-175000 GRID_MAX=-75000 GRID_BIN=500 
  GRID_WSTRIDE=500000 GRID_WFILE=BIAS
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>
</pre>{% endraw %}
