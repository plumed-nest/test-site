**Project ID:** [plumID:20.006]({{ '/' | absolute_url }}eggs/20/006/)  
**Source:** NEST/metad_GCGR/plumed.dat  
**Originally used with PLUMED version:** 2.4.3  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">MOLINFO</a> STRUCTURE=nowat.pdb
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=1-471 ENTITY1=472-6973 STRIDE=1

open: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_m_s_d.html">RMSD</a> REFERENCE=model.TM.open.skipped.pdb TYPE=OPTIMAL
closed: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_m_s_d.html">RMSD</a> REFERENCE=model.TM.closed.skipped.pdb TYPE=OPTIMAL

ene: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ...
  LABEL=prog
  ARG=open,closed
  COEFFICIENTS=1,-1
  PERIODIC=NO
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ...
  LABEL=dist
  ARG=open,closed
  COEFFICIENTS=1,1
  PERIODIC=NO
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
  LABEL=wte
  ARG=ene
  PACE=500000000 <span style="color:blue"># 10us</span>
  HEIGHT=5 SIGMA=1000
  FILE=HILLS_WTE.0
  BIASFACTOR=20.0 TEMP=300.0
  GRID_MIN=-1500000 GRID_MAX=-500000 GRID_SPACING=10
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
  LABEL=meta
  ARG=prog,dist
  SIGMA=0.05,0.05 HEIGHT=1.5 PACE=500
  BIASFACTOR=15 TEMP=300.0
  GRID_MIN=-1.2,0.5 GRID_MAX=1.2,2.0 GRID_SPACING=0.005,0.005
  FILE=HILLS
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>


<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=open,closed,dist AT=1.2,1.2,1.6 KAPPA=3000.0,3000.0,3000.0 LABEL=uwall


<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=* STRIDE=500 FILE=COLVAR FMT=%8.4f

</pre>{% endraw %}
