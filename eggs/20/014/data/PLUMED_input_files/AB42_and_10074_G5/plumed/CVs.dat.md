**Project ID:** [plumID:20.014]({{ '/' | absolute_url }}eggs/20/014/)  
**Source:** PLUMED_input_files/AB42_and_10074_G5/plumed/CVs.dat  
{% raw %}<pre>
<span style="color:blue">#This is the metadynamics CV file for CVs on the peptide</span>

<span style="color:blue">#CV1 alpha helix</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_r_m_s_d.html">ALPHARMSD</a> RESIDUES=1-42 TYPE=DRMSD LESS_THAN={RATIONAL R_0=0.08 NN=8 MM=12} LABEL=helix

<span style="color:blue">#CV2 sum parallel and anti-parallel beta-content</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_a_r_a_b_e_t_a_r_m_s_d.html">PARABETARMSD</a> RESIDUES=1-42 TYPE=DRMSD LESS_THAN={RATIONAL R_0=0.08 NN=8 MM=12} LABEL=par
<a href="https://plumed.github.io/doc-master/user-doc/html/_a_n_t_i_b_e_t_a_r_m_s_d.html">ANTIBETARMSD</a> RESIDUES=1-42 TYPE=DRMSD LESS_THAN={RATIONAL R_0=0.08 NN=8 MM=12} LABEL=anti
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=par.lessthan,anti.lessthan PERIODIC=NO LABEL=beta

<span style="color:blue">#CV3 radius of gyration</span>
ca: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=5,17,27,42,62,86,103,115,126,133,154,169,185,202,219,236,258,277,293,313,333,343,358,370,386,393,404,418,440,447,457,476,495,502,521,538,554,561,568,584,600,619
rgyr: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_y_r_a_t_i_o_n.html">GYRATION</a> ATOMS=ca NOPBC

<span style="color:blue">#CV4 contacts between hydrophobic residues calculated as the number of Cbeta carbon couples closer than 0.6 nm </span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=19,44,171,260,279,295,315,335,372,449,459,478,504,523,540,570,586,602,621 R_0=0.6 NOPBC NLIST NL_CUTOFF=1.0 NL_STRIDE=20 LABEL=hydro

<span style="color:blue">#CV5 the number of salt-bridges calculated as the number of couples of heavy atoms from the charged group closer than 0.6 nm </span>
<span style="color:blue">#GROUP A is all the heavy atoms from RCOO- group of aspartic acids and glutamic acids </span>
<span style="color:blue">#GROUP B is all the heavy atoms from RHN3+ from lysines or (RNHC(NH2)2+) of arginines</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=10,11,12,35,36,37,108,109,110,162,163,164,351,352,353,363,364,365 GROUPB=75,76,77,78,79,80,81,250,251,252,253,432,433,434,435 R_0=0.6 NOPBC NLIST NL_CUTOFF=1.0 NL_STRIDE=20 LABEL=salt

<span style="color:blue">#CV6 correlation between consecutive psi torsion angles.</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_h_c_o_r.html">DIHCOR</a> ...
ATOMS1=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-1</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-2</a>
ATOMS2=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-2</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-3</a>
ATOMS3=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-3</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-4</a>
ATOMS4=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-4</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-5</a>
ATOMS5=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-5</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-6</a>
ATOMS6=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-6</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-7</a>
ATOMS7=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-7</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-8</a>
ATOMS8=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-8</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-9</a>
ATOMS9=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-9</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-10</a>
ATOMS10=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-10</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-11</a>
ATOMS11=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-11</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-12</a>
ATOMS12=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-12</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-13</a>
ATOMS13=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-13</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-14</a>
ATOMS14=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-14</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-15</a>
ATOMS15=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-15</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-16</a>
ATOMS16=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-16</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-17</a>
ATOMS17=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-17</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-18</a>
ATOMS18=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-18</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-19</a>
ATOMS19=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-19</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-20</a>
ATOMS20=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-20</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-21</a>
ATOMS21=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-21</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-22</a>
ATOMS22=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-22</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-23</a>
ATOMS23=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-23</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-24</a>
ATOMS24=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-24</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-25</a>
ATOMS25=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-25</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-26</a>
ATOMS26=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-26</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-27</a>
ATOMS27=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-27</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-28</a>
ATOMS28=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-28</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-29</a>
ATOMS29=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-29</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-30</a>
ATOMS30=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-30</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-31</a>
ATOMS31=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-31</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-32</a>
ATOMS32=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-32</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-33</a>
ATOMS33=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-33</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-34</a>
ATOMS34=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-34</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-35</a>
ATOMS35=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-35</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-36</a>
ATOMS36=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-36</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-37</a>
ATOMS37=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-37</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-38</a>
ATOMS38=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-38</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-39</a>
ATOMS39=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-39</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-40</a>
ATOMS40=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-40</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-41</a>
LABEL=dihcor
NOPBC
... <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_h_c_o_r.html">DIHCOR</a>

</pre>{% endraw %}
