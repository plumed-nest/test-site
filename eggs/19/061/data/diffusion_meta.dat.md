**Project ID:** [plumID:19.061]({{ '/' | absolute_url }}eggs/19/061/)  
**Source:** diffusion_meta.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [raw zipped stdout](diffusion_meta.dat.plumed.stdout.txt.zip) - [stderr](diffusion_meta.dat.plumed.stderr)  
**Master:** [raw zipped stdout](diffusion_meta.dat.plumed_master.stdout.txt.zip) - [stderr](diffusion_meta.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue">#Restart the simulation</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>

<span style="color:blue">#Define the guest molecule in the simulation</span>
guest: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=169-186
guest_com: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=guest

<span style="color:blue">#Define the cage centre of mass</span>
centre_com: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=1-168

<span style="color:blue">#Define the centres of the windows as the centre of the three phenyl H atoms in the window</span>
circle1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=22,78,134
circle2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=36,64,162
circle3: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=8,106,148
circle4: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r.html">CENTER</a> ATOMS=50,92,120

<span style="color:blue">#Define distances between the guest centre of mass and the centres of the windows of interest</span>
d1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=guest_com,circle1
d2: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=guest_com,circle2

<span style="color:blue">#Define distances that will need energetic walls - these are the distances to the other two windows and the overall distance from the cage centre of mass</span>
d3: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=guest_com,circle3
d4: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=guest_com,circle4
dc: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=centre_com,guest_com

lwalls: <a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=d3,d4 AT=0.25,0.25 KAPPA=4500,4500 OFFSET=0,0 EXP=2,2 EPS=1,1
uwall: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=dc AT=0.45 KAPPA=3500 OFFSET=0 EXP=2 EPS=1

<span style="color:blue">#Deposit Gaussians, with the distances d1 and d2 as the collective variable</span>
meta: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=d1,d2 SIGMA=0.01,0.01 HEIGHT=1.2 BIASFACTOR=15 TEMP=300 PACE=500 GRID_MIN=-2.0,-2.0 GRID_MAX=6.0,6.0 GRID_BIN=4000,4000 

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=d1,d2,d3,d4,meta.*,uwall.*,lwalls.* FILE=COLVAR STRIDE=2000
</pre>{% endraw %}
