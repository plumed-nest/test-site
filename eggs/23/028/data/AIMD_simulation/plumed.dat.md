**Project ID:** [plumID:23.028]({{ '/' | absolute_url }}eggs/23/028/)  
**Source:** AIMD_simulation/plumed.dat  
**Originally used with PLUMED version:** 2.9  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/AIMD_simulation/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<div class="tooltip" style="color:blue"># vim:ft=plumed<div class="right">Enables syntax highlighting for PLUMED files in vim. See <a href="https://www.plumed.org/doc-master/user-doc/html/_vim_syntax.html">here for more details. </a><i></i></div></div>
<span style="color:blue" class="comment">#RESTART</span>
<div class="tooltip" style="color:green">UNITS<div class="right">This command sets the internal units for the code. <a href="https://www.plumed.org/doc-master/user-doc/html/_u_n_i_t_s.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">LENGTH<div class="right">the units of lengths<i></i></div></div>=A
<span style="display:none;" id="data/AIMD_simulation/plumed.dat">The UNITS action with label <b></b> calculates something</span><b name="data/AIMD_simulation/plumed.datH" onclick='showPath("data/AIMD_simulation/plumed.dat","data/AIMD_simulation/plumed.datH","data/AIMD_simulation/plumed.datH","violet")'>H</b><span style="display:none;" id="data/AIMD_simulation/plumed.datH">The GROUP action with label <b>H</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">H</td><td width="5%"><font color="violet">atoms</font></td><td>indices of atoms specified in GROUP</td></tr></table></span>: <div class="tooltip" style="color:green">GROUP<div class="right">Define a group of atoms so that a particular list of atoms can be referenced with a single label in definitions of CVs or virtual atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_g_r_o_u_p.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the numerical indexes for the set of atoms in the group<i></i></div></div>=9,10,11,12,13,14,15,16,27,28,31,32,99,100,101,102,103,104,105,106,107,108,109,110,111,112,113,114,115,116,117,118,119,120,121,122,147,148,149,150,155,156,157,158,161,162,167,168,169,170,175,176,177,178,181,182,183,184,189,190,191,192,197,198,258,259,260
<b name="data/AIMD_simulation/plumed.datN" onclick='showPath("data/AIMD_simulation/plumed.dat","data/AIMD_simulation/plumed.datN","data/AIMD_simulation/plumed.datN","violet")'>N</b><span style="display:none;" id="data/AIMD_simulation/plumed.datN">The GROUP action with label <b>N</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">N</td><td width="5%"><font color="violet">atoms</font></td><td>indices of atoms specified in GROUP</td></tr></table></span>: <div class="tooltip" style="color:green">GROUP<div class="right">Define a group of atoms so that a particular list of atoms can be referenced with a single label in definitions of CVs or virtual atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_g_r_o_u_p.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the numerical indexes for the set of atoms in the group<i></i></div></div>=17,18,19,20,21,22,23,24,25,26,29,30,123,124,125,126,127,128,129,130,131,132,133,134,135,136,137,138,139,140,141,142,143,144,145,146,151,152,153,154,159,160,163,164,165,166,171,172,173,174,179,180,185,186,187,188,193,194,195,196,199,200,201,202,257
<b name="data/AIMD_simulation/plumed.datLi" onclick='showPath("data/AIMD_simulation/plumed.dat","data/AIMD_simulation/plumed.datLi","data/AIMD_simulation/plumed.datLi","violet")'>Li</b><span style="display:none;" id="data/AIMD_simulation/plumed.datLi">The GROUP action with label <b>Li</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">Li</td><td width="5%"><font color="violet">atoms</font></td><td>indices of atoms specified in GROUP</td></tr></table></span>: <div class="tooltip" style="color:green">GROUP<div class="right">Define a group of atoms so that a particular list of atoms can be referenced with a single label in definitions of CVs or virtual atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_g_r_o_u_p.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the numerical indexes for the set of atoms in the group<i></i></div></div>=1-8:1,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48,49,50,51,52,53,54,55,56,57,58,59,60,61,62,63,64,65,66,67,68,69,70,71,72,73,74,75,76,77,78,79,80,81,82,83,84,85,86,87,88,89,90,91,92,93,94,95,96,97,98,203,204,205,206,207,208,209,210,211,212,213,214,215,216,217,218,219,220,221,222,223,224,225,226,227,228,229,230,231,232,233,234,235,236,237,238,239,240,241,242,243,244,245,246,247,248,249,250,251,252,253,254,255,256
<br/><b name="data/AIMD_simulation/plumed.datene" onclick='showPath("data/AIMD_simulation/plumed.dat","data/AIMD_simulation/plumed.datene","data/AIMD_simulation/plumed.datene","black")'>ene</b><span style="display:none;" id="data/AIMD_simulation/plumed.datene">The ENERGY action with label <b>ene</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ene</td><td width="5%"><font color="black">scalar</font></td><td>the value calculated by this action</td></tr></table></span>: <div class="tooltip" style="color:green">ENERGY<div class="right">Calculate the total potential energy of the simulation box. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_n_e_r_g_y.html" style="color:green">More details</a><i></i></div></div>
<span id="data/AIMD_simulation/plumed.datmax_H_short"><b name="data/AIMD_simulation/plumed.datmax_H" onclick='showPath("data/AIMD_simulation/plumed.dat","data/AIMD_simulation/plumed.datmax_H","data/AIMD_simulation/plumed.datmax_H_shortcut","blue")'>max_H</b><span style="display:none;" id="data/AIMD_simulation/plumed.datmax_H_shortcut">The COORDINATIONNUMBER action with label <b>max_H</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">max_H</td><td width="5%"><font color="blue">vector</font></td><td>the value calculated by this action</td></tr><tr><td width="5%">max_H_max</td><td width="5%"><font color="black">scalar</font></td><td>the maximum colvar</td></tr></table></span>: <div class="tooltip" style="color:green">COORDINATIONNUMBER<div class="right">Calculate the coordination numbers of atoms so that you can then calculate functions of the distribution of This action is <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/AIMD_simulation/plumed.datmax_H");'>a shortcut</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_o_r_d_i_n_a_t_i_o_n_n_u_m_b_e_r.html">More details</a><i></i></div></div> <div class="tooltip">SPECIESA<div class="right">this keyword is used for colvars such as the coordination number<i></i></div></div>=<b name="data/AIMD_simulation/plumed.datH">H</b> <div class="tooltip">SPECIESB<div class="right">this keyword is used for colvars such as the coordination number<i></i></div></div>=<b name="data/AIMD_simulation/plumed.datLi">Li</b>,<b name="data/AIMD_simulation/plumed.datN">N</b> <div class="tooltip">SWITCH<div class="right">the switching function that it used in the construction of the contact matrix<i></i></div></div>={RATIONAL R_0=1.6 D_MAX=5}  <div class="tooltip">MAX<div class="right">calculate the maximum value<i></i></div></div>={BETA=0.05}
</span><span id="data/AIMD_simulation/plumed.datmax_H_long" style="display:none;"><span style="color:blue" class="comment"># PLUMED interprets the command:
</span><span class="toggler" style="color:red" onclick='toggleDisplay("data/AIMD_simulation/plumed.datmax_H")'># max_H: COORDINATIONNUMBER SPECIESA=H SPECIESB=Li,N SWITCH={RATIONAL R_0=1.6 D_MAX=5}  MAX={BETA=0.05}</span>
<span style="color:blue" class="comment"># as follows (Click the red comment above to revert to the short version of the input):</span>
<b name="data/AIMD_simulation/plumed.datmax_H_grp" onclick='showPath("data/AIMD_simulation/plumed.dat","data/AIMD_simulation/plumed.datmax_H_grp","data/AIMD_simulation/plumed.datmax_H_grp","violet")'>max_H_grp</b><span style="display:none;" id="data/AIMD_simulation/plumed.datmax_H_grp">The GROUP action with label <b>max_H_grp</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">max_H_grp</td><td width="5%"><font color="violet">atoms</font></td><td>indices of atoms specified in GROUP</td></tr></table></span>: <div class="tooltip" style="color:green">GROUP<div class="right">Define a group of atoms so that a particular list of atoms can be referenced with a single label in definitions of CVs or virtual atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_g_r_o_u_p.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the numerical indexes for the set of atoms in the group<i></i></div></div>=<b name="data/AIMD_simulation/plumed.datH">H</b> 
<b name="data/AIMD_simulation/plumed.datmax_H_mat" onclick='showPath("data/AIMD_simulation/plumed.dat","data/AIMD_simulation/plumed.datmax_H_mat","data/AIMD_simulation/plumed.datmax_H_mat","red")'>max_H_mat</b><span style="display:none;" id="data/AIMD_simulation/plumed.datmax_H_mat">The CONTACT_MATRIX action with label <b>max_H_mat</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">max_H_mat</td><td width="5%"><font color="red">matrix</font></td><td>a matrix containing the weights for the bonds between each pair of atoms</td></tr></table></span>: <div class="tooltip" style="color:green">CONTACT_MATRIX<div class="right">Adjacency matrix in which two atoms are adjacent if they are within a certain cutoff. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_t_a_c_t__m_a_t_r_i_x.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">SWITCH<div class="right">specify the switching function to use between two sets of indistinguishable atoms<i></i></div></div>={RATIONAL R_0=1.6 D_MAX=5} 
<b name="data/AIMD_simulation/plumed.datmax_H_ones" onclick='showPath("data/AIMD_simulation/plumed.dat","data/AIMD_simulation/plumed.datmax_H_ones","data/AIMD_simulation/plumed.datmax_H_ones","blue")'>max_H_ones</b><span style="display:none;" id="data/AIMD_simulation/plumed.datmax_H_ones">The CONSTANT action with label <b>max_H_ones</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">max_H_ones</td><td width="5%"><font color="blue">vector</font></td><td>the constant value that was read from the plumed input</td></tr></table></span>: <div class="tooltip" style="color:green">ONES<div class="right">Create a constant vector with all elements equal to one <a href="https://www.plumed.org/doc-master/user-doc/html/_o_n_e_s.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">SIZE<div class="right">the number of ones that you would like to create<i></i></div></div>=193
<b name="data/AIMD_simulation/plumed.datmax_H" onclick='showPath("data/AIMD_simulation/plumed.dat","data/AIMD_simulation/plumed.datmax_H","data/AIMD_simulation/plumed.datmax_H","blue")'>max_H</b><span style="display:none;" id="data/AIMD_simulation/plumed.datmax_H">The MATRIX_VECTOR_PRODUCT action with label <b>max_H</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">max_H</td><td width="5%"><font color="blue">vector</font></td><td>the vector that is obtained by taking the product between the matrix and the vector that were input</td></tr></table></span>: <div class="tooltip" style="color:green">MATRIX_VECTOR_PRODUCT<div class="right">Calculate the product of the matrix and the vector <a href="https://www.plumed.org/doc-master/user-doc/html/_m_a_t_r_i_x__v_e_c_t_o_r__p_r_o_d_u_c_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/AIMD_simulation/plumed.datmax_H_mat">max_H_mat</b>,<b name="data/AIMD_simulation/plumed.datmax_H_ones">max_H_ones</b> 
<b name="data/AIMD_simulation/plumed.datmax_H_caverage" onclick='showPath("data/AIMD_simulation/plumed.dat","data/AIMD_simulation/plumed.datmax_H_caverage","data/AIMD_simulation/plumed.datmax_H_caverage","black")'>max_H_caverage</b><span style="display:none;" id="data/AIMD_simulation/plumed.datmax_H_caverage">The MEAN action with label <b>max_H_caverage</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">max_H_caverage</td><td width="5%"><font color="black">scalar</font></td><td>the mean of all the elements in the input vector</td></tr></table></span>: <div class="tooltip" style="color:green">MEAN<div class="right">Calculate the arithmetic mean of the elements in a vector <a href="https://www.plumed.org/doc-master/user-doc/html/_m_e_a_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input to this function<i></i></div></div>=<b name="data/AIMD_simulation/plumed.datmax_H">max_H</b> <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO 
<b name="data/AIMD_simulation/plumed.datmax_H_me_max" onclick='showPath("data/AIMD_simulation/plumed.dat","data/AIMD_simulation/plumed.datmax_H_me_max","data/AIMD_simulation/plumed.datmax_H_me_max","blue")'>max_H_me_max</b><span style="display:none;" id="data/AIMD_simulation/plumed.datmax_H_me_max">The CUSTOM action with label <b>max_H_me_max</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">max_H_me_max</td><td width="5%"><font color="blue">vector</font></td><td>the vector obtained by doing an element-wise application of an arbitrary function to the input vectors</td></tr></table></span>: <div class="tooltip" style="color:green">CUSTOM<div class="right">Calculate a combination of variables using a custom expression. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_u_s_t_o_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input to this function<i></i></div></div>=<b name="data/AIMD_simulation/plumed.datmax_H">max_H</b> <div class="tooltip">FUNC<div class="right">the function you wish to evaluate<i></i></div></div>=exp(x/0.05 <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO 
<b name="data/AIMD_simulation/plumed.datmax_H_mec_max" onclick='showPath("data/AIMD_simulation/plumed.dat","data/AIMD_simulation/plumed.datmax_H_mec_max","data/AIMD_simulation/plumed.datmax_H_mec_max","black")'>max_H_mec_max</b><span style="display:none;" id="data/AIMD_simulation/plumed.datmax_H_mec_max">The SUM action with label <b>max_H_mec_max</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">max_H_mec_max</td><td width="5%"><font color="black">scalar</font></td><td>the sum of all the elements in the input vector</td></tr></table></span>: <div class="tooltip" style="color:green">SUM<div class="right">Calculate the sum of the arguments <a href="https://www.plumed.org/doc-master/user-doc/html/_s_u_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input to this function<i></i></div></div>=<b name="data/AIMD_simulation/plumed.datmax_H_me_max">max_H_me_max</b> <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO 
<b name="data/AIMD_simulation/plumed.datmax_H_max" onclick='showPath("data/AIMD_simulation/plumed.dat","data/AIMD_simulation/plumed.datmax_H_max","data/AIMD_simulation/plumed.datmax_H_max","black")'>max_H_max</b><span style="display:none;" id="data/AIMD_simulation/plumed.datmax_H_max">The CUSTOM action with label <b>max_H_max</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">max_H_max</td><td width="5%"><font color="black">scalar</font></td><td>an arbitrary function</td></tr></table></span>: <div class="tooltip" style="color:green">CUSTOM<div class="right">Calculate a combination of variables using a custom expression. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_u_s_t_o_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input to this function<i></i></div></div>=<b name="data/AIMD_simulation/plumed.datmax_H_mec_max">max_H_mec_max</b> <div class="tooltip">FUNC<div class="right">the function you wish to evaluate<i></i></div></div>=0.05*log(x <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO 
<span style="color:blue"># --- End of included input --- </span></span><br/><span id="data/AIMD_simulation/plumed.datdefghosta_short"><b name="data/AIMD_simulation/plumed.datghosta" onclick='showPath("data/AIMD_simulation/plumed.dat","data/AIMD_simulation/plumed.datghosta","data/AIMD_simulation/plumed.datghosta","violet")'>ghosta</b><span style="display:none;" id="data/AIMD_simulation/plumed.datghosta">The FIXEDATOM action with label <b>ghosta</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ghosta</td><td width="5%"><font color="violet">atoms</font></td><td>virtual atom calculated by FIXEDATOM action</td></tr></table></span>: <div class="tooltip" style="color:green">FIXEDATOM<div class="right">Add a virtual atom in a fixed position. This action has <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/AIMD_simulation/plumed.datdefghosta");'>hidden defaults</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_f_i_x_e_d_a_t_o_m.html">More details</a><i></i></div></div> <div class="tooltip">AT<div class="right">coordinates of the virtual atom<i></i></div></div>=0,0,20
</span><span id="data/AIMD_simulation/plumed.datdefghosta_long" style="display:none;"><b name="data/AIMD_simulation/plumed.datghosta" onclick='showPath("data/AIMD_simulation/plumed.dat","data/AIMD_simulation/plumed.datghosta","data/AIMD_simulation/plumed.datghosta","violet")'>ghosta</b>: <div class="tooltip" style="color:green">FIXEDATOM<div class="right">Add a virtual atom in a fixed position. This action uses the <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/AIMD_simulation/plumed.datdefghosta");'>defaults shown here</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_f_i_x_e_d_a_t_o_m.html">More details</a><i></i></div></div> <div class="tooltip">AT<div class="right">coordinates of the virtual atom<i></i></div></div>=0,0,20  <div class="tooltip">SET_MASS<div class="right"> mass of the virtual atom<i></i></div></div>=1 <div class="tooltip">SET_CHARGE<div class="right"> charge of the virtual atom<i></i></div></div>=0
</span><b name="data/AIMD_simulation/plumed.datNH3c" onclick='showPath("data/AIMD_simulation/plumed.dat","data/AIMD_simulation/plumed.datNH3c","data/AIMD_simulation/plumed.datNH3c","violet")'>NH3c</b><span style="display:none;" id="data/AIMD_simulation/plumed.datNH3c">The COM action with label <b>NH3c</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">NH3c</td><td width="5%"><font color="violet">atoms</font></td><td>virtual atom calculated by COM action</td></tr></table></span>: <div class="tooltip" style="color:green">COM<div class="right">Calculate the center of mass for a group of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the list of atoms which are involved the virtual atom's definition<i></i></div></div>=257-260
<b name="data/AIMD_simulation/plumed.datdNH3hosta" onclick='showPath("data/AIMD_simulation/plumed.dat","data/AIMD_simulation/plumed.datdNH3hosta","data/AIMD_simulation/plumed.datdNH3hosta","black")'>dNH3hosta</b><span style="display:none;" id="data/AIMD_simulation/plumed.datdNH3hosta">The DISTANCE action with label <b>dNH3hosta</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">dNH3hosta.x</td><td width="5%"><font color="black">scalar</font></td><td>the x-component of the vector connecting the two atoms</td></tr><tr><td width="5%">dNH3hosta.y</td><td width="5%"><font color="black">scalar</font></td><td>the y-component of the vector connecting the two atoms</td></tr><tr><td width="5%">dNH3hosta.z</td><td width="5%"><font color="black">scalar</font></td><td>the z-component of the vector connecting the two atoms</td></tr></table></span>: <div class="tooltip" style="color:green">DISTANCE<div class="right">Calculate the distance between a pair of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=<b name="data/AIMD_simulation/plumed.datghosta">ghosta</b>,<b name="data/AIMD_simulation/plumed.datNH3c">NH3c</b> <div class="tooltip">COMPONENTS<div class="right"> calculate the x, y and z components of the distance separately and store them as label<i></i></div></div>
<b name="data/AIMD_simulation/plumed.databs_dNH3hostaz" onclick='showPath("data/AIMD_simulation/plumed.dat","data/AIMD_simulation/plumed.databs_dNH3hostaz","data/AIMD_simulation/plumed.databs_dNH3hostaz","black")'>abs_dNH3hostaz</b><span style="display:none;" id="data/AIMD_simulation/plumed.databs_dNH3hostaz">The MATHEVAL action with label <b>abs_dNH3hostaz</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">abs_dNH3hostaz</td><td width="5%"><font color="black">scalar</font></td><td>an arbitrary function</td></tr></table></span>: <div class="tooltip" style="color:green">MATHEVAL<div class="right">An alias to the CUSTOM function that can also be used to calaculate combinations of variables using a custom expression. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_a_t_h_e_v_a_l.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input to this function<i></i></div></div>=<b name="data/AIMD_simulation/plumed.datdNH3hosta">dNH3hosta.z</b> <div class="tooltip">FUNC<div class="right">the function you wish to evaluate<i></i></div></div>=abs(x <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO
<b name="data/AIMD_simulation/plumed.datuwall1" onclick='showPath("data/AIMD_simulation/plumed.dat","data/AIMD_simulation/plumed.datuwall1","data/AIMD_simulation/plumed.datuwall1","black")'>uwall1</b><span style="display:none;" id="data/AIMD_simulation/plumed.datuwall1">The UPPER_WALLS action with label <b>uwall1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">uwall1.bias</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">uwall1.force2</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the squared force due to this bias potential</td></tr></table></span>: <div class="tooltip" style="color:green">UPPER_WALLS<div class="right">Defines a wall for the value of one or more collective variables, <a href="https://www.plumed.org/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the arguments on which the bias is acting<i></i></div></div>=<b name="data/AIMD_simulation/plumed.databs_dNH3hostaz">abs_dNH3hostaz</b> <div class="tooltip">AT<div class="right">the positions of the wall<i></i></div></div>=11.0 <div class="tooltip">KAPPA<div class="right">the force constant for the wall<i></i></div></div>=2000.0 <div class="tooltip">EXP<div class="right"> the powers for the walls<i></i></div></div>=2 
<br/><span id="data/AIMD_simulation/plumed.datdefopes2_short"><div class="tooltip" style="color:green">OPES_METAD<div class="right">On-the-fly probability enhanced sampling with metadynamics-like target distribution. This action has <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/AIMD_simulation/plumed.datdefopes2");'>hidden defaults</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s__m_e_t_a_d.html">More details</a><i></i></div></div> ... 
<div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/AIMD_simulation/plumed.datopes2" onclick='showPath("data/AIMD_simulation/plumed.dat","data/AIMD_simulation/plumed.datopes2","data/AIMD_simulation/plumed.datopes2","black")'>opes2</b><span style="display:none;" id="data/AIMD_simulation/plumed.datopes2">The OPES_METAD action with label <b>opes2</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">opes2.bias</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">opes2.rct</td><td width="5%"><font color="black">scalar</font></td><td>estimate of c(t). log(exp(beta V)/beta, should become flat as the simulation converges. Do NOT use for reweighting</td></tr><tr><td width="5%">opes2.zed</td><td width="5%"><font color="black">scalar</font></td><td>estimate of Z_n. should become flat once no new CV-space region is explored</td></tr><tr><td width="5%">opes2.neff</td><td width="5%"><font color="black">scalar</font></td><td>effective sample size</td></tr><tr><td width="5%">opes2.nker</td><td width="5%"><font color="black">scalar</font></td><td>total number of compressed kernels used to represent the bias</td></tr></table></span>
<div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/AIMD_simulation/plumed.datmax_H">max_H.max</b> 
<div class="tooltip">PACE<div class="right">the frequency for kernel deposition<i></i></div></div>=50
<div class="tooltip">BARRIER<div class="right">the free energy barrier to be overcome<i></i></div></div>=100 <span style="color:blue" class="comment"># #BIASFACTOR=20 # #KERNEL_CUTOFF=7.5 </span>
<div class="tooltip">TEMP<div class="right"> temperature<i></i></div></div>=750
... OPES_METAD
</span><span id="data/AIMD_simulation/plumed.datdefopes2_long" style="display:none;"><div class="tooltip" style="color:green">OPES_METAD<div class="right">On-the-fly probability enhanced sampling with metadynamics-like target distribution. This action uses the <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/AIMD_simulation/plumed.datdefopes2");'>defaults shown here</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_o_p_e_s__m_e_t_a_d.html">More details</a><i></i></div></div> ... 
<div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/AIMD_simulation/plumed.datopes2" onclick='showPath("data/AIMD_simulation/plumed.dat","data/AIMD_simulation/plumed.datopes2","data/AIMD_simulation/plumed.datopes2","black")'>opes2</b>
<div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/AIMD_simulation/plumed.datmax_H">max_H.max</b> 
<div class="tooltip">PACE<div class="right">the frequency for kernel deposition<i></i></div></div>=50
<div class="tooltip">BARRIER<div class="right">the free energy barrier to be overcome<i></i></div></div>=100 <span style="color:blue" class="comment"># #BIASFACTOR=20 # #KERNEL_CUTOFF=7.5 </span>
<div class="tooltip">TEMP<div class="right"> temperature<i></i></div></div>=750
 <div class="tooltip">SIGMA<div class="right"> the initial widths of the kernels<i></i></div></div>=ADAPTIVE <div class="tooltip">COMPRESSION_THRESHOLD<div class="right"> merge kernels if closer than this threshold, in units of sigma<i></i></div></div>=1 <div class="tooltip">FILE<div class="right"> a file in which the list of all deposited kernels is stored<i></i></div></div>=KERNELS
... OPES_METAD
</span><br/><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div> <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=colvar <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=2
<div class="tooltip" style="color:green">FLUSH<div class="right">This command instructs plumed to flush all the open files with a user specified frequency. <a href="https://www.plumed.org/doc-master/user-doc/html/_f_l_u_s_h.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">STRIDE<div class="right">the frequency with which all the open files should be flushed<i></i></div></div>=2
</pre>
{% endraw %}