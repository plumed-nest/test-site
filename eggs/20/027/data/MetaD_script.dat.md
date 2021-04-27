**Project ID:** [plumID:20.027]({{ '/' | absolute_url }}eggs/20/027/)  
**Source:** MetaD_script.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [raw zipped stdout](MetaD_script.dat.plumed.stdout.txt.zip) - [stderr](MetaD_script.dat.plumed.stderr)  
**Master:** [raw zipped stdout](MetaD_script.dat.plumed_master.stdout.txt.zip) - [stderr](MetaD_script.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>
<span style="color:blue">#PLUMED script to perform metadynamics over the C-CA-CB-CG dihedral angle of His41 in SARS-CoV1/CoV-2 MPro</span>

t1: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=607,609,612,618

<span style="color:blue">#Metadynamics setup - Gaussian of height 0.1 kJ/mol with adaptive bias width - geometric scheme</span>
metad: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=t1 SIGMA=0.05 HEIGHT=0.01 ADAPTIVE=GEOM GRID_MIN=-pi GRID_MAX=pi GRID_SPACING=0.1 PACE=500 FILE=HILLS_His41Tor

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=t1,metad.bias STRIDE=100 FILE=COLVAR_His14Tor
</pre>{% endraw %}
