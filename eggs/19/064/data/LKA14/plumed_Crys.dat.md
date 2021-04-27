**Project ID:** [plumID:19.064]({{ '/' | absolute_url }}eggs/19/064/)  
**Source:** LKA14/plumed_Crys.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed_Crys.dat.plumed.stdout.txt.zip) - [stderr](plumed_Crys.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_Crys.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_Crys.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">MOLINFO</a> MOLTYPE=protein STRUCTURE=conf.pdb

<span style="color:blue">#PEPTIDE DISTANCE#</span>
pep1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=1-287
d1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=6205,pep1 COMPONENTS NOPBC

<span style="color:blue">##radius of gyration##</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_g_y_r_a_t_i_o_n.html">GYRATION</a> TYPE=RADIUS ATOMS=5,24,46,68,87,106,128,147,166,188,210,229,248,270 LABEL=rg

<span style="color:blue">##ENERGY##</span>
ene: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a>


<span style="color:blue">##Blocks##</span>
B1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=1-84
d2: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=6205,B1 COMPONENTS 
B2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=85-210
d3: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=6205,B2 COMPONENTS 
B3: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=211-287
d4: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=6205,B3 COMPONENTS 


<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
ARG=ene
PACE=2500 BIASFACTOR=15.0 HEIGHT=2.0
SIGMA=300
GRID_MIN=1300000.00000
GRID_MAX=1500000.00000
FILE=HILLS
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

wall1: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=d1.z,d2.z,d3.z,d4.z AT=8.0,8.0,8.0,8.0 KAPPA=1500,1500,1500,1500 

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
ARG=d1.z,rg
PACE=500 BIASFACTOR=15.0 HEIGHT=2.0
SIGMA=0.01,0.02
GRID_MIN=0.0,0.0
GRID_MAX=10.0,20.0
FILE=HILLS_MTD
LABEL=cvbias
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=d1.z,rg,ene,cvbias.bias STRIDE=500 FILE=COLVAR
</pre>{% endraw %}
