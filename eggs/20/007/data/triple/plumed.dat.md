**Project ID:** [plumID:20.007]({{ '/' | absolute_url }}eggs/20/007/)  
**Source:** triple/plumed.dat  
**Originally used with PLUMED version:** 2.4.2  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># The commented out lines are the original implementation. They have been altered to be compatible with newer PLUMED versions.</span>

d1775_2417: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1775,2417
d1739_1755: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1739,1755
d1795_453: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1795,453
d1809_1823: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1809,1823
d1823_1834: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1823,1834

loop_dist: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1772,1822
psi: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=1773,1775,1791,1793

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ...
LABEL=rc1 ARG=d1775_2417,d1739_1755,d1795_453,d1809_1823,d1823_1834 COEFFICIENTS=0.41801464557647705,-0.04167945683002472,0.8776463866233826,-0.21770134568214417,0.07661298662424088 PERIODIC=NO
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ...
LABEL=rc2 ARG=d1775_2417,d1739_1755,d1795_453,d1809_1823,d1823_1834 COEFFICIENTS=-0.7833237051963806,0.06509189307689667,0.42879876494407654,0.0804712250828743,-0.43797600269317627 PERIODIC=NO
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
BIASFACTOR=10
TEMP=300
ARG=rc1,rc2
SIGMA=0.092,0.069
HEIGHT=1.5
PACE=500
LABEL=metad
<span style="color:blue">#GRID_MIN=0.0,-6.0</span>
<span style="color:blue">#GRID_MAX=8.0,2.0</span>
<span style="color:blue">#GRID_BIN=150,150</span>
<span style="color:blue">#REWEIGHTING_NGRID=150,150</span>
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<span style="color:blue">#PRINT ARG=d1775_2417,d1739_1755,d1795_453,d1809_1823,d1823_1834,loop_dist,psi,rc1,rc2,metad.bias,metad.rbias STRIDE=1 FILE=BIASED_COLVAR</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=d1775_2417,d1739_1755,d1795_453,d1809_1823,d1823_1834,loop_dist,psi,rc1,rc2,metad.bias STRIDE=1 FILE=BIASED_COLVAR
</pre>{% endraw %}
