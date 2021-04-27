**Project ID:** [plumID:19.059]({{ '/' | absolute_url }}eggs/19/059/)  
**Source:** plumed.1.dat  
**Originally used with PLUMED version:** 2.2.3  
**Stable:** [raw zipped stdout](plumed.1.dat.plumed.stdout.txt.zip) - [stderr](plumed.1.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.1.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.1.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>
<a href="https://plumed.github.io/doc-master/user-doc/html/_i_n_c_l_u_d_e.html">INCLUDE</a> FILE=<a href="plumed_be-common.dat.html">plumed_be-common.dat</a>

<span style="color:blue">#METAD activates metadynamics</span>
<span style="color:blue">#ARG indicates variables to enhance (omega & psi)</span>
<span style="color:blue">#PACE indicates frequency of Gaussian deposition is 1000 time step (2ps)</span>
<span style="color:blue">#HEIGHT indicates that height of the Gaussians is 0.2 kJ/mol</span>
<span style="color:blue">#SIGMA indicates the width of the Gaussians on the biased cv, respectively</span>

be: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=cv2 PACE=1000 HEIGHT=0.2 SIGMA=0.23

<span style="color:blue">#print in other file the values of the CVS and the bias potential</span>
<span style="color:blue">#STRIDE frequency of output</span>
<span style="color:blue">#ARG things to print, omega, psi</span>
<span style="color:blue">#FILE, name of the file to output; COLVAR</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=500 ARG=cv1,cv2 FILE=COLVAR
</pre>{% endraw %}
