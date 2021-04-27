**Project ID:** [plumID:19.078]({{ '/' | absolute_url }}eggs/19/078/)  
**Source:** analytic_pes/2_D/plumed_reweight.dat  
**Originally used with PLUMED version:** 2.5-mod  
**Stable:** [raw zipped stdout](plumed_reweight.dat.plumed.stdout.txt.zip) - [stderr](plumed_reweight.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_reweight.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_reweight.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue">#</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> NATURAL
d1: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=1,2 COMPONENTS

ff: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html">MATHEVAL</a> ARG=d1.x,d1.y VAR=x0,x1 PERIODIC=NO FUNC=30.0*exp(-4.0*(x0-1)^2-4.0*(x1-1)^2)+30.0*exp(-4.0*(x0-1)^2-4.0*(x1+1)^2)+30.0*exp(-4.0*(x0+1)^2-4.0*(x1+1)^2)+30.0/(1.0/((5.0*x0+5.0)^2+(5.0*x1+5.0)^2+1)+1.0/((5.0*x0-5.0)^2+(5.0*x1+5.0)^2+1)+1.0/((5.0*x0-5.0)^2+(5.0*x1-5.0)^2+1)+1.0/((-3.5355339059*x0+3.5355339059*x1)^2+(0.500000000834386*x0+0.500000000834386*x1)^8)+1.0/(1.0*x1^8+(5.0*x0-5.0)^2)+1.0/(1.0*x0^8+(5.0*x1+5.0)^2))

bb: <a href="https://plumed.github.io/doc-master/user-doc/html/_b_i_a_s_v_a_l_u_e.html">BIASVALUE</a> ARG=ff

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=bb.bias FILE=pes.TRAJ STRIDE=1
</pre>{% endraw %}
