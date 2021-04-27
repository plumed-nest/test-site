**Project ID:** [plumID:21.011]({{ '/' | absolute_url }}eggs/21/011/)  
**Source:** NaCl_at_graphite-cmumd/cmumd.plmd  
**Originally used with PLUMED version:** 2.5.1  
**Stable:** [raw zipped stdout](cmumd.plmd.plumed.stdout.txt.zip) - [stderr](cmumd.plmd.plumed.stderr)  
**Master:** [raw zipped stdout](cmumd.plmd.plumed_master.stdout.txt.zip) - [stderr](cmumd.plmd.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># Plumed (v2) input file to implement CmuMD</span>
<span style="color:blue"># Please consider citing Perego et al. J Chem Phys 142, 144113 (2015)</span>
<span style="color:blue"># Please consider citing Finney et al. </span>

<span style="color:blue"># CmuMD is not yet implemented in Plumed</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_a_d.html">LOAD</a> FILE=Cmumd.cpp

<span style="color:blue"># Define groups of atoms</span>
gra: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=1-9152:1 
sod: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=43320-43737:1
chl: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=43738-44155:1
slt: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=43320-44155:1
wat: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=9153-43319:1
sln: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=9153-44155:1 
all: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=1-44155:1

<span style="color:blue"># Provide parameters for the CV</span>
nwat: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_m_u_m_d.html">CMUMD</a> GROUP=wat NSV=3 DCR=0.25 CRSIZE=0.15 WF=0.0001 NINT=1.0 NZ=291
nsod: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_m_u_m_d.html">CMUMD</a> GROUP=sod NSV=1 FIXED=0.5 DCR=0.25 CRSIZE=0.15 WF=0.0001 NINT=0.1 NZ=291
nchl: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_m_u_m_d.html">CMUMD</a> GROUP=chl NSV=1 FIXED=0.5 DCR=0.25 CRSIZE=0.15 WF=0.0001 NINT=0.1 NZ=291

<span style="color:blue"># CmuMD is implemented as a restraint on the densities of species in CR</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=nsod AT=0.3011 KAPPA=20000.0 LABEL=resna
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=nchl AT=0.3011 KAPPA=20000.0 LABEL=rescl
<span style="color:blue">#RESTRAINT ARG=n_water AT=29.5 KAPPA=20.0 LABEL=wres</span>


<span style="color:blue"># Report the densities and bias</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ...
ARG=nsod,nchl,nwat,resna.bias,rescl.bias
 STRIDE=50
 FILE=COLVAR
... <a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a>



</pre>{% endraw %}
