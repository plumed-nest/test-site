**Project ID:** [plumID:19.067]({{ '/' | absolute_url }}eggs/19/067/)  
**Source:** ache-pwf/plumed-unbiased.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed-unbiased.dat.plumed.stdout.txt.zip) - [stderr](plumed-unbiased.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed-unbiased.dat.plumed_master.stdout.txt.zip) - [stderr](plumed-unbiased.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> LENGTH=nm TIME=ps ENERGY=kcal/mol

pwf: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_a_t_h_m_s_d.html">PATHMSD</a> REFERENCE=pwf.pdb LAMBDA=65

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=* STRIDE=10 FILE=colvar_pwf FMT=%12.8f
</pre>{% endraw %}
