**Project ID:** [plumID:22.021]({{ '/' | absolute_url }}eggs/22/021/)  
**Source:** IceIII-Liquid/5-BiasedCoexistence/COEX_2000.0atm/270.0K/plumed.strict.dat  
**Originally used with PLUMED version:** 2.8  
**Stable:** [zipped raw stdout](plumed.strict.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.strict.dat.plumed.stderr.txt.zip) - [stderr](plumed.strict.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.strict.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.strict.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.strict.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/IceIII-Liquid/5-BiasedCoexistence/COEX_2000.0atm/270.0K/plumed.strict.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.strict.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.strict.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue"># Strict counting of molecules</span>
<div class="tooltip" style="color:green">ENVIRONMENTSIMILARITY<div class="right">Measure how similar the environment around atoms is to that found in some reference crystal structure. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_n_v_i_r_o_n_m_e_n_t_s_i_m_i_l_a_r_i_t_y.html" style="color:green">More details</a><i></i></div></div> ...
 <div class="tooltip">SPECIES<div class="right">this keyword is used for colvars such as coordination number<i></i></div></div>=1-2268:3
 <div class="tooltip">SIGMA<div class="right"> Broadening parameter<i></i></div></div>=0.0675
 <div class="tooltip">CRYSTAL_STRUCTURE<div class="right"> Targeted crystal structure<i></i></div></div>=CUSTOM
 <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/IceIII-Liquid/5-BiasedCoexistence/COEX_2000.0atm/270.0K/plumed.strict.datrefcv2" onclick='showPath("data/IceIII-Liquid/5-BiasedCoexistence/COEX_2000.0atm/270.0K/plumed.strict.dat","data/IceIII-Liquid/5-BiasedCoexistence/COEX_2000.0atm/270.0K/plumed.strict.datrefcv2")'>refcv2</b>
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
 <div class="tooltip">REFERENCE_11<div class="right">PDB files with relative distances from central atom<i></i></div></div>=env11.pdb
 <div class="tooltip">REFERENCE_12<div class="right">PDB files with relative distances from central atom<i></i></div></div>=env12.pdb
 <div class="tooltip">MORE_THAN<div class="right">calculate the number of variables more than a certain target value<i></i></div></div>={CUBIC D_0=0.7675 D_MAX=0.7675001}
 <div class="tooltip">MEAN<div class="right">take the mean of these variables<i></i></div></div>
... ENVIRONMENTSIMILARITY
<span style="display:none;" id="data/IceIII-Liquid/5-BiasedCoexistence/COEX_2000.0atm/270.0K/plumed.strict.datrefcv2">The ENVIRONMENTSIMILARITY action with label <b>refcv2</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">refcv2.mean</td><td>the mean value</td></tr><tr><td width="5%">refcv2.morethan</td><td>the number of values more than a target value</td></tr></table></span></pre>
{% endraw %}
