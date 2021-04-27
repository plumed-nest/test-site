**Project ID:** [plumID:20.022]({{ '/' | absolute_url }}eggs/20/022/)  
**Source:** sodium/plumed.dat  
**Originally used with PLUMED version:** 2.8  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>

<span style="color:blue">#+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++#</span>
<span style="color:blue">#                                                                   #</span>
<span style="color:blue">#  This input generates a multithermal-multibaric simulation that   #</span>
<span style="color:blue">#  samples a whole range of temperatures and pressures, while also  #</span>
<span style="color:blue">#  enhancing the sampling of a crystallinity order parameter        #</span>
<span style="color:blue">#                                                                   #</span>
<span style="color:blue">#+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++#</span>

ene: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a>
vol: <a href="https://plumed.github.io/doc-master/user-doc/html/_v_o_l_u_m_e.html">VOLUME</a>
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_v_i_r_o_n_m_e_n_t_s_i_m_i_l_a_r_i_t_y.html">ENVIRONMENTSIMILARITY</a> ...
  LABEL=refcv
  SPECIES=1-250
  SIGMA=0.065
  LATTICE_CONSTANTS=0.423
  CRYSTAL_STRUCTURE=BCC
  MORE_THAN={RATIONAL R_0=0.5 NN=12 MM=24}
  MEAN
... <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_v_i_r_o_n_m_e_n_t_s_i_m_i_l_a_r_i_t_y.html">ENVIRONMENTSIMILARITY</a>

mtp: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_c_v__m_u_l_t_i_t_h_e_r_m_a_l__m_u_l_t_i_b_a_r_i_c.html">ECV_MULTITHERMAL_MULTIBARIC</a> ...
  ARG=ene,vol
  TEMP=400
  MIN_TEMP=350
  MAX_TEMP=450
  PRESSURE=0.06022140857*5000 <span style="color:blue">#0.5 GPa</span>
  MIN_PRESSURE=0
  MAX_PRESSURE=0.06022140857*10000
...
umb: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_c_v__u_m_b_r_e_l_l_a_s__l_i_n_e.html">ECV_UMBRELLAS_LINE</a> ...
  ARG=refcv.morethan
  TEMP=400
  SIGMA=10
  MIN_CV=0
  MAX_CV=250
...
opes: <a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_e_s__e_x_p_a_n_d_e_d.html">OPES_EXPANDED</a> ARG=mtp.*,umb.* FILE=DeltaFs.data PACE=500 WALKERS_MPI

<a href="https://plumed.github.io/doc-master/user-doc/html/_q6.html">Q6</a> SPECIES=1-250 SWITCH={CUBIC D_0=0.4 D_MAX=0.5} VMEAN LABEL=q6
diff: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=q6.vmean,refcv.mean FUNC=(x-0.06540)/(0.4035-0.06540)-(y-0.33023)/(0.745086-0.33023) PERIODIC=NO
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=diff AT=0.1 KAPPA=100000 EXP=2 LABEL=uwall

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=500  ARG=ene,vol,refcv.*,opes.*,q6.*,diff,uwall.bias FILE=Colvar.data

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
<span style="color:blue"></span>
<span style="color:blue">All walkers have been combined:</span>
<span style="color:blue"> sort -gsk1 Colvar.* > all_Colvar.data</span>
<span style="color:blue"></span>
<span style="color:blue">The provided file DeltaFs.data has only few first and last lines</span>
</pre>{% endraw %}
