**Project ID:** [plumID:21.001]({{ '/' | absolute_url }}eggs/21/001/)  
**Source:** HS6ST/cvs.dat  
{% raw %}<pre>
wte: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=ene PACE=250 HEIGHT=1.2 SIGMA=140.0 FILE=HILLS_PTWTE BIASFACTOR=16.0 TEMP=354.368

<span style="color:blue"># monitor the three variables and the metadynamics bias potential</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> STRIDE=10 ARG=dP,cn,ene,wte.bias FILE=COLVAR_PTWTE
</pre>{% endraw %}
