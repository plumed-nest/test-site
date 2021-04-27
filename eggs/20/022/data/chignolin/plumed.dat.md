**Project ID:** [plumID:20.022]({{ '/' | absolute_url }}eggs/20/022/)  
**Source:** chignolin/plumed.dat  
**Originally used with PLUMED version:** 2.8  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>

<span style="color:blue">#++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++#</span>
<span style="color:blue">#                                                                  #</span>
<span style="color:blue">#  This input generates a multithermal-multibaric simulation that  #</span>
<span style="color:blue">#  samples a whole range of temperatures and pressures, using a    #</span>
<span style="color:blue">#  chosen fixed number of replicas (multiple walkers)              #</span>
<span style="color:blue">#                                                                  #</span>
<span style="color:blue">#++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++#</span>

<span style="color:blue">#RESTART</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">MOLINFO</a> STRUCTURE=input-chignolin.pdb
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> STRIDE=1 ENTITY0=1-166

ene: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_e_r_g_y.html">ENERGY</a>
vol: <a href="https://plumed.github.io/doc-master/user-doc/html/_v_o_l_u_m_e.html">VOLUME</a>
pdb_rmsd: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_m_s_d.html">RMSD</a> REFERENCE=input-chignolin.pdb TYPE=OPTIMAL

ecv: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_c_v__m_u_l_t_i_t_h_e_r_m_a_l__m_u_l_t_i_b_a_r_i_c.html">ECV_MULTITHERMAL_MULTIBARIC</a> ...
  ARG=ene,vol
<span style="color:blue"># TEMP=500</span>
  MIN_TEMP=270
  MAX_TEMP=800
  PRESSURE=0.06022140857*2000 <span style="color:blue">#2 kbar</span>
  MIN_PRESSURE=0.06022140857  <span style="color:blue">#1 bar</span>
  MAX_PRESSURE=0.06022140857*4000 <span style="color:blue">#4 kbar</span>
  CUT_CORNER=500,0.06022140857,800,0.06022140857*1000
...
opes: <a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_e_s__e_x_p_a_n_d_e_d.html">OPES_EXPANDED</a> ARG=ecv.* FILE=DeltaFs.data PACE=500 WALKERS_MPI

<span style="color:blue">#e2e: DISTANCE ATOMS=5,147 #first and last CA</span>
<span style="color:blue">#gyr: GYRATION ATOMS=5,26,47,67,73,88,102,109,123,147</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FMT=%g STRIDE=500 FILE=Colvar.data ARG=ene,vol,pdb_rmsd,opes.*

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
<span style="color:blue"></span>
<span style="color:blue">temp=500 K</span>
<span style="color:blue">pres=2000 bar</span>
<span style="color:blue"></span>
<span style="color:blue">input obtained from unbiased simultation, only rep 6,8,9 start from folded</span>
<span style="color:blue"></span>
</pre>{% endraw %}
