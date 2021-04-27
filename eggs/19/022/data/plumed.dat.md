**Project ID:** [plumID:19.022]({{ '/' | absolute_url }}eggs/19/022/)  
**Source:** plumed.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
phi: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=5,7,9,15
psi: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> ATOMS=7,9,15,17

<a href="https://plumed.github.io/doc-master/user-doc/html/_d_r_r.html">DRR</a> ...
LABEL=alad
ARG=phi,psi
FULLSAMPLES=500
GRID_MIN=-pi,-pi
GRID_MAX=pi,pi
GRID_BIN=180,180
FRICTION=2.0,2.0
TAU=0.2,0.2
OUTPUTFREQ=50000
HISTORYFREQ=500000
... <a href="https://plumed.github.io/doc-master/user-doc/html/_d_r_r.html">DRR</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=10 ARG=phi,psi,alad.phi_fict,alad.psi_fict,alad.phi_biasforce,alad.psi_biasforce FILE=COLVAR

</pre>{% endraw %}
