**Project ID:** [plumID:20.019]({{ '/' | absolute_url }}eggs/20/019/)  
**Source:** Crystal-Energy-Landscapes/plumed.dat  
**Originally used with PLUMED version:** 2.3-mod  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue">#RESTART</span>

<span style="color:blue"># Avoid too skewed triclinic box</span>
cell: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_l_l.html">CELL</a>

bx: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=cell.bx,cell.ax FUNC=abs(x)-0.5*y PERIODIC=NO
cx: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=cell.cx,cell.ax FUNC=abs(x)-0.5*y PERIODIC=NO
cy: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=cell.cy,cell.by FUNC=abs(x)-0.5*y PERIODIC=NO

<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=bx,cx,cy AT=0.0,0.0,0.0 KAPPA=100000.0,100000.0,100000.0 EXP=2,2,2 EPS=1,1,1 OFFSET=0.3,0.3,0.3 LABEL=uwall

<span style="color:blue"># CV1 - Density</span>
vol: <a href="https://plumed.github.io/doc-master/user-doc/html/_v_o_l_u_m_e.html">VOLUME</a>
density: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=vol FUNC=400.0/x*1.66054*118.0 PERIODIC=NO

<span style="color:blue"># Constraints to force the system to stay in the grid </span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=density AT=1800 KAPPA=100.0 EXP=2 EPS=1 OFFSET=25 LABEL=ulimit
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=density AT=1200 KAPPA=100.0 EXP=2 EPS=1 OFFSET=25 LABEL=llimit

<span style="color:blue">#CV2 - Potential Energy </span>
ene_pot: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a>
elatt: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=ene_pot,uwall.bias,ulimit.bias,llimit.bias VAR=a,b,c,d FUNC=(a-b-c-d)/400.0+350.507 PERIODIC=NO

<span style="color:blue"># WTmetaD Parameters</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
LABEL=metad
ARG=elatt,density
PACE=1000
HEIGHT=2.0
SIGMA=2.0,20.0
TEMP=300
BIASFACTOR=200.0
GRID_MIN=-120,1200
GRID_MAX=400,1800
GRID_BIN=5200,600
<span style="color:blue"># PLUMED 2.3 syntax</span>
<span style="color:blue"># REWEIGHTING_NGRID=5200,600</span>
<span style="color:blue"># REWEIGHTING_NHILLS=10</span>
<span style="color:blue"># PLUMED 2.4 syntax</span>
CALC_RCT
<span style="color:blue"># RCT_USTRIDE=10</span>
FILE=HILLS
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=100 ARG=elatt,density,metad.bias,metad.rbias,metad.rct,ulimit.bias,llimit.bias,uwall.bias FILE=COLVAR


</pre>{% endraw %}
