**Project ID:** [plumID:19.015]({{ '/' | absolute_url }}eggs/19/015/)  
**Source:** adsorbed/100_apolar/plumed_restart.dat  
**Originally used with PLUMED version:** 2.3  
**Stable:** [raw zipped stdout](plumed_restart.dat.plumed.stdout.txt.zip) - [stderr](plumed_restart.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_restart.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_restart.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue">#######IBU 321##########</span>

<span style="color:blue">#torsion1 between vector1 C2,C1 and axis C2,C10 and vector2 C10,C11 </span>
t1: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=10564,10563 AXIS=10564,10572 VECTOR2=10572,10573

<span style="color:blue">#torsion2 between vector1 C10,C7 and axis C10,C11 and vector2 C11,C12 </span>
t2: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=10572,10569 AXIS=10572,10573 VECTOR2=10573,10574

pseudobulk: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=5380-5412,6139-6171,5776-5808,5578-5610,4324-4356,5116-5148,4852-4884,4588-4620,5314-5346,6106-6138,5710-5742,5512-5544,4258-4290,5050-5082,4786-4818,4522-4554,5875-5907,6073-6105,6007-6039,5941-5973,4456-4488,5248-5280,4984-5016,4720-4752,5446-5478,6172-6204,5842-5874,5644-5676,4390-4422,5182-5214,4918-4950,4654-4686,6238-6270,5743-5775,5545-5577,5347-5379,4555-4587,4291-4323,5083-5115,4819-4851,6205-6237,5677-5709,5479-5511,5281-5312,4489-4521,4225-4257,5017-5049,4753-4785,6304-6336,6040-6072,5974-6006,5908-5940,4687-4719,4423-4455,5215-5247,4951-4983,6271-6303,5809-5841,5611-5643,5413-5445,4621-4653,4357-4389,5149-5181,4885-4917

mymol: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=10566-10569

d: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=mymol,pseudobulk COMPONENTS
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=d.z AT=3.7 KAPPA=500.0 LABEL=uwall
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=d.z AT=3.4 KAPPA=500.0 LABEL=lwall

<span style="color:blue">#metadynamics</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
ARG=t1,t2
SIGMA=0.1,0.1
HEIGHT=0.96
PACE=500
BIASFACTOR=10.0
TEMP=300.0
LABEL=metad
FILE=HILLS
GRID_MIN=-pi,-pi
GRID_MAX=pi,pi
GRID_BIN=350,350
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=t1,t2,d.z,metad.bias,uwall.bias,lwall.bias STRIDE=10 FILE=COLVAR
</pre>{% endraw %}
