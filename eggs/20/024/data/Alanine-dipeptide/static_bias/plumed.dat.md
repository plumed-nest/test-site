**Project ID:** [plumID:20.024]({{ '/' | absolute_url }}eggs/20/024/)  
**Source:** Alanine-dipeptide/static_bias/plumed.dat  
**Originally used with PLUMED version:** 2.7  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_a_d.html">LOAD</a> FILE=../../GAMBES.cpp

<span style="color:blue"># Descriptors</span>
phi: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=5,7,9,15
psi: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=7,9,15,17

<span style="color:blue"># Bias</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_g_a_m_b_e_s.html">GAMBES</a> ...
  ARG=phi,psi
  NSTATES=2
  FILENAME=state
  PACE=500
  LABEL=ext
  BIAS_CUTOFF
  CUTOFF=30
  LAMBDA=1
  STATIC_BIAS
  STATIC_FACTORS=1,0.035
... <a href="https://plumed.github.io/doc-master/user-doc/html/_g_a_m_b_e_s.html">GAMBES</a>



<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=* STRIDE=10 FILE=COLVAR FMT=%.9f
</pre>{% endraw %}
