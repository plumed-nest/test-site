**Project ID:** [plumID:19.015]({{ '/' | absolute_url }}eggs/19/015/)  
**Source:** surface/100_polar/plumed_kinetics.dat  
**Originally used with PLUMED version:** 2.3  
**Stable:** [raw zipped stdout](plumed_kinetics.dat.plumed.stdout.txt.zip) - [stderr](plumed_kinetics.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_kinetics.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_kinetics.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue">#######IBU 28##########</span>


<span style="color:blue">#torsion1 between vector C1,C2 and C10,C11 with axis C2,C10</span>
t1: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=895,894 AXIS=895,903 VECTOR2=903,904

<span style="color:blue">#torsion2 between vector C7,C10 and C11,C12 with axis C10,C11</span>
t2: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=903,900 AXIS=903,904 VECTOR2=904,905

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
  BASIN_LL1=-3.15,-3.15
  BASIN_UL1=-2.3,-2.85
  BASIN_LL2=-3.15,3.13
  BASIN_UL2=-2.3,3.15
  BASIN_LL3=3.13,3.13
  BASIN_UL3=3.15,3.15
  BASIN_LL4=3.13,-3.15
  BASIN_UL4=3.15,-2.85
  
<span style="color:blue">#C2 basin</span>
   BASIN_LL5=-2.7,-1.3
   BASIN_UL5=-1.9,-1.0

<span style="color:blue">#C3 basin</span>
   BASIN_LL6=-2.7,0.9
   BASIN_UL6=-2.3,1.2

<span style="color:blue">#C4 basin</span>
   BASIN_LL7=-0.1,-3.15
   BASIN_UL7=0.85,-2.85
   BASIN_LL8=-0.1,3.13
   BASIN_UL8=0.85,3.15

<span style="color:blue">#C5 basin</span>
<span style="color:blue">#   BASIN_LL5=0.5,-1.3</span>
<span style="color:blue">#   BASIN_UL5=1.3,-1.0</span>

<span style="color:blue">#C6 basin</span>
   BASIN_LL9=0.5,0.9
   BASIN_UL9=1.0,1.2
  
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_m_i_t_t_o_r.html">COMMITTOR</a>


<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=t1,t2,metad.bias STRIDE=10 FILE=COLVAR
</pre>{% endraw %}
