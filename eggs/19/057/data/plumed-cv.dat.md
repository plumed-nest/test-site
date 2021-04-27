**Project ID:** [plumID:19.057]({{ '/' | absolute_url }}eggs/19/057/)  
**Source:** plumed-cv.dat  
{% raw %}<pre>
<span style="color:blue">#--------------------------------------------------------------------------------------------------------------------------------------------------</span>
<span style="color:blue">#CONTACT</span>

<span style="color:blue">#DEFINE GROUPS</span>
hydroph1: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> NDX_FILE=index.ndx NDX_GROUP=SC-CARBON_HYDROPH_A-G-I-L-V-P-F-M-W_&_Protein_&_r_1-76	
hydroph2: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> NDX_FILE=index.ndx NDX_GROUP=SC-CARBON_HYDROPH_A-G-I-L-V-P-F-M-W_&_Protein_&_r_77-152
polar1: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> NDX_FILE=index.ndx NDX_GROUP=ALL_donor-acceptor_&_Protein_&_r_1-76
polar2: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> NDX_FILE=index.ndx NDX_GROUP=ALL_donor-acceptor_&_Protein_&_r_77-152

<span style="color:blue"># COORDINATION</span>
hyd: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=hydroph1 GROUPB=hydroph2 SWITCH={RATIONAL R_0=0.5 D_MAX=2.6 NN=6 MM=10} NLIST NL_CUTOFF=2.6 NL_STRIDE=20 NOPBC	
pol: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n.html">COORDINATION</a> GROUPA=polar1 GROUPB=polar2 SWITCH={RATIONAL R_0=0.5 D_MAX=1.2 NN=6 MM=12} NLIST NL_CUTOFF=1.2 NL_STRIDE=20 NOPBC


<span style="color:blue">#--------------------------------------------------------------------------------------------------------------------------------------------------</span>
<span style="color:blue">#DIHEDRALS</span>

<span style="color:blue"># DIHEDRAL linker</span>
psi75ATM: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=1219,1221,1224,1226
phi76ATM: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=1224,1226,1228,1231
psi76ATM: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=1226,1228,1231,2246
lypglpATM:  <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=1231,2246,2243,2240
lyp-chi4ATM: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=2246,2243,2240,2237
lyp-chi3ATM: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=2243,2240,2237,2234
lyp-chi2ATM: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=2240,2237,2234,2232
lyp-chi1ATM: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=2237,2234,2232,2230

<span style="color:blue"># CENTER OF MASS FOR GLOBAL DIH CALCULATIONS</span>
al1ATM: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> NDX_FILE=index.ndx NDX_GROUP=C-alpha_&_r_24-32
al2ATM: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> NDX_FILE=index.ndx NDX_GROUP=C-alpha_&_r_100-108
bb1ATM: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> NDX_FILE=index.ndx NDX_GROUP=r_42-45_r_68-71_&_C-alpha
bb2ATM: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> NDX_FILE=index.ndx NDX_GROUP=r_118-121_r_144-147_&_C-alpha
ba1ATM: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> NDX_FILE=index.ndx NDX_GROUP=r_3-6_r_13-16_&_C-alpha
cm1ATM: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> NDX_FILE=index.ndx NDX_GROUP=C-alpha_&_r_24-32_r_42-45_r_68-71_&_C-alpha_r_3-6_r_13-16_&_C-alpha
cm2ATM: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> NDX_FILE=index.ndx NDX_GROUP=C-alpha_&_r_100-108_r_118-121_r_144-147_&_C-alpha_r_78-82_r_89-92_&_C-alpha
cmlinATM: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> NDX_FILE=index.ndx NDX_GROUP=r_71-76_r_139_&_C-alpha

al1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=al1ATM NOPBC
al2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=al2ATM NOPBC
bb1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=bb1ATM NOPBC 
bb2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=bb2ATM NOPBC
ba1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=ba1ATM NOPBC	
cm1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=cm1ATM NOPBC 
cm2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=cm2ATM NOPBC 
cmlin: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=cmlinATM NOPBC 

angCM: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_n_g_l_e.html">ANGLE</a> ATOMS=cm1,cmlin,cm2 NOPBC
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=angCM VAR=x FUNC=0.5+0.5*cos(x) PERIODIC=NO LABEL=ab18

<a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_b_e_t_a.html">ALPHABETA</a> ...
	ATOMS1=al1,bb1,bb2,al2 COEFFICIENT1=0.6853644995570499
	ATOMS2=bb1,ba1,al1,bb2 COEFFICIENT2=0.48086151944511846
	ATOMS3=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">phi-72</a> COEFFICIENT3=0.003292645978257468
	ATOMS4=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-72</a> COEFFICIENT4=0.06978956636126267
	ATOMS5=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">phi-73</a> COEFFICIENT5=-0.1857627096512617
	ATOMS6=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-73</a> COEFFICIENT6=0.01183445725350315
	ATOMS7=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">phi-74</a> COEFFICIENT7=-0.13467277605544367
	ATOMS8=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-74</a> COEFFICIENT8=0.08650033183819082
	ATOMS9=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">phi-75</a> COEFFICIENT9=0.16313118843978844
	ATOMS10=psi75ATM COEFFICIENT10=-0.025906352743917914
	ATOMS11=phi76ATM COEFFICIENT11=-0.026251531267691197
	ATOMS12=psi76ATM COEFFICIENT12=-0.009125395945226543
	ATOMS13=lypglpATM COEFFICIENT13=-0.016938741251970535
	ATOMS14=lyp-chi4ATM COEFFICIENT14=0.03413407121020375
	ATOMS15=lyp-chi3ATM COEFFICIENT15=-0.004460021721679498
	ATOMS16=lyp-chi2ATM COEFFICIENT16=0.014183921876930208
	ATOMS17=lyp-chi1ATM COEFFICIENT17=-0.04840847090226132	
	REFERENCE=1.2
	LABEL=alphabeta1
...

<a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_b_e_t_a.html">ALPHABETA</a> ...
	ATOMS1=al1,bb1,bb2,al2 COEFFICIENT1=-0.5162378574779953
	ATOMS2=bb1,ba1,al1,bb2 COEFFICIENT2=0.2727109903462744
	ATOMS3=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">phi-72</a> COEFFICIENT3=0.02615298801617476
	ATOMS4=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-72</a> COEFFICIENT4=-0.21749148517084058
	ATOMS5=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">phi-73</a> COEFFICIENT5=0.2045895216019467
	ATOMS6=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-73</a> COEFFICIENT6=-0.0004317179880744841
	ATOMS7=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">phi-74</a> COEFFICIENT7=0.06266501293109115
	ATOMS8=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-74</a> COEFFICIENT8=0.07608293285965884
	ATOMS9=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">phi-75</a> COEFFICIENT9=0.02467532769100892
	ATOMS10=psi75ATM COEFFICIENT10=-0.0303816314200478
	ATOMS11=phi76ATM COEFFICIENT11=-0.054467496977825394
	ATOMS12=psi76ATM COEFFICIENT12=0.021947773506833777
	ATOMS13=lypglpATM COEFFICIENT13=0.006286384110294116
	ATOMS14=lyp-chi4ATM COEFFICIENT14=-0.08453887438639353
	ATOMS15=lyp-chi3ATM COEFFICIENT15=-0.004487859866813722
	ATOMS16=lyp-chi2ATM COEFFICIENT16=-0.022650169679449442
	ATOMS17=lyp-chi1ATM COEFFICIENT17=-0.11785923783854135	
	REFERENCE=1.2
	LABEL=alphabeta2
...

<span style="color:blue">#TICA_CV</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ... 
	LABEL=cv1 
	ARG=alphabeta1,ab18
	COEFFICIENTS=1,0.4492521823194412
	PERIODIC=NO
...

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ... 
	LABEL=cv2
	ARG=alphabeta2,ab18
	COEFFICIENTS=1,0.7300530466078213
	PERIODIC=NO
...
</pre>{% endraw %}
