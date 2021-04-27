**Project ID:** [plumID:20.022]({{ '/' | absolute_url }}eggs/20/022/)  
**Source:** model/plumed.dat  
**Originally used with PLUMED version:** 2.8  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>

<span style="color:blue">#+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++#</span>
<span style="color:blue">#                                                           #</span>
<span style="color:blue">#  This input generates a simulation that samples the same  #</span>
<span style="color:blue">#  distribution as 28 umbrella-sampling windows             #</span>
<span style="color:blue">#                                                           #</span>
<span style="color:blue">#+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++#</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> NATURAL

p: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_o_s_i_t_i_o_n.html">POSITION</a> ATOM=1

ecv: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_c_v__u_m_b_r_e_l_l_a_s__l_i_n_e.html">ECV_UMBRELLAS_LINE</a> ...
  ARG=p.x
  MIN_CV=-2.5
  MAX_CV=2.5
  SIGMA=0.185815
...
opes: <a href="https://plumed.github.io/doc-master/user-doc/html/_o_p_e_s__e_x_p_a_n_d_e_d.html">OPES_EXPANDED</a> ARG=ecv.* FILE=DeltaFs.data PACE=500

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FMT=%g STRIDE=500 FILE=Colvar.data ARG=p.x,p.y,opes.*

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
<span style="color:blue"></span>
<span style="color:blue">will produce 10 independent run, use instead WALKERS_MPI to make multiple walkers share bias</span>
<span style="color:blue"></span>
<span style="color:blue">to print the running FES with GNUPLOT:</span>
<span style="color:blue">p '<awk ''END{for(i=3;i<=NF;i++)print -2.5+(i-3)*5/(NF-3),$i}'' DeltaFs.0.data'w lp</span>
<span style="color:blue"></span>
</pre>{% endraw %}
