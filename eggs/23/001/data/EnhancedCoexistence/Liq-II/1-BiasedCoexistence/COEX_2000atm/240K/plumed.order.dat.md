**Project ID:** [plumID:23.001]({{ '/' | absolute_url }}eggs/23/001/)  
**Source:** EnhancedCoexistence/Liq-II/1-BiasedCoexistence/COEX_2000atm/240K/plumed.order.dat  
**Originally used with PLUMED version:** 2.8  
**Stable:** [zipped raw stdout](plumed.order.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.order.dat.plumed.stderr.txt.zip) - [stderr](plumed.order.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.order.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.order.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.order.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/EnhancedCoexistence/Liq-II/1-BiasedCoexistence/COEX_2000atm/240K/plumed.order.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.order.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-failed-red.svg" alt="tested onv2.10" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.order.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-failed-red.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span class="plumedtooltip" style="color:green">ENVIRONMENTSIMILARITY<span class="right">Measure how similar the environment around atoms is to that found in some reference crystal structure. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_n_v_i_r_o_n_m_e_n_t_s_i_m_i_l_a_r_i_t_y.html" style="color:green">More details</a><i></i></span></span> ...
 <span class="plumedtooltip">SPECIES<span class="right">this keyword is used for colvars such as coordination number<i></i></span></span>=1-1152:3
 <span class="plumedtooltip">SIGMA<span class="right"> the width to use for the gaussian kernels<i></i></span></span>=0.05
 <span class="plumedtooltip">CRYSTAL_STRUCTURE<span class="right"> Targeted crystal structure<i></i></span></span>=CUSTOM
 <span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/EnhancedCoexistence/Liq-II/1-BiasedCoexistence/COEX_2000atm/240K/plumed.order.datrefcv" onclick='showPath("data/EnhancedCoexistence/Liq-II/1-BiasedCoexistence/COEX_2000atm/240K/plumed.order.dat","data/EnhancedCoexistence/Liq-II/1-BiasedCoexistence/COEX_2000atm/240K/plumed.order.datrefcv","data/EnhancedCoexistence/Liq-II/1-BiasedCoexistence/COEX_2000atm/240K/plumed.order.datrefcv","brown")'>refcv</b>
REPLACE_REFERENCE
 <span class="plumedtooltip">MORE_THAN1<span class="right">calculate the number of variables that are more than a certain target value<i></i></span></span>={CUBIC D_0=4.792375 D_MAX=4.888625}
 <span class="plumedtooltip">MORE_THAN2<span class="right">calculate the number of variables that are more than a certain target value<i></i></span></span>={CUBIC D_0=4.850125 D_MAX=4.850225}
 <span class="plumedtooltip">MEAN<span class="right"> calculate the mean of all the quantities<i></i></span></span>
 <span class="plumedtooltip">ATOM_NAMES_FILE<span class="right">PDB file with atom names for all atoms in SPECIES<i></i></span></span>=ice.pdb

... ENVIRONMENTSIMILARITY
<span style="display:none;" id="data/EnhancedCoexistence/Liq-II/1-BiasedCoexistence/COEX_2000atm/240K/plumed.order.datrefcv">The ENVIRONMENTSIMILARITY action with label <b>refcv</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">refcv.value</td><td>the environmental similar parameter for each of the input atoms</td></tr><tr><td width="5%">refcv.mean</td><td>the mean of the colvars</td></tr></table></span></pre>
{% endraw %}
