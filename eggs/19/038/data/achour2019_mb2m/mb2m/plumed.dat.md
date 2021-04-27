**Project ID:** [plumID:19.038]({{ '/' | absolute_url }}eggs/19/038/)  
**Source:** achour2019_mb2m/mb2m/plumed.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># <a href="https://plumed.github.io/doc-master/user-doc/html/_vim_syntax.html">vim:ft=plumed</a></span>

<span style="color:blue">#general setup</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">MOLINFO</a> STRUCTURE=template.pdb
protein: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=1-1618
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=protein
<span style="color:blue">#collective variables</span>
ab: <a href="https://plumed.github.io/doc-master/user-doc/html/_a_n_t_i_b_e_t_a_r_m_s_d.html">ANTIBETARMSD</a> RESIDUES=all TYPE=OPTIMAL R_0=0.11 STRANDS_CUTOFF=0.9 NOPBC

<a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_b_e_t_a.html">ALPHABETA</a> ...
LABEL=abback
REFERENCE=0
ATOMS1=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-4</a>
ATOMS2=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-5</a>
ATOMS3=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-6</a>
ATOMS4=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-7</a>
ATOMS5=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-8</a>
ATOMS6=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-9</a>
ATOMS7=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-10</a>
ATOMS8=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-11</a>
ATOMS9=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-12</a>
ATOMS10=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-13</a>
ATOMS11=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-14</a>
ATOMS12=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-15</a>
ATOMS13=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-16</a>
ATOMS14=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-17</a>
ATOMS15=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-18</a>
ATOMS16=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-19</a>
ATOMS17=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-20</a>
ATOMS18=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-21</a>
ATOMS19=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-22</a>
ATOMS20=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-23</a>
ATOMS21=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-24</a>
ATOMS22=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-25</a>
ATOMS23=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-26</a>
ATOMS24=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-27</a>
ATOMS25=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-28</a>
ATOMS26=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-29</a>
ATOMS27=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-30</a>
ATOMS28=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-31</a>
ATOMS29=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-32</a>
ATOMS30=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-33</a>
ATOMS31=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-34</a>
ATOMS32=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-35</a>
ATOMS33=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-36</a>
ATOMS34=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-37</a>
ATOMS35=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-38</a>
ATOMS36=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-39</a>
ATOMS37=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-40</a>
ATOMS38=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-41</a>
ATOMS39=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-42</a>
ATOMS40=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-43</a>
ATOMS41=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-44</a>
ATOMS42=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-45</a>
ATOMS43=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-46</a>
ATOMS44=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-47</a>
ATOMS45=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-48</a>
ATOMS46=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-49</a>
ATOMS47=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-50</a>
ATOMS48=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-51</a>
ATOMS49=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-52</a>
ATOMS50=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-53</a>
ATOMS51=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-54</a>
ATOMS52=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-55</a>
ATOMS53=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-56</a>
ATOMS54=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-57</a>
ATOMS55=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-58</a>
ATOMS56=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-59</a>
ATOMS57=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-60</a>
ATOMS58=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-61</a>
ATOMS59=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-62</a>
ATOMS60=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-63</a>
ATOMS61=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-64</a>
ATOMS62=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-65</a>
ATOMS63=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-66</a>
ATOMS64=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-67</a>
ATOMS65=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-68</a>
ATOMS66=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-69</a>
ATOMS67=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-70</a>
ATOMS68=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-71</a>
ATOMS69=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-72</a>
ATOMS70=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-73</a>
ATOMS71=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-74</a>
ATOMS72=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-75</a>
ATOMS73=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-76</a>
ATOMS74=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-77</a>
ATOMS75=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-78</a>
ATOMS76=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-79</a>
ATOMS77=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-80</a>
ATOMS78=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-81</a>
ATOMS79=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-82</a>
ATOMS80=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-83</a>
ATOMS81=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-84</a>
ATOMS82=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-85</a>
ATOMS83=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-86</a>
ATOMS84=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-87</a>
ATOMS85=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-88</a>
ATOMS86=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-89</a>
ATOMS87=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-90</a>
ATOMS88=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-91</a>
ATOMS89=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-92</a>
ATOMS90=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-93</a>
ATOMS91=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-94</a>
ATOMS92=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-95</a>
ATOMS93=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">psi-96</a>
... <a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_b_e_t_a.html">ALPHABETA</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_b_e_t_a.html">ALPHABETA</a> ...
LABEL=absccore
REFERENCE=0
ATOMS1=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-4</a>
ATOMS2=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-6</a>
ATOMS3=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-7</a>
ATOMS4=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-8</a>
ATOMS5=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-9</a>
ATOMS6=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-10</a>
ATOMS7=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-11</a>
ATOMS8=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-17</a>
ATOMS9=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-21</a>
ATOMS10=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-22</a>
ATOMS11=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-23</a>
ATOMS12=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-24</a>
ATOMS13=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-25</a>
ATOMS14=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-26</a>
ATOMS15=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-27</a>
ATOMS16=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-28</a>
ATOMS17=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-29</a>
ATOMS18=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-30</a>
ATOMS19=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-35</a>
ATOMS20=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-37</a>
ATOMS21=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-38</a>
ATOMS22=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-39</a>
ATOMS23=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-40</a>
ATOMS24=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-42</a>
ATOMS25=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-46</a>
ATOMS26=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-49</a>
ATOMS27=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-51</a>
ATOMS28=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-52</a>
ATOMS29=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-54</a>
ATOMS30=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-55</a>
ATOMS31=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-56</a>
ATOMS32=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-57</a>
ATOMS33=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-60</a>
ATOMS34=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-61</a>
ATOMS35=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-62</a>
ATOMS36=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-63</a>
ATOMS37=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-64</a>
ATOMS38=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-65</a>
ATOMS39=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-68</a>
ATOMS40=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-70</a>
ATOMS41=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-71</a>
ATOMS42=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-73</a>
ATOMS43=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-75</a>
ATOMS44=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-77</a>
ATOMS45=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-78</a>
ATOMS46=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-80</a>
ATOMS47=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-82</a>
ATOMS48=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-86</a>
ATOMS49=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-87</a>
ATOMS50=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-92</a>
ATOMS51=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-93</a>
ATOMS52=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-94</a>
ATOMS53=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-95</a>
... <a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_b_e_t_a.html">ALPHABETA</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_b_e_t_a.html">ALPHABETA</a> ...
LABEL=abscsurf
REFERENCE=0
ATOMS1=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-12</a>
ATOMS2=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-13</a>
ATOMS3=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-16</a>
ATOMS4=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-19</a>
ATOMS5=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-31</a>
ATOMS6=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-34</a>
ATOMS7=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-36</a>
ATOMS8=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-41</a>
ATOMS9=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-44</a>
ATOMS10=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-45</a>
ATOMS11=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-48</a>
ATOMS12=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-50</a>
ATOMS13=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-53</a>
ATOMS14=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-58</a>
ATOMS15=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-59</a>
ATOMS16=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-67</a>
ATOMS17=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-69</a>
ATOMS18=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-74</a>
ATOMS19=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-76</a>
ATOMS20=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-81</a>
ATOMS21=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-83</a>
ATOMS22=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-84</a>
ATOMS23=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-85</a>
ATOMS24=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-89</a>
ATOMS25=@<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">chi1-91</a>
... <a href="https://plumed.github.io/doc-master/user-doc/html/_a_l_p_h_a_b_e_t_a.html">ALPHABETA</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_b_m_e_t_a_d.html">PBMETAD</a> ...
LABEL=mm
ARG=ab,abback,absccore,abscsurf
ADAPTIVE=DIFF
SIGMA=2000
SIGMA_MIN=0.1,0.12,0.12,0.12 
PACE=200 HEIGHT=1.0 BIASFACTOR=20 
GRID_MIN=10,0,0,0 GRID_MAX=35,60,50,40 
INTERVAL_MIN=12,10,10,0 INTERVAL_MAX=30,42,40,33 
WALKERS_MPI
GRID_WSTRIDE=10000
<span style="color:blue">#GRID_RFILES=GRID.ab,GRID.abback,GRID.absccore,GRID.abscsurf</span>
... <a href="https://plumed.github.io/doc-master/user-doc/html/_p_b_m_e_t_a_d.html">PBMETAD</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=ab,abback,absccore AT=12,10,10 KAPPA=500,200,200
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=ab,abback,absccore AT=30,42,40 KAPPA=500,200,200

<span style="color:blue"># experimental data</span>
meta_ca: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_s2_b_a_c_k_b_o_n_e.html">CS2BACKBONE</a> ATOMS=protein DATADIR=data_ca/ TEMPLATE=template.pdb NOPBC DOSCORE OPTSIGMAMEAN=SEM AVERAGING=200 ARG=mm.bias REWEIGHT SIGMA_MIN=0.01 SIGMA_MAX=10 NOISETYPE=OUTLIERS
meta_cb: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_s2_b_a_c_k_b_o_n_e.html">CS2BACKBONE</a> ATOMS=protein DATADIR=data_cb/ TEMPLATE=template.pdb NOPBC DOSCORE OPTSIGMAMEAN=SEM AVERAGING=200 ARG=mm.bias REWEIGHT SIGMA_MIN=0.01 SIGMA_MAX=10 NOISETYPE=OUTLIERS
meta_co: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_s2_b_a_c_k_b_o_n_e.html">CS2BACKBONE</a> ATOMS=protein DATADIR=data_co/ TEMPLATE=template.pdb NOPBC DOSCORE OPTSIGMAMEAN=SEM AVERAGING=200 ARG=mm.bias REWEIGHT SIGMA_MIN=0.01 SIGMA_MAX=10 NOISETYPE=OUTLIERS
meta_hn: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_s2_b_a_c_k_b_o_n_e.html">CS2BACKBONE</a> ATOMS=protein DATADIR=data_hn/ TEMPLATE=template.pdb NOPBC DOSCORE OPTSIGMAMEAN=SEM AVERAGING=200 ARG=mm.bias REWEIGHT SIGMA_MIN=0.01 SIGMA_MAX=10 NOISETYPE=OUTLIERS
meta_nh: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_s2_b_a_c_k_b_o_n_e.html">CS2BACKBONE</a> ATOMS=protein DATADIR=data_nh/ TEMPLATE=template.pdb NOPBC DOSCORE OPTSIGMAMEAN=SEM AVERAGING=200 ARG=mm.bias REWEIGHT SIGMA_MIN=0.01 SIGMA_MAX=10 NOISETYPE=OUTLIERS

<a href="https://plumed.github.io/doc-master/user-doc/html/_b_i_a_s_v_a_l_u_e.html">BIASVALUE</a> ARG=meta_ca.score,meta_cb.score,meta_co.score,meta_hn.score,meta_nh.score

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=ab,abback,absccore,abscsurf,mm.bias FILE=COLVAR STRIDE=200
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=meta_ca.score,meta_ca.biasDer,meta_ca.weight,meta_ca.acceptSigma,meta_ca.sigmaMean,meta_ca.sigma FILE=MI_CS_CA.dat STRIDE=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=meta_cb.score,meta_cb.biasDer,meta_cb.weight,meta_cb.acceptSigma,meta_cb.sigmaMean,meta_cb.sigma FILE=MI_CS_CB.dat STRIDE=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=meta_co.score,meta_co.biasDer,meta_co.weight,meta_co.acceptSigma,meta_co.sigmaMean,meta_co.sigma FILE=MI_CS_CO.dat STRIDE=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=meta_hn.score,meta_hn.biasDer,meta_hn.weight,meta_hn.acceptSigma,meta_hn.sigmaMean,meta_hn.sigma FILE=MI_CS_HN.dat STRIDE=2000
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=meta_nh.score,meta_nh.biasDer,meta_nh.weight,meta_nh.acceptSigma,meta_nh.sigmaMean,meta_nh.sigma FILE=MI_CS_NH.dat STRIDE=2000

<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=10000
<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
</pre>{% endraw %}
