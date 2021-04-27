**Project ID:** [plumID:19.026]({{ '/' | absolute_url }}eggs/19/026/)  
**Source:** EXAMPLE/plumed.dat  
**Originally used with PLUMED version:** 2.3.0-mod  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># Order parameter:</span>
<span style="color:blue"># Number of water molecules within the largest connected "icy" cluster</span>
<span style="color:blue"># Whether a water molecule is defined as icy or not, it depends on its hydrogen bond network</span>
<span style="color:blue"># as well as the value of an order parameter built on the Steinhardt parameter Q6.</span>
<span style="color:blue"># The exact definition can be found at:</span>
<span style="color:blue"># https://pubs.acs.org/doi/suppl/10.1021/acs.jpclett.6b01013/suppl_file/jz6b01013_si_001.pdf</span>

<span style="color:blue"># Geometric criteria for hydrogen bonds (HBs) </span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_h_b_o_n_d__c_o_o_r_d.html">HBOND_COORD</a> SPECIES=2665-10353:4 HYDROGENS=2666-10354:4,2667-10355:4 RCUTOO=0.324 RCUTOH=0.25 ACUT=0.20pi LABEL=hb

<span style="color:blue"># Selecting those oxygens with 4 HB</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_f_i_l_t_e_r__b_e_t_w_e_e_n.html">MFILTER_BETWEEN</a> DATA=hb LOWER=3.9 UPPER=4.1 SMEAR=0.0 LABEL=rsumsb

<span style="color:blue"># Steinhardt parameter Q6 for this particular subset of molecules </span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_q6.html">Q6</a> SPECIES=rsumsb                SWITCH={GAUSSIAN D_0=0.324  R_0=0.00001 D_MAX=0.3241} LABEL=q6 LOWMEM

<span style="color:blue"># Local Q6 (see Plumed Docs, LOCAL_Q6) for this particular subset</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_c_a_l__q6.html">LOCAL_Q6</a> DATA=q6                 SWITCH={GAUSSIAN D_0=0.324  R_0=0.00001 D_MAX=0.3241} LABEL=lq6 LOWMEM

<span style="color:blue"># Selecting atoms with a certain value of LQ6</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_f_i_l_t_e_r__m_o_r_e.html">MFILTER_MORE</a> DATA=lq6            SWITCH={GAUSSIAN D_0=0.45   R_0=0.00001 D_MAX=0.4501} LABEL=cf

<span style="color:blue"># Create a contact matrix based on distance</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t__m_a_t_r_i_x.html">CONTACT_MATRIX</a> ATOMS=cf WTOL=0.1 SWITCH={GAUSSIAN D_0=0.324  R_0=0.00001 D_MAX=0.3241} LABEL=mat

<span style="color:blue"># Clustering, based on MFILTER_MORE and CONTACT_MATRIX</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_f_s_c_l_u_s_t_e_r_i_n_g.html">DFSCLUSTERING</a> MATRIX=mat LABEL=cls SERIAL

<span style="color:blue"># Including "surface" (nearest neighbours) atoms</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_l_u_s_t_e_r__w_i_t_h_s_u_r_f_a_c_e.html">CLUSTER_WITHSURFACE</a> CLUSTERS=cls RCUT_SURF=0.324 LABEL=scls SERIAL

<span style="color:blue"># Finding the largest connected cluster - this is the order parameter lambda we are building our</span>
<span style="color:blue"># Forward Flux Sampling (FFS) machinery upon</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_l_u_s_t_e_r__n_a_t_o_m_s.html">CLUSTER_NATOMS</a> CLUSTERS=scls CLUSTER=1 LABEL=lambda

<span style="color:blue"># In order to decide whether a particular MD run has reached the next FFS interface </span>
<span style="color:blue"># (see e.g. https://pubs.acs.org/doi/abs/10.1021/acs.jpclett.6b01013) or got back to the first interface,</span>
<span style="color:blue"># we use the COMMITTOR action</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_m_i_t_t_o_r.html">COMMITTOR</a> ARG=lambda STRIDE=2000 BASIN_LL1=0 BASIN_UL1=24 BASIN_LL2=110 BASIN_UL2=10000 FILE=shoot.dat

<span style="color:blue"># Output the value of lambda as we go along</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_o_u_t_p_u_t__c_l_u_s_t_e_r.html">OUTPUT_CLUSTER</a> CLUSTERS=scls CLUSTER=1 STRIDE=2000 FILE=dfs_surf.dat <span style="color:blue"># Output lambda</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=2000

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
