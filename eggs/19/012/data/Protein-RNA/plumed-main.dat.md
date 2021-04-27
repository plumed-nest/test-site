**Project ID:** [plumID:19.012]({{ '/' | absolute_url }}eggs/19/012/)  
**Source:** ./Protein-RNA/plumed-main.dat  
**Originally used with PLUMED version:** 2.6  
**Stable:** [raw zipped stdout](plumed-main.dat.plumed.stdout.txt.zip) - [stderr](plumed-main.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed-main.dat.plumed_master.stdout.txt.zip) - [stderr](plumed-main.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">MOLINFO</a> STRUCTURE=aacgmodel.pdb
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=1-1393,3125-3349,1372-2938,3320-3511,2262-3124

<span style="color:blue">### BEADS DEFINITION</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_i_n_c_l_u_d_e.html">INCLUDE</a> FILE=<a href="plumed-beads.dat.html">plumed-beads.dat</a> 

<span style="color:blue">### RESTRAINTS</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_i_n_c_l_u_d_e.html">INCLUDE</a> FILE=<a href="plumed-restr.dat.html">plumed-restr.dat</a> 

<span style="color:blue">### METAINFERENCE</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_i_n_c_l_u_d_e.html">INCLUDE</a> FILE=<a href="plumed-saxsCG.dat.html">plumed-saxsCG.dat</a>
saxsbias: <a href="https://plumed.github.io/doc-master/user-doc/html/_b_i_a_s_v_a_l_u_e.html">BIASVALUE</a> ARG=(saxsdata\.score) STRIDE=10 


<span style="color:blue">#STAT</span>
statcg: <a href="https://plumed.github.io/doc-master/user-doc/html/_s_t_a_t_s.html">STATS</a> ARG=(saxsdata\.q-.*) PARARG=(saxsdata\.exp-.*)

<span style="color:blue">## PRINT</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=(saxsdata\.score),(saxsdata\.scale),(saxsdata\.acceptScale),(saxsdata\.acceptSigma),(saxsdata\.sigma.*) STRIDE=500 FILE=BAYES.SAXS
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=(saxsdata\.q-.*) STRIDE=500 FILE=QVALCG
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=statcg.* STRIDE=500 FILE=ST.SAXSCG

</pre>{% endraw %}
