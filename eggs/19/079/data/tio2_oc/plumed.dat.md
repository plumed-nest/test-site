**Project ID:** [plumID:19.079]({{ '/' | absolute_url }}eggs/19/079/)  
**Source:** tio2_oc/plumed.dat  
**Originally used with PLUMED version:** 2.4.2  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">MOLINFO</a> MOLTYPE=protein STRUCTURE=conf.pdb

ene: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a>

<span style="color:blue">##radius of gyration##</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_g_y_r_a_t_i_o_n.html">GYRATION</a> TYPE=RADIUS ATOMS=5,28,40,54,66,85,104,116,140,164,181,197,208,225,244 LABEL=rg

<span style="color:blue">#PEPTIDE</span>
pep1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=1-256
ref: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=2801
d1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=ref,pep1 COMPONENTS NOPBC

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
ARG=ene
PACE=2500 BIASFACTOR=10.0 HEIGHT=2.0
SIGMA=290
GRID_MIN=-5600000.000000
GRID_MAX=-5300000.000000
FILE=HILLS
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<span style="color:blue">#MTD</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
ARG=d1.z,rg
PACE=500 BIASFACTOR=10.0 HEIGHT=2.0
SIGMA=0.01,0.02
GRID_MIN=0.0,0.0
GRID_MAX=10.0,10.0
FILE=HILLS_MTD
LABEL=cvbias
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>


<span style="color:blue">## wall </span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=d1.z AT=4.5 KAPPA=50000 LABEL=uwall

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=* STRIDE=500 FILE=COLVAR


</pre>{% endraw %}
