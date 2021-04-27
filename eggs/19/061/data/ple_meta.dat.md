**Project ID:** [plumID:19.061]({{ '/' | absolute_url }}eggs/19/061/)  
**Source:** ple_meta.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [raw zipped stdout](ple_meta.dat.plumed.stdout.txt.zip) - [stderr](ple_meta.dat.plumed.stderr)  
**Master:** [raw zipped stdout](ple_meta.dat.plumed_master.stdout.txt.zip) - [stderr](ple_meta.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue">#Restart the simulation</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>

<span style="color:blue">#Define the cage and guest centres of mass and the distance between them</span>
cage_com: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=1-168
guest_com: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=169-186

d1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=cage_com,guest_com NOPBC

<span style="color:blue">#Define the energetic wall for the system, to prevent the guest moving too far from the cage</span>
uwall: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=d1 AT=2.4 KAPPA=150.0 EXP=2 EPS=1 OFFSET=0

<span style="color:blue">#Deposit Gaussians using the distance between the centres of mass as the collective variable, and print the output to the COLVAR file</span>
meta: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=d1 SIGMA=0.05 HEIGHT=1.2 PACE=500 BIASFACTOR=10 TEMP=300 GRID_MIN=-1.0 GRID_MAX=5.0 GRID_BIN=2400

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=d1,meta.*,uwall.* FILE=COLVAR STRIDE=2000
</pre>{% endraw %}
