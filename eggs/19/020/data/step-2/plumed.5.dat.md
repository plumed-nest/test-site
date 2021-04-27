**Project ID:** [plumID:19.020]({{ '/' | absolute_url }}eggs/19/020/)  
**Source:** step-2/plumed.5.dat  
**Originally used with PLUMED version:** 2.2  
**Stable:** [raw zipped stdout](plumed.5.dat.plumed.stdout.txt.zip) - [stderr](plumed.5.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.5.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.5.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">MOLINFO</a> STRUCTURE=reference.pdb
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> STRIDE=1 ENTITY0=1-427

a: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_r_m_s_d.html">ALPHARMSD</a> RESIDUES=all TYPE=DRMSD R_0=0.08 NN=8 MM=12 
g: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_y_r_a_t_i_o_n.html">GYRATION</a> TYPE=RADIUS ATOMS=9,23,35,50,62,78,89,101,120,135,159,183,202,212,229,253,272,282,297,321,345,362,377,389,400,410
ene: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a>

wte: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=ene PACE=999999999 HEIGHT=2.5 SIGMA=500.0 FILE=HILLS_PTWTE BIASFACTOR=50.0 TEMP=367.734

metad: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=a,g PACE=500 HEIGHT=0.4184 SIGMA=0.15,0.025 FILE=HILLS_PTMetaDWTE BIASFACTOR=15.0 TEMP=367.734

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=a,g,ene,wte.bias,metad.bias STRIDE=50 FILE=COLVAR_MetadWTE

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
<span style="color:blue"></span>
</pre>{% endraw %}
