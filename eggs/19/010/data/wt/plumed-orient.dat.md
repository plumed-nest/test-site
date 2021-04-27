**Project ID:** [plumID:19.010]({{ '/' | absolute_url }}eggs/19/010/)  
**Source:** wt/plumed-orient.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed-orient.dat.plumed.stdout.txt.zip) - [stderr](plumed-orient.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed-orient.dat.plumed_master.stdout.txt.zip) - [stderr](plumed-orient.dat.plumed_master.stderr)  

{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">MOLINFO</a> STRUCTURE=template.pdb
whole: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=1-3223
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=whole

<a href="https://plumed.github.io/doc-master/user-doc/html/_r_d_c.html">RDC</a> ...
NOPBC
LABEL=nh
GYROM=-72.5388
SCALE=0.002 
ATOMS1=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-10</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-10</a> COUPLING1=6.4
ATOMS2=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-17</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-17</a> COUPLING2=-1.6
ATOMS3=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-18</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-18</a> COUPLING3=10.4
ATOMS4=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-19</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-19</a> COUPLING4=12.8
ATOMS5=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-22</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-22</a> COUPLING5=14.0
ATOMS6=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-26</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-26</a> COUPLING6=-11.2
ATOMS7=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-27</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-27</a> COUPLING7=-17.4
ATOMS8=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-28</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-28</a> COUPLING8=-10.6
ATOMS9=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-32</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-32</a> COUPLING9=-19.5
ATOMS10=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-52</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-52</a> COUPLING10=20.5
ATOMS11=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-54</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-54</a> COUPLING11=-8.1
ATOMS12=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-58</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-58</a> COUPLING12=15.5
ATOMS13=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-61</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-61</a> COUPLING13=-20.0
ATOMS14=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-62</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-62</a> COUPLING14=5.8
ATOMS15=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-64</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-64</a> COUPLING15=17.2
ATOMS16=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-65</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-65</a> COUPLING16=10.6
ATOMS17=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-66</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-66</a> COUPLING17=0.4
ATOMS18=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-68</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-68</a> COUPLING18=11.4
ATOMS19=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-69</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-69</a> COUPLING19=-3.2
ATOMS20=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-70</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-70</a> COUPLING20=6.3
ATOMS21=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-74</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-74</a> COUPLING21=26.7
ATOMS22=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-80</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-80</a> COUPLING22=-19.2
ATOMS23=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-83</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-83</a> COUPLING23=-15.0
ATOMS24=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-84</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-84</a> COUPLING24=-0.7
ATOMS25=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-85</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-85</a> COUPLING25=-3.7
ATOMS26=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-87</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-87</a> COUPLING26=-0.3
ATOMS27=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-104</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-104</a> COUPLING27=13.9
ATOMS28=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-116</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-116</a> COUPLING28=10.0
ATOMS29=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-124</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-124</a> COUPLING29=-3.9
ATOMS30=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-125</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-125</a> COUPLING30=-3.5
ATOMS31=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-126</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-126</a> COUPLING31=-6.5
ATOMS32=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-127</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-127</a> COUPLING32=-13.4
ATOMS33=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-128</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-128</a> COUPLING33=7.4
ATOMS34=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-129</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-129</a> COUPLING34=-2.1
ATOMS35=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-131</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-131</a> COUPLING35=-3.7
ATOMS36=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-133</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-133</a> COUPLING36=3.9
ATOMS37=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-134</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-134</a> COUPLING37=6.3
ATOMS38=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-143</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-143</a> COUPLING38=-12.2
ATOMS39=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-144</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-144</a> COUPLING39=3.3
ATOMS40=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-146</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-146</a> COUPLING40=11.5
ATOMS41=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-151</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-151</a> COUPLING41=-0.2
ATOMS42=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-153</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-153</a> COUPLING42=-8.0
ATOMS43=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-159</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-159</a> COUPLING43=0.9
ATOMS44=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-160</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-160</a> COUPLING44=2.5
ATOMS45=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-178</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-178</a> COUPLING45=3.7
ATOMS46=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-179</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-179</a> COUPLING46=2.1
ATOMS47=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-184</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-184</a> COUPLING47=8.1
ATOMS48=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-187</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-187</a> COUPLING48=0.1
ATOMS49=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-188</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-188</a> COUPLING49=1.6
ATOMS50=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-189</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-189</a> COUPLING50=11.4
ATOMS51=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-190</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-190</a> COUPLING51=1.7
ATOMS52=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-191</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-191</a> COUPLING52=-0.9
ATOMS53=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-194</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-194</a> COUPLING53=2.7
ATOMS54=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-197</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-197</a> COUPLING54=2.4
ATOMS55=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-199</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-199</a> COUPLING55=15.4
ATOMS56=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-200</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-200</a> COUPLING56=1.8
ATOMS57=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-201</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-201</a> COUPLING57=0.7
ATOMS58=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-205</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-205</a> COUPLING58=6.0
ATOMS59=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-206</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-206</a> COUPLING59=3.1
ATOMS60=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-207</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-207</a> COUPLING60=1.3
ATOMS61=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-208</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-208</a> COUPLING61=2.5
ATOMS62=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">N-209</a>,@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">H-209</a> COUPLING62=-0.8
... <a href="https://plumed.github.io/doc-master/user-doc/html/_r_d_c.html">RDC</a>

rdce: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_s_e_m_b_l_e.html">ENSEMBLE</a> ARG=(nh\.rdc-.*) <span style="color:blue">#,metad.bias REWEIGHT</span>
strdc: <a href="https://plumed.github.io/doc-master/user-doc/html/_s_t_a_t_s.html">STATS</a> ARG=rdce.* PARARG=(nh\.exp-.*)

theta: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=strdc.corr AT=1 KAPPA=0 SLOPE=-1000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> FILE=STATS ARG=strdc.* STRIDE=10

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
