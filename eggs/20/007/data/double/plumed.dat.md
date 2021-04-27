**Project ID:** [plumID:20.007]({{ '/' | absolute_url }}eggs/20/007/)  
**Source:** double/plumed.dat  
**Originally used with PLUMED version:** 2.4.2  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=1-2640

d686_1739: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=686,1739
d1834_1853: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1834,1853
d1732_1739: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1732,1739
d1755_1765: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1755,1765
d1823_1834: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1823,1834
d1765_1823: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1765,1823
d1809_1877: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1809,1877
d1187_1739: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1187,1739
d1877_1894: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1877,1894
d1853_1947: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1853,1947

psi: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=1773,1775,1791,1793
dist: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1772,1822 <span style="color:blue"># A1130-S117H</span>

rmsd: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_m_s_d.html">RMSD</a> REFERENCE=rmsd.pdb TYPE=OPTIMAL

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ...
LABEL=rc1 
ARG=d686_1739,d1834_1853,d1732_1739,d1755_1765,d1823_1834,d1765_1823,d1809_1877,d1187_1739,d1877_1894,d1853_1947 
COEFFICIENTS=0.135,-0.343,0.432,0.348,-0.377,0.162,-0.138,0.294,0.527,-0.070
PERIODIC=NO
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ...
LABEL=rc2 
ARG=d686_1739,d1834_1853,d1732_1739,d1755_1765,d1823_1834,d1765_1823,d1809_1877,d1187_1739,d1877_1894,d1853_1947 
COEFFICIENTS=-0.075,-0.226,0.758,0.083,-0.326,0.247,-0.173,-0.137,0.194,0.330
PERIODIC=NO
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a>


<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
LABEL=metad
ARG=rc1,rc2
PACE=500
HEIGHT=1.5
SIGMA=0.021,0.014
BIASFACTOR=10.0
TEMP=300.0
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=rmsd AT=.4 KAPPA=10000.0 EXP=4 EPS=1 OFFSET=0 LABEL=uwall

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=d686_1739,d1834_1853,d1732_1739,d1755_1765,d1823_1834,d1765_1823,d1809_1877,d1187_1739,d1877_1894,d1853_1947,rc1,rc2,psi,dist,rmsd,uwall.bias,metad.bias STRIDE=1 FILE=COLVAR_full
</pre>{% endraw %}
