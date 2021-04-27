**Project ID:** [plumID:21.012]({{ '/' | absolute_url }}eggs/21/012/)  
**Source:** wild/plumed.dat  
**Originally used with PLUMED version:** 2.7  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>

<span style="color:blue"># COLVAR</span>
lig: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=5533-5577 <span style="color:blue"># you need the COM of your ligand/molecule</span>
pbd1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=3261-3284 <span style="color:blue"># describe product binding domain (res 213)</span>
pbd2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=3736-3756 <span style="color:blue"># describe prroduct binding domain (res 245)</span>
wallres: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=4335-4349 <span style="color:blue"># lower wall on deep active site residue</span>

<span style="color:blue"># FUNNEL</span>
wd: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=3616,lig <span style="color:blue"># anchor dist for walls </span>
fps: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_u_n_n_e_l__p_s.html">FUNNEL_PS</a> REFERENCE=ref.pdb LIGAND=lig ANCHOR=3616 POINTS=5.1375,4.3952,5.3672,6.5414,3.6569,5.4359

d1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=pbd1,lig <span style="color:blue"># For the meta, not Funnel related</span>
d2: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=pbd2,lig
d3: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=wallres,lig

<a href="https://plumed.github.io/doc-master/user-doc/html/_f_u_n_n_e_l.html">FUNNEL</a> ARG=fps.lp,fps.ld ZCC=2.5 ALPHA=0.55 RCYL=0.1 MINS=-1 MAXS=6 KAPPA=50000 NBINS=500 NBINZ=500 SAFETY=1.0 SLOPE=1.0 LABEL=funnel FILE=BIAS

<span style="color:blue">### METADYNAMICS ### </span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
    ARG=d1,fps.lp
    SIGMA=0.05,0.05
    HEIGHT=2.5 <span style="color:blue">#kj/mol</span>
    PACE=1000
    BIASFACTOR=8
    TEMP=300
    GRID_MIN=-0.5,-1
    GRID_MAX=5.0,6.0
    LABEL=metad <span style="color:blue"># Not Funnel related</span>
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>

<span style="color:blue">### WALLS ###</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=fps.lp AT=4.0 KAPPA=500000.0 EXP=2 OFFSET=0 LABEL=uwall1
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=fps.ld AT=1.0 KAPPA=500000.0 EXP=2 OFFSET=0 LABEL=uwall2

<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=fps.lp AT=0.00 KAPPA=500000.0 EXP=3 OFFSET=0 LABEL=lwall1
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=fps.ld AT=0.0 KAPPA=500000.0 EXP=3 OFFSET=0 LABEL=lwall2
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=d3 AT=0.7 KAPPA=500000.0 LABEL=reswall


<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=1000 ARG=* FILE=COLVAR
</pre>{% endraw %}
