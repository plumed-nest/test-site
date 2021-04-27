**Project ID:** [plumID:19.076]({{ '/' | absolute_url }}eggs/19/076/)  
**Source:** Pulling/000100/pleq1  
**Originally used with PLUMED version:** 2.1  
**Stable:** [raw zipped stdout](pleq1.plumed.stdout.txt.zip) - [stderr](pleq1.plumed.stderr)  
**Master:** [raw zipped stdout](pleq1.plumed_master.stdout.txt.zip) - [stderr](pleq1.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># Adapt units to LAMMPS script (units real)</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> LENGTH=A TIME=fs ENERGY=kcal/mol

<span style="color:blue"># Radius of Gyration</span>
rg: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_y_r_a_t_i_o_n.html">GYRATION</a> TYPE=RADIUS ATOMS=1-293


restr: ...
        <a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_v_i_n_g_r_e_s_t_r_a_i_n_t.html">MOVINGRESTRAINT</a>
        ARG=rg
        STEP0=0 AT0=26.2759 KAPPA0=10
        STEP1=1 AT1=26.2759 KAPPA1=10
...
<span style="color:blue"># Print rg</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=rg,restr.rg_cntr,restr.rg_work FILE=workeq1 STRIDE=100000

<span style="color:blue"># End of Program</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
