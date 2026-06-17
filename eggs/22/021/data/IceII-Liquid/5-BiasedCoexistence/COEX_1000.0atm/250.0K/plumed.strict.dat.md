**Project ID:** [plumID:22.021]({{ '/' | absolute_url }}eggs/22/021/)  
**Source:** IceII-Liquid/5-BiasedCoexistence/COEX_1000.0atm/250.0K/plumed.strict.dat  
**Originally used with PLUMED version:** 2.8  
**Stable:** [zipped raw stdout](plumed.strict.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.strict.dat.plumed.stderr.txt.zip) - [stderr](plumed.strict.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.strict.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.strict.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.strict.dat.plumed_master.stderr)  

{% raw %}
<div class="plumedInputContainer">
<div class="plumedpreheader">
<div class="headerInfo" id="value_details_data/IceII-Liquid/5-BiasedCoexistence/COEX_1000.0atm/250.0K/plumed.strict.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div class="containerBadge">
<div class="headerBadge"><a href="plumed.strict.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-passing-green.svg" alt="tested onv2.10" /></a></div>
<div class="headerBadge"><a href="plumed.strict.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></div>
</div>
</div>
<pre class="plumedlisting">
<span style="color:blue" class="comment"># Strict counting of molecules</span>
<span class="plumedtooltip" style="color:green">ENVIRONMENTSIMILARITY<span class="right">Measure how similar the environment around atoms is to that found in some reference crystal structure. <a href="https://www.plumed.org/doc-master/user-doc/html/ENVIRONMENTSIMILARITY" style="color:green">More details</a><i></i></span></span> ...
 <span class="plumedtooltip">SPECIES<span class="right">this keyword is used for colvars such as coordination number<i></i></span></span>=1-2592:3
 <span class="plumedtooltip">SIGMA<span class="right"> the width to use for the gaussian kernels<i></i></span></span>=0.0775
 <span class="plumedtooltip">CRYSTAL_STRUCTURE<span class="right"> Targeted crystal structure<i></i></span></span>=CUSTOM
 <span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/IceII-Liquid/5-BiasedCoexistence/COEX_1000.0atm/250.0K/plumed.strict.datrefcv2" onclick='showPath("data/IceII-Liquid/5-BiasedCoexistence/COEX_1000.0atm/250.0K/plumed.strict.dat","data/IceII-Liquid/5-BiasedCoexistence/COEX_1000.0atm/250.0K/plumed.strict.datrefcv2","data/IceII-Liquid/5-BiasedCoexistence/COEX_1000.0atm/250.0K/plumed.strict.datrefcv2","brown")'>refcv2</b>
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
 <span class="plumedtooltip">MORE_THAN<span class="right">calculate the number of variables that are more than a certain target value. Options for this keyword are explained in the documentation for <a href="https://www.plumed.org/doc-master/user-doc/html/MORE_THAN">MORE_THAN</a>.<i></i></span></span>={CUBIC D_0=0.96 D_MAX=0.96001}
 <span class="plumedtooltip">MEAN<span class="right"> calculate the mean of all the quantities<i></i></span></span>
... ENVIRONMENTSIMILARITY
<span style="display:none;" id="data/IceII-Liquid/5-BiasedCoexistence/COEX_1000.0atm/250.0K/plumed.strict.datrefcv2">The ENVIRONMENTSIMILARITY action with label <b>refcv2</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">refcv2.value</td><td>the environmental similar parameter for each of the input atoms</td></tr><tr><td width="5%">refcv2.morethan</td><td>the number of colvars that have a value more than a threshold</td></tr><tr><td width="5%">refcv2.mean</td><td>the mean of the colvars</td></tr></table></span></pre></div>

{% endraw %}
