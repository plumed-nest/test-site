**Project ID:** [plumID:19.057]({{ '/' | absolute_url }}eggs/19/057/)  
**Source:** plumed-main.dat  
**Originally used with PLUMED version:** 2.6  
**Stable:** [raw zipped stdout](plumed-main.dat.plumed.stdout.txt.zip) - [stderr](plumed-main.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed-main.dat.plumed_master.stdout.txt.zip) - [stderr](plumed-main.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">MOLINFO</a> STRUCTURE=aacgmodel.pdb
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=1-2473

<span style="color:blue">### BEADS DEFINITION</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_i_n_c_l_u_d_e.html">INCLUDE</a> FILE=<a href="plumed-beads.dat.html">plumed-beads.dat</a> 


<span style="color:blue">### METADYNAMICS</span>
<span style="color:blue">#</span>
<span style="color:blue"># CV DEFINITION</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_i_n_c_l_u_d_e.html">INCLUDE</a> FILE=<a href="plumed-cv.dat.html">plumed-cv.dat</a>
<span style="color:blue"># PB-METAD</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_b_m_e_t_a_d.html">PBMETAD</a> ...
 	<span style="color:blue">#GRID_RFILES=../GRID.cv1,../GRID.cv2,../GRID.hyd,../GRID.pol  </span>
	ARG=cv1,cv2,hyd,pol
	ADAPTIVE=DIFF SIGMA=2000	
	SIGMA_MIN=0.01,0.01,0.01,0.05
	HEIGHT=1.0
	PACE=200
	BIASFACTOR=30
	LABEL=pb
	GRID_MIN=-0.6,-1.2,0,0        
        GRID_MAX=2.1,1.5,800,800
	WALKERS_MPI
	GRID_WSTRIDE=5000000
	GRID_WFILES=GRID.cv1,GRID.cv2,GRID.hyd,GRID.pol
... <a href="https://plumed.github.io/doc-master/user-doc/html/_p_b_m_e_t_a_d.html">PBMETAD</a>


<span style="color:blue">### METAINFERENCE</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_i_n_c_l_u_d_e.html">INCLUDE</a> FILE=<a href="plumed-saxsCG.dat.html">plumed-saxsCG.dat</a>
saxsbias: <a href="https://plumed.github.io/doc-master/user-doc/html/_b_i_a_s_v_a_l_u_e.html">BIASVALUE</a> ARG=(saxsdata\.score) STRIDE=10 

<span style="color:blue">### MONITOR</span>
<span style="color:blue"># SAXS-AA</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_i_n_c_l_u_d_e.html">INCLUDE</a> FILE=<a href="plumed-saxsAA.dat.html">plumed-saxsAA.dat</a>
<span style="color:blue"># ENSEMBLE AND STATISTICS</span>
ens: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_s_e_m_b_l_e.html">ENSEMBLE</a> ARG=(saxsdata\.q-.*),(saxsallatom\.q-.*),pb.bias REWEIGHT
statsaxs: <a href="https://plumed.github.io/doc-master/user-doc/html/_s_t_a_t_s.html">STATS</a> ARG=(ens\.saxsdata\.q-.*) PARARG=(saxsdata\.exp-.*)
statsaa: <a href="https://plumed.github.io/doc-master/user-doc/html/_s_t_a_t_s.html">STATS</a> ARG=(ens\.saxsallatom\.q-.*) PARARG=(saxsallatom\.exp-.*)

<span style="color:blue">### PRINT</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=(saxsdata\.score),(saxsdata\.biasDer),(saxsdata\.weight),(saxsdata\.scale),(saxsdata\.acceptScale),(saxsdata\.acceptSigma),(saxsdata\.sigma.*) STRIDE=500 FILE=BAYES.SAXS
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=statsaxs.*,(ens\.saxsdata\.q-.*) STRIDE=1000 FILE=ST.SAXS
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=(saxsdata\.q-.*) STRIDE=1000 FILE=QVAL
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=statsaa.*,(ens\.saxsallatom\.q-.*) STRIDE=1000 FILE=ST.SAXSAA
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=(saxsallatom\.q-.*) STRIDE=1000 FILE=QVALAA
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=cv1,cv2,hyd,pol,pb.bias STRIDE=500 FILE=CVS

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a> 
</pre>{% endraw %}
