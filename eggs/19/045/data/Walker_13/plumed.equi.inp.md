**Project ID:** [plumID:19.045]({{ '/' | absolute_url }}eggs/19/045/)  
**Source:** Walker_13/plumed.equi.inp  
**Originally used with PLUMED version:** 2.3  
**Stable:** [raw zipped stdout](plumed.equi.inp.plumed.stdout.txt.zip) - [stderr](plumed.equi.inp.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.equi.inp.plumed_master.stdout.txt.zip) - [stderr](plumed.equi.inp.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># Restart command</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>

<span style="color:blue"># Units</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> ENERGY=eV LENGTH=A TIME=ps

<span style="color:blue"># Water oxygens group</span>
ow: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=25205-60049:3

<span style="color:blue"># Position of the adsorbate</span>
p1: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_o_s_i_t_i_o_n.html">POSITION</a> ATOM=1 NOPBC

<span style="color:blue"># cation-water coordination no</span>
c1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=13365 GROUPB=ow D_0=2.1 R_0=1.0 NN=4 MM=10 NLIST NL_CUTOFF=7 NL_STRIDE=20

<span style="color:blue"># Walls free energy - position</span>
lwallp1x: <a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=p1.x AT=53.0 KAPPA=1  EXP=2 EPS=1 OFFSET=0
uwallp1x: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=p1.x AT=72.0 KAPPA=1  EXP=2 EPS=1 OFFSET=0
lwallp1y: <a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=p1.y AT=32.5 KAPPA=1  EXP=2 EPS=1 OFFSET=0
uwallp1y: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=p1.y AT=39.0 KAPPA=1  EXP=2 EPS=1 OFFSET=0
uwallp1z: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=p1.z AT=50.0 KAPPA=1  EXP=4 EPS=1 OFFSET=0

<span style="color:blue"># Metadynamics</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
  LABEL=mtd
  ARG=p1.x,p1.z,c1
  SIGMA=0.2,0.2,0.2
  PACE=1000000
  HEIGHT=0.026
  BIASFACTOR=10 TEMP=300
  WALKERS_DIR=../HILLS_DIR WALKERS_RSTRIDE=500 WALKERS_N=30 WALKERS_ID=13
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<span style="color:blue"># Print CV</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ...
  ARG=p1.x,p1.y,p1.z,c1,lwallp1x.bias,uwallp1x.bias,lwallp1y.bias,uwallp1y.bias,uwallp1z.bias
  FILE=COLVAR 
  STRIDE=1000
... <a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a>
<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=1000

</pre>{% endraw %}
