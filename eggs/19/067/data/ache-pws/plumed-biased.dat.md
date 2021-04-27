**Project ID:** [plumID:19.067]({{ '/' | absolute_url }}eggs/19/067/)  
**Source:** ache-pws/plumed-biased.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed-biased.dat.plumed.stdout.txt.zip) - [stderr](plumed-biased.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed-biased.dat.plumed_master.stdout.txt.zip) - [stderr](plumed-biased.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> LENGTH=nm TIME=ps ENERGY=kcal/mol

pws: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_a_t_h_m_s_d.html">PATHMSD</a> REFERENCE=pws.pdb LAMBDA=62

us: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=pws.sss AT=19.5 KAPPA=30000 EXP=2 EPS=1 OFFSET=0
ls: <a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=pws.sss AT=1.10 KAPPA=30000 EXP=2 EPS=1 OFFSET=0
uz: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=pws.zzz AT=0.06 KAPPA=30000 EXP=2 EPS=1 OFFSET=0

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ... 
  LABEL=meta
  ARG=pws.sss
  ADAPTIVE=DIFF 
  SIGMA=125 
  HEIGHT=2.0 
  TEMP=300 
  BIASFACTOR=13
  PACE=125 
  GRID_MIN=0.5
  GRID_MAX=20.5
  GRID_BIN=1000
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=* STRIDE=10 FILE=colvar_pws FMT=%12.8f
</pre>{% endraw %}
