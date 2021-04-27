**Project ID:** [plumID:20.027]({{ '/' | absolute_url }}eggs/20/027/)  
**Source:** MetaD_analysis.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [raw zipped stdout](MetaD_analysis.dat.plumed.stdout.txt.zip) - [stderr](MetaD_analysis.dat.plumed.stderr)  
**Master:** [raw zipped stdout](MetaD_analysis.dat.plumed_master.stdout.txt.zip) - [stderr](MetaD_analysis.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue">#PLUMED script to output the C-CA-CB-CG and CA-CB-CG-CD2 dihedral angles of His41 in SARS-CoV1/CoV2 Mpro</span>

t1: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=607,609,612,618
t2: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=607,609,612,620
dyad_dist: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=616,2241

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=1 ARG=t1,t2,dyad_dist FILE=COLVAR_analysis
</pre>{% endraw %}
