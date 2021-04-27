**Project ID:** [plumID:21.011]({{ '/' | absolute_url }}eggs/21/011/)  
**Source:** NaCl_at_graphite-cmumd/clusters.plmd  
**Originally used with PLUMED version:** 2.5.1  
**Stable:** [raw zipped stdout](clusters.plmd.plumed.stdout.txt.zip) - [stderr](clusters.plmd.plumed.stderr)  
**Master:** [raw zipped stdout](clusters.plmd.plumed_master.stdout.txt.zip) - [stderr](clusters.plmd.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># Define atom groups</span>
gra: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=1-9152:1 
wat: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=9153-43319:3
sod: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=43320-43737:1
chl: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=43738-44155:1
slt: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=43320-44155:1
sln: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=9153-44155:1 

<span style="color:blue"># Set a virtual atom at the origin and in the 'bulk'</span>
p0: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_i_x_e_d_a_t_o_m.html">FIXEDATOM</a> AT=2.696525,2.75872,7.403535
p1: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_i_x_e_d_a_t_o_m.html">FIXEDATOM</a> AT=2.696525,2.75872,11.403535

<span style="color:blue"># Identify cations at the interface and in the bulk</span>
denssod: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_e_n_s_i_t_y.html">DENSITY</a> SPECIES=43320-43737
sodint: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_r_o_u_n_d.html">AROUND</a> DATA=denssod ATOM=p0 ZLOWER=1.4 ZUPPER=2.0 SIGMA=0.01
sodblk: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_r_o_u_n_d.html">AROUND</a> DATA=denssod ATOM=p1 ZLOWER=-0.5 ZUPPER=0.5 SIGMA=0.01

<span style="color:blue"># Get the Na-Cl coordination number distribution at the interface and in the bulk</span>
cnint: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIESA=sodint SPECIESB=chl SWITCH={RATIONAL R_0=0.355 NN=32 MM=64} MEAN HIGHEST
cnblk: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">COORDINATIONNUMBER</a> SPECIESA=sodblk SPECIESB=chl SWITCH={RATIONAL R_0=0.355 NN=32 MM=64} MEAN HIGHEST

<span style="color:blue"># Report the mean and highest coordination numbers in the different regions</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=cnint.*,cnblk.* FILE=cn-regions.dat

<span style="color:blue"># DFS on ion clusters at the interface</span>
mat0: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t__m_a_t_r_i_x.html">CONTACT_MATRIX</a> ATOMS=cnint SWITCH={GAUSSIAN D_0=0.355 R_0=0.01}
dfs0: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_f_s_c_l_u_s_t_e_r_i_n_g.html">DFSCLUSTERING</a> MATRIX=mat0
<span style="color:blue"># Number of ion clusters at the interface</span>
nclust0: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_l_u_s_t_e_r__d_i_s_t_r_i_b_u_t_i_o_n.html">CLUSTER_DISTRIBUTION</a> CLUSTERS=dfs0 MORE_THAN={GAUSSIAN D_0=1.95 R_0=0.01 D_MAX=1.99}
<span style="color:blue"># Largest cluster at the interface</span>
clust0nat: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_l_u_s_t_e_r__n_a_t_o_m_s.html">CLUSTER_NATOMS</a> CLUSTERS=dfs0 CLUSTER=1

<span style="color:blue"># DFS on ion clusters in the bulk</span>
mat1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t__m_a_t_r_i_x.html">CONTACT_MATRIX</a> ATOMS=cnblk SWITCH={RATIONAL R_0=0.355 D_MAX=0.356}
dfs1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_f_s_c_l_u_s_t_e_r_i_n_g.html">DFSCLUSTERING</a> MATRIX=mat1
<span style="color:blue"># Number of ion clusters in the bulk</span>
nclust1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_l_u_s_t_e_r__d_i_s_t_r_i_b_u_t_i_o_n.html">CLUSTER_DISTRIBUTION</a> CLUSTERS=dfs1 MORE_THAN={GAUSSIAN D_0=1.95 R_0=0.01 D_MAX=1.99}
<span style="color:blue"># Largest cluster in the bulk</span>
clust1nat: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_l_u_s_t_e_r__n_a_t_o_m_s.html">CLUSTER_NATOMS</a> CLUSTERS=dfs1 CLUSTER=1

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=nclust0.*,clust0nat.*,nclust1.*,clust1nat.* FILE=cluster.dat
</pre>{% endraw %}
