**Project ID:** [plumID:19.077]({{ '/' | absolute_url }}eggs/19/077/)  
**Source:** TBP/6mer_NH.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](6mer_NH.dat.plumed.stdout.txt.zip) - [stderr](6mer_NH.dat.plumed.stderr)  
**Master:** [raw zipped stdout](6mer_NH.dat.plumed_master.stdout.txt.zip) - [stderr](6mer_NH.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">MOLINFO</a> MOLTYPE=protein STRUCTURE=6mer.pdb

<span style="color:blue">#PEPTIDE DISTANCE#</span>
pep1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=1-104
d1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=2383,pep1 COMPONENTS NOPBC

<span style="color:blue">##radius of gyration##</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_g_y_r_a_t_i_o_n.html">GYRATION</a> TYPE=RADIUS ATOMS=5,29,51,72,84,96 LABEL=rg

<span style="color:blue">##ENERGY##</span>
ene: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
ARG=ene
PACE=5000 BIASFACTOR=10.0 HEIGHT=2.00
SIGMA=280
GRID_MIN=-5500000.000000
GRID_MAX=-5000000.000000
FILE=HILLS
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

wall1: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=d1.z AT=4.0 KAPPA=1500

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
ARG=d1.z,rg
PACE=250 BIASFACTOR=15.0 HEIGHT=2.0
SIGMA=0.01,0.02
GRID_MIN=0.0,0.0
GRID_MAX=20.0,10.0
FILE=HILLS_MTD
LABEL=cvbias
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=d1.z,rg STRIDE=500 FILE=COLVAR
</pre>{% endraw %}
