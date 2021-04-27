**Project ID:** [plumID:19.050]({{ '/' | absolute_url }}eggs/19/050/)  
**Source:** plumed_histogram.dat  
**Originally used with PLUMED version:** not specified  
**Stable:** [raw zipped stdout](plumed_histogram.dat.plumed.stdout.txt.zip) - [stderr](plumed_histogram.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed_histogram.dat.plumed_master.stdout.txt.zip) - [stderr](plumed_histogram.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># These first two commands instruct plumed to read in the quantities for each</span>
<span style="color:blue"># trajectory frame that were computed using the previous input file</span>
cv: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_a_d.html">READ</a> FILE=COLVAR-reweight VALUES=cont2.* IGNORE_TIME
w: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_a_d.html">READ</a> FILE=COLVAR-reweight VALUES=bias IGNORE_TIME
<span style="color:blue"># This command computes the reweighting factors for each of the frames in the</span>
<span style="color:blue"># trajectory from the simulation bias for that frame.  These reweighting factors</span>
<span style="color:blue"># are the exponential terms in the expression above.</span>
aa: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_w_e_i_g_h_t__b_i_a_s.html">REWEIGHT_BIAS</a> ARG=w TEMP=325
<span style="color:blue"># This command constructs the weighted histogram that appears inside the</span>
<span style="color:blue"># logarithm in the equation above</span>
hh: <a href="https://plumed.github.io/doc-master/user-doc/html/_h_i_s_t_o_g_r_a_m.html">HISTOGRAM</a> ...
  ARG=cv.dist1  GRID_MIN=0  GRID_MAX=6.5  GRID_BIN=650
  BANDWIDTH=0.02  LOGWEIGHTS=aa
...
<span style="color:blue"># This first of these two commands takes the logarithm of the weighted</span>
<span style="color:blue"># histogram, while the second outputs the final free energy surface to a file.</span>
ff: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_v_e_r_t__t_o__f_e_s.html">CONVERT_TO_FES</a> GRID=hh TEMP=325
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_u_m_p_g_r_i_d.html">DUMPGRID</a> GRID=ff FILE=FES-reweight.dat
</pre>{% endraw %}
