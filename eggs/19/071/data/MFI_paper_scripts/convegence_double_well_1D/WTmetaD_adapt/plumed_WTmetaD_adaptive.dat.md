**Project ID:** [plumID:19.071]({{ '/' | absolute_url }}eggs/19/071/)  
**Source:** MFI_paper_scripts/convegence_double_well_1D/WTmetaD_adapt/plumed_WTmetaD_adaptive.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed_WTmetaD_adaptive.dat.plumed.stdout.txt.zip) - [stderr](plumed_WTmetaD_adaptive.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_WTmetaD_adaptive.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_WTmetaD_adaptive.dat.plumed_master.stderr)  

{% raw %}<pre>
p: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1,2 COMPONENTS
ff: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=p.x PERIODIC=NO FUNC=(-5*x^2+x^4)
bb: <a href="https://plumed.github.io/doc-master/user-doc/html/_b_i_a_s_v_a_l_u_e.html">BIASVALUE</a> ARG=ff

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=p.x SIGMA=50 HEIGHT=0.1 PACE=500 BIASFACTOR=5 ADAPTIVE=DIFF LABEL=metad TEMP=120 GRID_MIN=-2.7 GRID_MAX=2.7 GRID_BIN=500 

<span style="color:blue">#METAD ARG=p.x SIGMA=0.1 HEIGHT=0.01 PACE=500 LABEL=metad </span>


<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FILE=position ARG=p.x

</pre>{% endraw %}
