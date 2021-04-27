**Project ID:** [plumID:19.015]({{ '/' | absolute_url }}eggs/19/015/)  
**Source:** solid/plumed_restart.dat  
**Originally used with PLUMED version:** 2.3  
**Stable:** [raw zipped stdout](plumed_restart.dat.plumed.stdout.txt.zip) - [stderr](plumed_restart.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_restart.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_restart.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue">#torsion1 between vector1 C2,C1 and axis C2,C10 and vector2 C10,C11 </span>
t1: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=4492,4491 AXIS=4492,4500 VECTOR2=4500,4501

<span style="color:blue">#torsion2 between vector1 C10,C7 and axis C10,C11 and vecotr2 C11,C12 </span>
t2: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=4500,4497 AXIS=4500,4501 VECTOR2=4501,4502

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

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=t1,t2,metad.bias STRIDE=100 FILE=COLVAR
</pre>{% endraw %}
