**Project ID:** [plumID:20.014]({{ '/' | absolute_url }}eggs/20/014/)  
**Source:** PLUMED_input_files/AB42_and_10074_G5/plumed/CVs_drug.dat  
{% raw %}<pre>
<span style="color:blue">#This is the metadynamics CV file for CVs involving the small molecule</span>

<span style="color:blue">#BELOW ARE SOME CVS BETWEEN 14 regions and the ligand based on CA atoms</span>
mol: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> NDX_FILE=../system/index.ndx NDX_GROUP=ligan

<span style="color:blue"># AB42 region 1, res 1-3</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=5,17,27 GROUPB=mol R_0=1.0 NOPBC NLIST NL_CUTOFF=2.0 NL_STRIDE=20 LABEL=reg1
 
<span style="color:blue"># AB42 region 2, res 4-6</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=42,62,86 GROUPB=mol R_0=1.0 NOPBC NLIST NL_CUTOFF=2.0 NL_STRIDE=20 LABEL=reg2

<span style="color:blue"># AB42 region 3, res 7-9</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=103,115,126 GROUPB=mol R_0=1.0 NOPBC NLIST NL_CUTOFF=2.0 NL_STRIDE=20 LABEL=reg3

<span style="color:blue"># AB42 region 4, res 10-12</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=133,154,169 GROUPB=mol R_0=1.0 NOPBC NLIST NL_CUTOFF=2.0 NL_STRIDE=20 LABEL=reg4

<span style="color:blue"># AB42 region 5, res 13-15</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=185,202,219 GROUPB=mol R_0=1.0 NOPBC NLIST NL_CUTOFF=2.0 NL_STRIDE=20 LABEL=reg5

<span style="color:blue"># AB42 region 6, res 16-18</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=236,258,277 GROUPB=mol R_0=1.0 NOPBC NLIST NL_CUTOFF=2.0 NL_STRIDE=20 LABEL=reg6

<span style="color:blue"># AB42 region 7, res 19-21</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=293,313,333 GROUPB=mol R_0=1.0 NOPBC NLIST NL_CUTOFF=2.0 NL_STRIDE=20 LABEL=reg7

<span style="color:blue"># AB42 region 8, res 22-24</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=343,358,370 GROUPB=mol R_0=1.0 NOPBC NLIST NL_CUTOFF=2.0 NL_STRIDE=20 LABEL=reg8

<span style="color:blue"># AB42 region 9, res 25-27</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=386,393,404 GROUPB=mol R_0=1.0 NOPBC NLIST NL_CUTOFF=2.0 NL_STRIDE=20 LABEL=reg9

<span style="color:blue"># AB42 region 10, res 28-30</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=418,440,447 GROUPB=mol R_0=1.0 NOPBC NLIST NL_CUTOFF=2.0 NL_STRIDE=20 LABEL=reg10

<span style="color:blue"># AB42 region 11, res 31-33</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=457,476,495 GROUPB=mol R_0=1.0 NOPBC NLIST NL_CUTOFF=2.0 NL_STRIDE=20 LABEL=reg11

<span style="color:blue"># AB42 region 12, res 34-36</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=502,521,538 GROUPB=mol R_0=1.0 NOPBC NLIST NL_CUTOFF=2.0 NL_STRIDE=20 LABEL=reg12

<span style="color:blue"># AB42 region 13, res 37-39</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=554,561,568 GROUPB=mol R_0=1.0 NOPBC NLIST NL_CUTOFF=2.0 NL_STRIDE=20 LABEL=reg13

<span style="color:blue"># AB42 region 14, res 40-42</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=584,600,619 GROUPB=mol R_0=1.0 NOPBC NLIST NL_CUTOFF=2.0 NL_STRIDE=20 LABEL=reg14

<span style="color:blue"># Ligand soft dihedrals</span>
ligtor1: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=641,628,629,640 NOPBC
ligtor2: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=642,641,628,629 NOPBC
ligtor3: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=634,635,636,637 NOPBC
ligtor4: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=641,646,647,648 NOPBC

</pre>{% endraw %}
