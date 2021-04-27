**Project ID:** [plumID:19.046]({{ '/' | absolute_url }}eggs/19/046/)  
**Source:** PLUMED_VAC/plumed_VAC.dat  
**Originally used with PLUMED version:** 2.5-mod  
**Stable:** [raw zipped stdout](plumed_VAC.dat.plumed.stdout.txt.zip) - [stderr](plumed_VAC.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_VAC.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_VAC.dat.plumed_master.stderr)  

{% raw %}<pre>
tbias: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_a_d.html">READ</a> FILE=COLVAR_FM.dat VALUES=tbias IGNORE_TIME
wBpock_norm: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_a_d.html">READ</a> FILE=COLVAR_FM.dat VALUES=wBpock_norm IGNORE_TIME
ab_t: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_a_d.html">READ</a> FILE=COLVAR_FM.dat VALUES=ab_t IGNORE_TIME
Prot_norm: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_a_d.html">READ</a> FILE=COLVAR_FM.dat VALUES=Prot_norm IGNORE_TIME
lig_OW_large_norm: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_a_d.html">READ</a> FILE=COLVAR_FM.dat VALUES=lig_OW_large_norm IGNORE_TIME

rw: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__b_i_a_s.html">REWEIGHT_BIAS</a> ARG=tbias TEMP=300

<a href="https://plumed.github.io/doc-master/user-doc/html/_t_i_c_a.html">TICA</a> ...
 ARG=Prot_norm,wBpock_norm,ab_t,lig_OW_large_norm
 EIGEN_NUMBERS=4
 LAGGED_TIME=150000
 TAU_NUMBER=5000
 STEP_SIZE=0.5
 LOGWEIGHTS=rw
... <a href="https://plumed.github.io/doc-master/user-doc/html/_t_i_c_a.html">TICA</a>
</pre>{% endraw %}
