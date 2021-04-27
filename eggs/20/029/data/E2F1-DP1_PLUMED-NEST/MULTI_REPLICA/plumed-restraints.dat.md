**Project ID:** [plumID:20.029]({{ '/' | absolute_url }}eggs/20/029/)  
**Source:** E2F1-DP1_PLUMED-NEST/MULTI_REPLICA/plumed-restraints.dat  
{% raw %}<pre>
<span style="color:blue"># RESTRAIN DNA</span>

A466_T437_H1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> NOPBC ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N6-466</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">O4-437</a> 
A466_T437_H2: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> NOPBC ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N1-466</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N3-437</a> 

G452_C451_H1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> NOPBC ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N2-452</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">O2-451</a> 
G452_C451_H2: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> NOPBC ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N1-452</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N3-451</a> 
G452_C451_H3: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> NOPBC ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">O6-452</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N4-451</a> 

<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=A466_T437_H1,A466_T437_H2,G452_C451_H1,G452_C451_H2,G452_C451_H3 AT=0.29,0.29,0.29,0.29,0.29  KAPPA=2000.0,2000.0,2000.0,2000.0,2000.0 LABEL=RESTRAINT_DNA


<span style="color:blue"># RESTRAIN ARGININE HBONDS</span>
<span style="color:blue"># see Genes Dev. 1999 Mar 15; 13(6): 666–674 [Reference paper for pdb: 1cf7]. Figure 4.</span>
<span style="color:blue"># consider common recognition sequence: C442-C445/G458-G462</span>

R46_DG458: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> NOPBC ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">NE-46</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">O6-458</a>
R47_DG444: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> NOPBC ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">NH2-47</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">O6-444</a>
R250_DG442: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> NOPBC ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">NE-250</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">O6-442</a>
R251_DG460: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> NOPBC ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">NH2-251</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">O6-460</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=R46_DG458,R47_DG444,R250_DG442,R251_DG460 AT=0.29,0.29,0.29,0.29  KAPPA=2000.0,2000.0,2000.0,2000.0 LABEL=RESTRAINT_ARG



<span style="color:blue"># PRINT</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=RESTRAINT_DNA.bias,RESTRAINT_ARG.bias STRIDE=2000 FILE=RESTRAINTS
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=A466_T437_H1,A466_T437_H2,G452_C451_H1,G452_C451_H2,G452_C451_H3,R46_DG458,R47_DG444,R250_DG442,R251_DG460 STRIDE=2000 FILE=HBONDS

</pre>{% endraw %}
