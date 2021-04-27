**Project ID:** [plumID:20.015]({{ '/' | absolute_url }}eggs/20/015/)  
**Source:** EMMI-ASCT2/2-EMMI/plumed.dat  
**Originally used with PLUMED version:** 2.6-dev  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># uncomment next line if your restart</span>
<span style="color:blue">#RESTART</span>

<span style="color:blue"># load extra file</span>
<span style="color:blue"># set to correct location</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_a_d.html">LOAD</a> FILE=EMMIVox.cpp

<span style="color:blue"># include topology info - set path a PDB file</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">MOLINFO</a> STRUCTURE=../0-TOPO/step5_charmm2gmx.pdb

<span style="color:blue"># define all heavy atoms - set path to index file</span>
protein-h: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> NDX_FILE=../0-TOPO/index.ndx NDX_GROUP=PROT-H

<span style="color:blue"># make protein whole and in the cell where map is defined</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ...
ADDREFERENCE 
ENTITY0=1-6701         REF0=5.3607,4.5911,3.1497
ENTITY1=6702-6741      REF1=3.2439,3.3684,6.0308
... <a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a>

<span style="color:blue"># create EMMI score</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_m_m_i_v_o_x.html">EMMIVOX</a> ...
<span style="color:blue"># name of this action</span>
LABEL=gmm
<span style="color:blue"># general parameters - do not change this! </span>
TEMP=303.15 NL_STRIDE=50 NL_CUTOFF=0.5 NS_CUTOFF=1.0
<span style="color:blue"># define atoms for cryo-EM restraint and read experimental data</span>
<span style="color:blue"># set path to map file if not in current directory</span>
ATOMS=protein-h DATA_FILE=map_zoned_align.dat
<span style="color:blue"># info about the experimental map</span>
NORM_DENSITY=2068.185 RESOLUTION=0.1 VOXEL=0.1012
<span style="color:blue"># data likelihood (or noise model): Marginal</span>
NOISETYPE=MARGINAL SIGMA_MIN=0.2
<span style="color:blue"># write output</span>
STATUS_FILE=EMMIStatus WRITE_STRIDE=2500
...

<span style="color:blue"># translate into bias - updated every 2 time steps</span>
emr: <a href="https://plumed.github.io/doc-master/user-doc/html/_b_i_a_s_v_a_l_u_e.html">BIASVALUE</a> ARG=gmm.scoreb STRIDE=2

<span style="color:blue"># print output to file</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=gmm.* FILE=COLVAR STRIDE=2500
</pre>{% endraw %}
