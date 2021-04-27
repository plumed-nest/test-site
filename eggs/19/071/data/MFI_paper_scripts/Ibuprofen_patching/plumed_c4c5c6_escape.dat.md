**Project ID:** [plumID:19.071]({{ '/' | absolute_url }}eggs/19/071/)  
**Source:** MFI_paper_scripts/Ibuprofen_patching/plumed_c4c5c6_escape.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed_c4c5c6_escape.dat.plumed.stdout.txt.zip) - [stderr](plumed_c4c5c6_escape.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_c4c5c6_escape.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_c4c5c6_escape.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue">#torsion1 between vector C1,C2 and C10,C11 with axis C2,C10</span>
t1: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5911,5910 AXIS=5919,5911 VECTOR2=5919,5920

<span style="color:blue">#torsion2 between vector C7,C10 and C11,C12 with axis C10,C11</span>
t2: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=5919,5916 AXIS=5920,5919 VECTOR2=5920,5921

<span style="color:blue">#metadynamics</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
ARG=t1,t2
SIGMA=0.1,0.1
HEIGHT=0.24
PACE=1000
BIASFACTOR=5.0
TEMP=300.0
LABEL=metad
FILE=HILLS
GRID_MIN=-pi,-pi
GRID_MAX=pi,pi
GRID_BIN=350,350
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>


<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_m_i_t_t_o_r.html">COMMITTOR</a> ...
  ARG=t1,t2

<span style="color:blue">#C1 basin</span>
  BASIN_LL1=-pi,-pi
  BASIN_UL1=-2.93,-2.7
  BASIN_LL2=-pi,3.13
  BASIN_UL2=-3.13,pi
  BASIN_LL3=3.13,3.13
  BASIN_UL3=pi,pi
  BASIN_LL4=2.6,-pi
  BASIN_UL4=pi,-2.6
  
<span style="color:blue">#C2 basin</span>
  BASIN_LL5=-2.7,-1.15
  BASIN_UL5=-1.8,-0.6

<span style="color:blue">#C3 basin</span>
   BASIN_LL6=-pi,0.6
   BASIN_UL6=-2.9,1.1
   BASIN_LL7=2.9,0.6
   BASIN_UL7=pi,1.1

... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_m_i_t_t_o_r.html">COMMITTOR</a>


<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=t1,t2,metad.bias STRIDE=10 FILE=COLVAR
</pre>{% endraw %}
