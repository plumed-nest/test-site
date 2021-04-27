**Project ID:** [plumID:19.062]({{ '/' | absolute_url }}eggs/19/062/)  
**Source:** utilities/plumed.dat  
**Originally used with PLUMED version:** 2.3  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
en: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
ARG=en
PACE=250 BIASFACTOR=21.0 HEIGHT=4.18 
SIGMA=250
GRID_MIN=-300000.000000
GRID_MAX=-200000.000000
FILE=HILLS
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<span style="color:blue">#make STRIDE = to your exchange attempt frequency!!!</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FILE=COLVAR ARG=* STRIDE=250
</pre>{% endraw %}
