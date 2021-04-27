**Project ID:** [plumID:20.002]({{ '/' | absolute_url }}eggs/20/002/)  
**Source:** plumed-MetaD.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed-MetaD.dat.plumed.stdout.txt.zip) - [stderr](plumed-MetaD.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed-MetaD.dat.plumed_master.stdout.txt.zip) - [stderr](plumed-MetaD.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim: ft=plumed</a></span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">MOLINFO</a> STRUCTURE=npt.pdb
protein: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=1-6518
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=protein
p1: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_a_t_h_m_s_d.html">PATHMSD</a> REFERENCE=frameset_CA.pdb LAMBDA=193.6

<span style="color:blue">#metad: METAD ARG=p1.sss SIGMA=500 SIGMA_MIN=0.005 SIGMA_MAX=0.05 HEIGHT=4.184 ADAPTIVE=DIFF TEMP=300.0 BIASFACTOR=10 PACE=100</span>
metad: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=p1.sss,p1.zzz SIGMA=0.2,0.02 HEIGHT=0.4184 GRID_SPARSE GRID_MIN=0,0 GRID_MAX=40,18 GRID_BIN=200,200 FILE=HILLS PACE=500 TEMP=300.0 BIASFACTOR=8
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=p1.zzz AT=0.16 KAPPA=100000.0 LABEL=uwall

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=* STRIDE=100 FILE=colvar_metaD

</pre>{% endraw %}
