**Project ID:** [plumID:23.001]({{ '/' | absolute_url }}eggs/23/001/)  
**Source:** EnhancedCoexistence/Liq-VI/4-BiasedCoexistence/COEX_7000.0atm/245.0K/plumed.order.dat  
**Originally used with PLUMED version:** 2.8  
**Stable:** [zipped raw stdout](plumed.order.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.order.dat.plumed.stderr.txt.zip) - [stderr](plumed.order.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.order.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.order.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.order.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/EnhancedCoexistence/Liq-VI/4-BiasedCoexistence/COEX_7000.0atm/245.0K/plumed.order.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.order.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.order.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue">#7000atm_255K</span>
<span style="color:blue">#sigma: 0.055</span>
<span style="color:blue">#Liquid max: 0.46</span>
<span style="color:blue">#Ice max: 0.9325</span>
<span style="color:blue">#Midpoint between distribitions: 0.7275</span>
<br/><div class="tooltip" style="color:green">ENVIRONMENTSIMILARITY<div class="right">Measure how similar the environment around atoms is to that found in some reference crystal structure. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_n_v_i_r_o_n_m_e_n_t_s_i_m_i_l_a_r_i_t_y.html" style="color:green">More details</a><i></i></div></div> ...
 <div class="tooltip">SPECIES<div class="right">this keyword is used for colvars such as coordination number<i></i></div></div>=1-3840:3
 <div class="tooltip">SIGMA<div class="right"> Broadening parameter<i></i></div></div>=0.055
 <div class="tooltip">CRYSTAL_STRUCTURE<div class="right"> Targeted crystal structure<i></i></div></div>=CUSTOM
 <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/EnhancedCoexistence/Liq-VI/4-BiasedCoexistence/COEX_7000.0atm/245.0K/plumed.order.datrefcv" onclick='showPath("data/EnhancedCoexistence/Liq-VI/4-BiasedCoexistence/COEX_7000.0atm/245.0K/plumed.order.dat","data/EnhancedCoexistence/Liq-VI/4-BiasedCoexistence/COEX_7000.0atm/245.0K/plumed.order.datrefcv")'>refcv</b>
 <div class="tooltip">REFERENCE_1<div class="right">PDB files with relative distances from central atom<i></i></div></div>=env1.pdb
 <div class="tooltip">REFERENCE_2<div class="right">PDB files with relative distances from central atom<i></i></div></div>=env2.pdb
 <div class="tooltip">REFERENCE_3<div class="right">PDB files with relative distances from central atom<i></i></div></div>=env3.pdb
 <div class="tooltip">REFERENCE_4<div class="right">PDB files with relative distances from central atom<i></i></div></div>=env4.pdb
 <div class="tooltip">REFERENCE_5<div class="right">PDB files with relative distances from central atom<i></i></div></div>=env5.pdb
 <div class="tooltip">REFERENCE_6<div class="right">PDB files with relative distances from central atom<i></i></div></div>=env6.pdb
 <div class="tooltip">REFERENCE_7<div class="right">PDB files with relative distances from central atom<i></i></div></div>=env7.pdb
 <div class="tooltip">REFERENCE_8<div class="right">PDB files with relative distances from central atom<i></i></div></div>=env8.pdb
 <div class="tooltip">REFERENCE_9<div class="right">PDB files with relative distances from central atom<i></i></div></div>=env9.pdb
 <div class="tooltip">REFERENCE_10<div class="right">PDB files with relative distances from central atom<i></i></div></div>=env10.pdb
 <div class="tooltip">MORE_THAN1<div class="right">calculate the number of variables more than a certain target value<i></i></div></div>={CUBIC D_0=0.46 D_MAX=0.9325}
 <div class="tooltip">MORE_THAN2<div class="right">calculate the number of variables more than a certain target value<i></i></div></div>={CUBIC D_0=0.72750 D_MAX=0.72751}
 <div class="tooltip">MEAN<div class="right">take the mean of these variables<i></i></div></div>
... ENVIRONMENTSIMILARITY
<span style="display:none;" id="data/EnhancedCoexistence/Liq-VI/4-BiasedCoexistence/COEX_7000.0atm/245.0K/plumed.order.datrefcv">The ENVIRONMENTSIMILARITY action with label <b>refcv</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">refcv.mean</td><td>the mean value</td></tr></table></span></pre>
{% endraw %}
