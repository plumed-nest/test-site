**Project ID:** [plumID:19.012]({{ '/' | absolute_url }}eggs/19/012/)  
**Source:** Protein-DNA/plumed-restr.dat  
{% raw %}<pre>
<span style="color:blue">#### RESTR ON HBONDS ####</span>
A1T76_H1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N6-1</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">O4-76</a>
A1T76_H2: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N1-1</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N3-76</a>

A2T75_H1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N6-2</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">O4-75</a>
A2T75_H2: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N1-2</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N3-75</a>


A38T39_H1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N6-38</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">O4-39</a>
A38T39_H2: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N1-38</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N3-39</a>

A37T40_H1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N6-37</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">O4-40</a>
A37T40_H2: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N1-37</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N3-40</a>


<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=A1T76_H1,A1T76_H2,A2T75_H1,A2T75_H2,A38T39_H1,A38T39_H2,A37T40_H1,A37T40_H2 AT=0.3,0.3,0.3,0.3,0.3,0.3,0.3,0.3 KAPPA=1000.0,1000.0,1000.0,1000.0,1000.0,1000.0,1000.0,1000.0 LABEL=restraint

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=restraint.bias STRIDE=1000 FILE=RESTRAINTS
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=A1T76_H1,A1T76_H2,A2T75_H1,A2T75_H2,A38T39_H1,A38T39_H2,A37T40_H1,A37T40_H2 STRIDE=1000 FILE=HBONDS
</pre>{% endraw %}
