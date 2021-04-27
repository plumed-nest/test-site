**Project ID:** [plumID:19.007]({{ '/' | absolute_url }}eggs/19/007/)  
**Source:** EMMI-MT/plumed.dat  
**Originally used with PLUMED version:** 2.6-dev  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># include topology info: this is needed to identify atom types</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">MOLINFO</a> STRUCTURE=structure.pdb
<span style="color:blue"># define all heavy atoms using GROMACS index file</span>
<span style="color:blue"># which can be created with gmx_mpi make_ndx</span>
protein-h: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> NDX_FILE=index.ndx NDX_GROUP=Protein-H
protein: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> NDX_FILE=index.ndx NDX_GROUP=Protein
protein-no-negative: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> NDX_FILE=index.ndx NDX_GROUP=Protein-no-negative-no-h
<span style="color:blue"># make protein whole: add reference position of first heavy atom (in nm)</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ADDREFERENCE ENTITY0=protein REF0=3.217,4.340,6.195
<span style="color:blue"># create EMMI score</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_m_m_i.html">EMMI</a> ...
LABEL=gmm NOPBC TEMP=300.0 NL_STRIDE=50 NL_CUTOFF=0.01
ATOMS=protein-no-negative GMM_FILE=AC_SYMM.dat
<span style="color:blue">#ATOMS selects what is refined</span>
<span style="color:blue"># no-negative-no-h or no-h are reasonable</span>
<span style="color:blue"># resolution is not used - no Bfactor fitting</span>
<span style="color:blue"># SIGMA_MIN can go down to 0.02, must be > NL_CUTOFF,</span>
<span style="color:blue"># if crashes, raise back to 0.05,</span>
<span style="color:blue"># the larger the number the softer the contribution of the EM data</span>
SIGMA_MIN=0.05 RESOLUTION=0.1 NOISETYPE=MARGINAL
...

<span style="color:blue"># translate into bias</span>
emr: <a href="https://plumed.github.io/doc-master/user-doc/html/_b_i_a_s_v_a_l_u_e.html">BIASVALUE</a> ARG=gmm.scoreb STRIDE=2
<span style="color:blue"># print useful info to file</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=gmm.* FILE=COLVAR STRIDE=500
</pre>{% endraw %}
