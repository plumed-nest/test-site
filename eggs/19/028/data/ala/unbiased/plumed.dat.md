**Project ID:** [plumID:19.028]({{ '/' | absolute_url }}eggs/19/028/)  
**Source:** ala/unbiased/plumed.dat  
**Originally used with PLUMED version:** 2.3  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
phi:   <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=5,7,9,15       NOPBC
psi:   <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=7,9,15,17      NOPBC

<a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_b_e_t_a.html">ALPHABETA</a> ATOMS1=5,7,9,15 REFERENCE=0 LABEL=ab1_phi
<a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_b_e_t_a.html">ALPHABETA</a> ATOMS1=5,7,9,15 REFERENCE=-1.5708 LABEL=ab2_phi
<a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_b_e_t_a.html">ALPHABETA</a> ATOMS1=7,9,15,17 REFERENCE=0 LABEL=ab1_psi
<a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_b_e_t_a.html">ALPHABETA</a> ATOMS1=7,9,15,17 REFERENCE=-1.5708 LABEL=ab2_psi


<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ...
LABEL=cos_phi  ARG=ab1_phi COEFFICIENTS=2.0 PARAMETERS=0.5 PERIODIC=NO
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ...
LABEL=sin_phi  ARG=ab2_phi COEFFICIENTS=-2.0 PARAMETERS=0.5 PERIODIC=NO
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ...
LABEL=cos_psi  ARG=ab1_psi COEFFICIENTS=2.0 PARAMETERS=0.5 PERIODIC=NO
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ...
LABEL=sin_psi  ARG=ab2_psi COEFFICIENTS=-2.0 PARAMETERS=0.5 PERIODIC=NO
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a>



<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=cos_phi,sin_phi,cos_psi,sin_psi,phi,psi STRIDE=1 FILE=ala_T300_1





</pre>{% endraw %}
