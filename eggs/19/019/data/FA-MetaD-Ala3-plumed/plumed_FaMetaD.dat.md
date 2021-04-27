**Project ID:** [plumID:19.019]({{ '/' | absolute_url }}eggs/19/019/)  
**Source:** FA-MetaD-Ala3-plumed/plumed_FaMetaD.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [raw zipped stdout](plumed_FaMetaD.dat.plumed.stdout.txt.zip) - [stderr](plumed_FaMetaD.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_FaMetaD.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_FaMetaD.dat.plumed_master.stderr)  

{% raw %}<pre>

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">MOLINFO</a> MOLTYPE=protein STRUCTURE=GMXfiles/ala3.pdb

<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=1

<a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_b_e_t_a.html">ALPHABETA</a> ATOMS1=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">phi-2</a> REFERENCE=1.25 LABEL=c1
<a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_b_e_t_a.html">ALPHABETA</a> ATOMS1=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">phi-3</a> REFERENCE=1.25 LABEL=c3
<a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_b_e_t_a.html">ALPHABETA</a> ATOMS1=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">phi-4</a> REFERENCE=1.25 LABEL=c5
<a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_b_e_t_a.html">ALPHABETA</a> ATOMS1=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-2</a> REFERENCE=1.25 LABEL=c2
<a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_b_e_t_a.html">ALPHABETA</a> ATOMS1=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-3</a> REFERENCE=1.25 LABEL=c4
<a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_b_e_t_a.html">ALPHABETA</a> ATOMS1=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-4</a> REFERENCE=1.25 LABEL=c6

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> LABEL=sum_abs ARG=c1,c2,c3,c4,c5,c6 POWERS=1,1,1,1,1,1 COEFFICIENTS=0.6228,0.1201,0.5643,0.1102,0.5153,0.0403 PERIODIC=NO

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...

 ARG=sum_abs
 HEIGHT=0.4
 BIASFACTOR=4
 TEMP=300.0
 SIGMA=0.04
 GRID_MIN=-0.02 GRID_MAX=2.0 GRID_BIN=200
 LABEL=WTMetaD

 FREQUENCY_ADAPTIVE
 PACE=1000 <span style="color:blue"># 2ps</span>
 FA_MAX_PACE=100000 <span style="color:blue"># 200ps</span>
 FA_UPDATE_FREQUENCY=500
 FA_MIN_ACCELERATION=1e1 <span style="color:blue"># enable the update of frq only after reaching a minimum alpha</span>
 ACCELERATION

... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_m_i_t_t_o_r.html">COMMITTOR</a> ...
  ARG=sum_abs
  STRIDE=5000
  BASIN_LL1=1.85
  BASIN_UL1=2.0
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_m_i_t_t_o_r.html">COMMITTOR</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=500 ARG=sum_abs,WTMetaD.* FILE=COLVAR FMT=%12.5f

</pre>{% endraw %}
