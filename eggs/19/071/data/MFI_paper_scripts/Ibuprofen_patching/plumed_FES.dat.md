**Project ID:** [plumID:19.071]({{ '/' | absolute_url }}eggs/19/071/)  
**Source:** MFI_paper_scripts/Ibuprofen_patching/plumed_FES.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed_FES.dat.plumed.stdout.txt.zip) - [stderr](plumed_FES.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_FES.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_FES.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue">#torsion1 between vector C1,C2 and C10,C11 with axis C2,C10</span>
t1: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5911,5910 AXIS=5919,5911 VECTOR2=5919,5920

<span style="color:blue">#torsion2 between vector C7,C10 and C11,C12 with axis C10,C11</span>
t2: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5919,5916 AXIS=5920,5919 VECTOR2=5920,5921

<span style="color:blue">#metadynamics</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
ARG=t1,t2
SIGMA=0.1,0.1
HEIGHT=0.96
PACE=500
BIASFACTOR=10.0
TEMP=300.0
LABEL=metad
FILE=HILLS
GRID_MIN=-pi,-pi
GRID_MAX=pi,pi
GRID_BIN=350,350
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=t1,t2,metad.bias FILE=COLVAR
</pre>{% endraw %}
