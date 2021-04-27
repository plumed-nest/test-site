**Project ID:** [plumID:19.053]({{ '/' | absolute_url }}eggs/19/053/)  
**Source:** plumed.dat  
**Originally used with PLUMED version:** not specified  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_n_i_t_s.html">UNITS</a> NATURAL

<span style="color:blue"># These two commands calculate one symmetry function for each atom.  These </span>
<span style="color:blue"># symmetry functions tell us whether the environment around each atom resembles </span>
<span style="color:blue"># the environment in the solid or the environment in the liquid.</span>
fcc: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_c_c_u_b_i_c.html">FCCUBIC</a> SPECIES=1-20736 SWITCH={CUBIC D_0=1.2 D_MAX=1.5} ALPHA=27 LOWMEM 
smapfcc: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_t_r_a_n_s_f_o_r_m__m_o_r_e.html">MTRANSFORM_MORE</a> DATA=fcc SWITCH={SMAP R_0=0.5 A=8 B=8} LOWMEM
<span style="color:blue"># This calculates the position of the center of the solid region of the simulation box.  What we are computing here a weighted average position </span>
<span style="color:blue"># the weights are the order parameters computed using the two commands above.</span>
center: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_n_t_e_r__o_f__m_u_l_t_i_c_o_l_v_a_r.html">CENTER_OF_MULTICOLVAR</a> DATA=smapfcc
<span style="color:blue"># This calculates the phase field that tells us whether the structure in each part of the simulation box is solid-like or liquid like.</span>
dens: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_u_l_t_i_c_o_l_v_a_r_d_e_n_s.html">MULTICOLVARDENS</a> DATA=smapfcc ORIGIN=center DIR=xyz NBINS=50,80,80 BANDWIDTH=1.0,1.0,1.0 XREDUCED XLOWER=0.0 XUPPER=20.0 STRIDE=1 CLEAR=1
<span style="color:blue"># This finds the instantaneous location of the interface between the solid and liquid phases</span>
contour: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_i_n_d__c_o_n_t_o_u_r__s_u_r_f_a_c_e.html">FIND_CONTOUR_SURFACE</a> GRID=dens CONTOUR=0.5 SEARCHDIR=x STRIDE=1 CLEAR=1
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=contour FILE=contour.dat
<span style="color:blue"># This does the fourier transform of the location of the interface.  We can extract the interfacial stiffness from the average of this fourier transform</span>
ft: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_o_u_r_i_e_r__t_r_a_n_s_f_o_r_m.html">FOURIER_TRANSFORM</a> GRID=contour STRIDE=10 FT_TYPE=norm FOURIER_PARAMETERS=-1,1
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=ft FILE=fourier.dat STRIDE=10
</pre>{% endraw %}
