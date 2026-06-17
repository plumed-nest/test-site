**Project ID:** [plumID:23.001]({{ '/' | absolute_url }}eggs/23/001/)  
**Source:** EnhancedCoexistence/Liq-V/3-BiasedCoexistence/COEX_5000.0atm/245.0K/plumed.order.dat  
**Originally used with PLUMED version:** 2.8  
**Stable:** [zipped raw stdout](plumed.order.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.order.dat.plumed.stderr.txt.zip) - [stderr](plumed.order.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.order.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.order.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.order.dat.plumed_master.stderr)  

{% raw %}
<div class="plumedInputContainer">
<div class="plumedpreheader">
<div class="headerInfo" id="value_details_data/EnhancedCoexistence/Liq-V/3-BiasedCoexistence/COEX_5000.0atm/245.0K/plumed.order.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div class="containerBadge">
<div class="headerBadge"><a href="plumed.order.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-passing-green.svg" alt="tested onv2.10" /></a></div>
<div class="headerBadge"><a href="plumed.order.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></div>
</div>
</div>
<pre class="plumedlisting">
<span class="plumedtooltip" style="color:green">ENVIRONMENTSIMILARITY<span class="right">Measure how similar the environment around atoms is to that found in some reference crystal structure. <a href="https://www.plumed.org/doc-master/user-doc/html/ENVIRONMENTSIMILARITY" style="color:green">More details</a><i></i></span></span> ...
 <span class="plumedtooltip">SPECIES<span class="right">this keyword is used for colvars such as coordination number<i></i></span></span>=1-2016:3
 <span class="plumedtooltip">SIGMA<span class="right"> the width to use for the gaussian kernels<i></i></span></span>=0.0725
 <span class="plumedtooltip">CRYSTAL_STRUCTURE<span class="right"> Targeted crystal structure<i></i></span></span>=CUSTOM
 <span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/EnhancedCoexistence/Liq-V/3-BiasedCoexistence/COEX_5000.0atm/245.0K/plumed.order.datrefcv" onclick='showPath("data/EnhancedCoexistence/Liq-V/3-BiasedCoexistence/COEX_5000.0atm/245.0K/plumed.order.dat","data/EnhancedCoexistence/Liq-V/3-BiasedCoexistence/COEX_5000.0atm/245.0K/plumed.order.datrefcv","data/EnhancedCoexistence/Liq-V/3-BiasedCoexistence/COEX_5000.0atm/245.0K/plumed.order.datrefcv","brown")'>refcv</b>
 <span class="plumedtooltip">REFERENCE_1<span class="right">PDB files with relative distances from central atom<i></i></span></span>=env1.pdb
 <span class="plumedtooltip">REFERENCE_2<span class="right">PDB files with relative distances from central atom<i></i></span></span>=env2.pdb
 <span class="plumedtooltip">REFERENCE_3<span class="right">PDB files with relative distances from central atom<i></i></span></span>=env3.pdb
 <span class="plumedtooltip">REFERENCE_4<span class="right">PDB files with relative distances from central atom<i></i></span></span>=env4.pdb
 <span class="plumedtooltip">REFERENCE_5<span class="right">PDB files with relative distances from central atom<i></i></span></span>=env5.pdb
 <span class="plumedtooltip">REFERENCE_6<span class="right">PDB files with relative distances from central atom<i></i></span></span>=env6.pdb
 <span class="plumedtooltip">REFERENCE_7<span class="right">PDB files with relative distances from central atom<i></i></span></span>=env7.pdb
 <span class="plumedtooltip">REFERENCE_8<span class="right">PDB files with relative distances from central atom<i></i></span></span>=env8.pdb
 <span class="plumedtooltip">REFERENCE_9<span class="right">PDB files with relative distances from central atom<i></i></span></span>=env9.pdb
 <span class="plumedtooltip">REFERENCE_10<span class="right">PDB files with relative distances from central atom<i></i></span></span>=env10.pdb
 <span class="plumedtooltip">REFERENCE_11<span class="right">PDB files with relative distances from central atom<i></i></span></span>=env11.pdb
 <span class="plumedtooltip">REFERENCE_12<span class="right">PDB files with relative distances from central atom<i></i></span></span>=env12.pdb
 <span class="plumedtooltip">REFERENCE_13<span class="right">PDB files with relative distances from central atom<i></i></span></span>=env13.pdb
 <span class="plumedtooltip">REFERENCE_14<span class="right">PDB files with relative distances from central atom<i></i></span></span>=env14.pdb
 <span class="plumedtooltip">REFERENCE_15<span class="right">PDB files with relative distances from central atom<i></i></span></span>=env15.pdb
 <span class="plumedtooltip">REFERENCE_16<span class="right">PDB files with relative distances from central atom<i></i></span></span>=env16.pdb
 <span class="plumedtooltip">REFERENCE_17<span class="right">PDB files with relative distances from central atom<i></i></span></span>=env17.pdb
 <span class="plumedtooltip">REFERENCE_18<span class="right">PDB files with relative distances from central atom<i></i></span></span>=env18.pdb
 <span class="plumedtooltip">REFERENCE_19<span class="right">PDB files with relative distances from central atom<i></i></span></span>=env19.pdb
 <span class="plumedtooltip">REFERENCE_20<span class="right">PDB files with relative distances from central atom<i></i></span></span>=env20.pdb
 <span class="plumedtooltip">REFERENCE_21<span class="right">PDB files with relative distances from central atom<i></i></span></span>=env21.pdb
 <span class="plumedtooltip">REFERENCE_22<span class="right">PDB files with relative distances from central atom<i></i></span></span>=env22.pdb
 <span class="plumedtooltip">REFERENCE_23<span class="right">PDB files with relative distances from central atom<i></i></span></span>=env23.pdb
 <span class="plumedtooltip">REFERENCE_24<span class="right">PDB files with relative distances from central atom<i></i></span></span>=env24.pdb
 <span class="plumedtooltip">REFERENCE_25<span class="right">PDB files with relative distances from central atom<i></i></span></span>=env25.pdb
 <span class="plumedtooltip">REFERENCE_26<span class="right">PDB files with relative distances from central atom<i></i></span></span>=env26.pdb
 <span class="plumedtooltip">REFERENCE_27<span class="right">PDB files with relative distances from central atom<i></i></span></span>=env27.pdb
 <span class="plumedtooltip">REFERENCE_28<span class="right">PDB files with relative distances from central atom<i></i></span></span>=env28.pdb
 <span class="plumedtooltip">MORE_THAN1<span class="right">calculate the number of variables that are more than a certain target value. Options for this keyword are explained in the documentation for <a href="https://www.plumed.org/doc-master/user-doc/html/MORE_THAN">MORE_THAN</a>.<i></i></span></span>={CUBIC D_0=0.75 D_MAX=1.06}
 <span class="plumedtooltip">MORE_THAN2<span class="right">calculate the number of variables that are more than a certain target value. Options for this keyword are explained in the documentation for <a href="https://www.plumed.org/doc-master/user-doc/html/MORE_THAN">MORE_THAN</a>.<i></i></span></span>={CUBIC D_0=0.8960 D_MAX=0.8961}
 <span class="plumedtooltip">MEAN<span class="right"> calculate the mean of all the quantities<i></i></span></span>
... ENVIRONMENTSIMILARITY
<span style="display:none;" id="data/EnhancedCoexistence/Liq-V/3-BiasedCoexistence/COEX_5000.0atm/245.0K/plumed.order.datrefcv">The ENVIRONMENTSIMILARITY action with label <b>refcv</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">refcv.value</td><td>the environmental similar parameter for each of the input atoms</td></tr><tr><td width="5%">refcv.mean</td><td>the mean of the colvars</td></tr></table></span></pre></div>

{% endraw %}
