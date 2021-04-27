**Project ID:** [plumID:20.034]({{ '/' | absolute_url }}eggs/20/034/)  
**Source:** plumed_SL5A.dat  
**Originally used with PLUMED version:** 2.5.3  
**Stable:** [raw zipped stdout](plumed_SL5A.dat.plumed.stdout.txt.zip) - [stderr](plumed_SL5A.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_SL5A.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_SL5A.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">MOLINFO</a> STRUCTURE=SL5a_ext_gmx.pdb MOLTYPE=rna


ermsd0_p1: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_r_m_s_d.html">ERMSD</a> REFERENCE=SL5a_H1_template.pdb ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-1</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-2</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-3</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-4</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-5</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-6</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-7</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-27</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-28</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-29</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-30</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-31</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-32</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-33</a>
ermsd1_p1: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_r_m_s_d.html">ERMSD</a> REFERENCE=SL5a_H1_template.pdb ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-1</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-2</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-3</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-4</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-5</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-6</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-7</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-27</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-28</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-29</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-30</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-31</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-32</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-33</a> CUTOFF=12

ermsd0_p2: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_r_m_s_d.html">ERMSD</a> REFERENCE=SL5a_H2_template.pdb ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-9</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-10</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-11</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-12</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-13</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-20</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-21</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-22</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-23</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-24</a>
ermsd1_p2: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_r_m_s_d.html">ERMSD</a> REFERENCE=SL5a_H2_template.pdb ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-9</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-10</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-11</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-12</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-13</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-20</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-21</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-22</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-23</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-24</a> CUTOFF=12


<span style="color:blue"># HELIX1 </span>
c1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-1</a>
c2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-2</a>
c3: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-3</a>
c4: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-4</a>
c5: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-5</a>
c6: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-6</a>
c7: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-7</a>

c27: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-27</a>
c28: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-28</a>
c29: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-29</a>
c30: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-30</a>
c31: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-31</a>
c32: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-32</a>
c33: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-33</a>

<span style="color:blue"># HELIX2</span>
c9: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-9</a>
c10: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-10</a>
c11: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-11</a>
c12: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-12</a>
c13: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-13</a>

c20: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-20</a>
c21: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-21</a>
c22: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-22</a>
c23: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-23</a>
c24: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-24</a>


dp1_1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=c1,c33
dp1_2: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=c2,c32
dp1_3: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=c3,c31
dp1_4: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=c4,c30
dp1_5: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=c5,c29
dp1_6: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=c6,c28
dp1_7: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=c7,c27

dp2_1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=c9,c24
dp2_2: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=c10,c23
dp2_3: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=c11,c22
dp2_4: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=c12,c21
dp2_5: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=c13,c20


<span style="color:blue"># other </span>
c8: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-8</a>
c14: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-14</a>
c15: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-15</a>
c18: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-18</a>
c19: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-19</a>
c25: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-25</a>
c26: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">lcs-26</a>

D8_25: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=c8,c25
D8_26: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=c8,c26
D14_19: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=c14,c19
D15_18: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=c15,c18

chi: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi-18</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_a_b_m_d.html">ABMD</a> ... 
ARG=ermsd1_p1,ermsd1_p2
KAPPA=1,1
TO=1,1 
LABEL=qq 
... <a href="https://plumed.github.io/doc-master/user-doc/html/_a_b_m_d.html">ABMD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FILE=ERMSD_YYY ARG=ermsd0_p1,ermsd0_p2,ermsd1_p1,ermsd1_p2,qq.bias STRIDE=5000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FILE=DIST_YYY ARG=dp1_1,dp1_2,dp1_3,dp1_4,dp1_5,dp1_6,dp1_7,dp2_1,dp2_2,dp2_3,dp2_4,dp2_5,D8_25,D8_26,D14_19,D15_18,chi STRIDE=5000

</pre>{% endraw %}
