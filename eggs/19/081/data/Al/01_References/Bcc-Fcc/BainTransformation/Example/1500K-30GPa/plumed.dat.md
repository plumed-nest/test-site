**Project ID:** [plumID:19.081]({{ '/' | absolute_url }}eggs/19/081/)  
**Source:** Al/01_References/Bcc-Fcc/BainTransformation/Example/1500K-30GPa/plumed.dat  
**Originally used with PLUMED version:** 2.6-dev  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>

energy: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a>

vol: <a href="https://plumed.github.io/doc-master/user-doc/html/_v_o_l_u_m_e.html">VOLUME</a>

cell: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_l_l.html">CELL</a>

lambda1: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=cell.cz FUNC=(x/4-0.378810046139)/(0.296244982844-0.378810046139) PERIODIC=NO
lambda2: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=cell.ax FUNC=(x/4-0.378810046139)/(sqrt(2)*0.296244982844-0.378810046139) PERIODIC=NO

diff: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=lambda1,lambda2 FUNC=(x-y)*(x-y) PERIODIC=NO

<span style="color:blue"># Construct a bias potential using VES</span>
<span style="color:blue">#</span>
<span style="color:blue"># Basis functions</span>

bf1: <a href="https://plumed.github.io/doc-master/user-doc/html/_b_f__l_e_g_e_n_d_r_e.html">BF_LEGENDRE</a> ORDER=20 MINIMUM=-0.5 MAXIMUM=1.5

<span style="color:blue"># Target distribution</span>
td_welltemp: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_d__w_e_l_l_t_e_m_p_e_r_e_d.html">TD_WELLTEMPERED</a> BIASFACTOR=15

<span style="color:blue"># Expansion</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_v_e_s__l_i_n_e_a_r__e_x_p_a_n_s_i_o_n.html">VES_LINEAR_EXPANSION</a> ...
 ARG=lambda1
 BASIS_FUNCTIONS=bf1
 TEMP=1500.0
 GRID_BINS=300
 TARGET_DISTRIBUTION=td_welltemp
 LABEL=b1
... <a href="https://plumed.github.io/doc-master/user-doc/html/_v_e_s__l_i_n_e_a_r__e_x_p_a_n_s_i_o_n.html">VES_LINEAR_EXPANSION</a>

<span style="color:blue"># Optimization algorithm</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_t__d_u_m_m_y.html">OPT_DUMMY</a> ...
  BIAS=b1
  STRIDE=500
  LABEL=o1
  COEFFS_OUTPUT=10
... <a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_t__d_u_m_m_y.html">OPT_DUMMY</a>

wall1: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=lambda1 AT=1. EXP=2 KAPPA=10000. 
wall2: <a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=lambda1 AT=0. EXP=2 KAPPA=10000. 
wall3: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=diff AT=0. EXP=2 KAPPA=10000. 

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=* FILE=COLVAR STRIDE=500
</pre>{% endraw %}
