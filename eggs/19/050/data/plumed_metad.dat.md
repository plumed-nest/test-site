**Project ID:** [plumID:19.050]({{ '/' | absolute_url }}eggs/19/050/)  
**Source:** plumed_metad.dat  
**Originally used with PLUMED version:** not specified  
**Stable:** [raw zipped stdout](plumed_metad.dat.plumed.stdout.txt.zip) - [stderr](plumed_metad.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_metad.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_metad.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># The two lines below instruct PLUMED to calculate the distance between</span>
<span style="color:blue"># the adsorbate and the isosurface.  Notice how, as discussed in the main text,</span>
<span style="color:blue"># only a subset of the atoms in the membrane are used when we calculate the</span>
<span style="color:blue"># density as this reduces the computational expense.</span>
d1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_e_n_s_i_t_y.html">DENSITY</a> SPECIES=2-2400:12,10-2400:12 LOWMEM
cont: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e__f_r_o_m__c_o_n_t_o_u_r.html">DISTANCE_FROM_CONTOUR</a> ...
  DATA=d1 ATOM=2413 BANDWIDTH=3.0,3.0,3.0 DIR=z CONTOUR=0.42
...
<span style="color:blue"># This command instructs PLUMED to construct a metadynamics bias that is a</span>
<span style="color:blue"># function of the CV that is used in the main text.  In order to reduce the</span>
<span style="color:blue"># computational expense this bias is stored on a grid.  Furthermore, adaptive</span>
<span style="color:blue"># hills are used to ensure faster convergence of the final free energy surface</span>
mm: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
  ARG=cont.qdist SIGMA=0.5 HEIGHT=1.3 PACE=100 BIASFACTOR=25 TEMP=325
  GRID_MIN=-15.0 GRID_MAX=100.0 GRID_BIN=115000
  ADAPTIVE=GEOM SIGMA_MIN=0.05 SIGMA_MAX=6.00
...
<span style="color:blue"># This command instructs PLUMED to add a restraint that prevents the collective</span>
<span style="color:blue"># variable from taking high values. This restraint thus prevents the adsorbate</span>
<span style="color:blue"># from moving too far from the membrane surface.</span>
uwall: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=cont.qdist AT=50.0 KAPPA=1.0 EXP=2
<span style="color:blue"># This command prints the value of the collective variable and the metadynamics</span>
<span style="color:blue"># bias to a file called colvar</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=cont.*,mm.* STRIDE=20 FILE=colvar
</pre>{% endraw %}
