**Project ID:** [plumID:20.000]({{ '/' | absolute_url }}eggs/20/000/)  
**Source:** ratchet/rMD_plumed.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [raw zipped stdout](rMD_plumed.dat.plumed.stdout.txt.zip) - [stderr](rMD_plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](rMD_plumed.dat.plumed_master.stdout.txt.zip) - [stderr](rMD_plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue">#</span>
<span style="color:blue"># This is the input file needed to perform Ratchet&Pawl MD simulation</span>
<span style="color:blue"># based on the CV given by the distance between the ligand's center </span>
<span style="color:blue"># of mass and the center of the binding pocket.</span>
<span style="color:blue">#</span>
<span style="color:blue"># This input file can be used with all the PLUMED versions >=2.3</span>
<span style="color:blue">#</span>

<span style="color:blue"># Definition of the center of mass of the ligand, considering only its heavy atoms</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=1,5,6,10,14,17,18,19,22,23,24,25,26,29  LABEL=ixo

<span style="color:blue"># Definition of the center of mass of the pocket</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=1396,1398,1400,1403,1404,1406,1408,1409,1411,1413,1415,1416,1449,1451,1453,1456,1458,1459,1495,1497,1499,1501,1505,1509,1510,2838,2840,2842,2845,2846,2848,2850,2852,2854,2856,2857,3605,3607,3609,3612,3613,3615,3617,3618,3620,3622,3624,3625 LABEL=pkt

<span style="color:blue"># Definition of the distance between the ligand and the pocket as a 3d vector xyz</span>
<span style="color:blue"># (the membrane is in the plane xy)</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=ixo,pkt LABEL=d1 COMPONENTS NOPBC

<span style="color:blue"># Definition of the periodicity of the components of the distance </span>
<span style="color:blue"># (to avoid jumps in the variable during the simulation due to the </span>
<span style="color:blue"># rototranslation of the system)</span>
d1x: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1.x PERIODIC=-4.7,4.7
d1y: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1.y PERIODIC=-4.7,4.7
d1z: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m_b_i_n_e.html">COMBINE</a> ARG=d1.z PERIODIC=-8.2,8.2

<span style="color:blue"># Activation of the Ratchet&Pawl MD, to observe the transition of the ligand. </span>
<span style="color:blue"># Starting from the bound structure, the bias will move the system outside </span>
<span style="color:blue"># the binding cavity with a k=100 kJ/mol/nm until the ligand is 4 nm outside</span>
<span style="color:blue"># the binding cavity </span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_a_b_m_d.html">ABMD</a> ...
  ARG=d1z
  TO=-4.0
  KAPPA=100.0
LABEL=rmd
... <a href="https://plumed.github.io/doc-master/user-doc/html/_a_b_m_d.html">ABMD</a>


<span style="color:blue"># Here we print all the data regarding rMD_data</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=rmd.* STRIDE=500 FILE=rMD_data
<span style="color:blue"># Here we print the distance between the molecule and the binding pocket</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=d1z STRIDE=500 FILE=IXO_dist.dat

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
