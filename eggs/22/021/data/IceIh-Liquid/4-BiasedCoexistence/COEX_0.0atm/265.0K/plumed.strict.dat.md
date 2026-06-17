**Project ID:** [plumID:22.021]({{ '/' | absolute_url }}eggs/22/021/)  
**Source:** IceIh-Liquid/4-BiasedCoexistence/COEX_0.0atm/265.0K/plumed.strict.dat  
**Originally used with PLUMED version:** 2.8  
**Stable:** [zipped raw stdout](plumed.strict.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.strict.dat.plumed.stderr.txt.zip) - [stderr](plumed.strict.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.strict.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.strict.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.strict.dat.plumed_master.stderr)  

{% raw %}
<div class="plumedInputContainer">
<div class="plumedpreheader">
<div class="headerInfo" id="value_details_data/IceIh-Liquid/4-BiasedCoexistence/COEX_0.0atm/265.0K/plumed.strict.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div class="containerBadge">
<div class="headerBadge"><a href="plumed.strict.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-passing-green.svg" alt="tested onv2.10" /></a></div>
<div class="headerBadge"><a href="plumed.strict.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></div>
</div>
</div>
<pre class="plumedlisting">
<span style="color:blue" class="comment"># Strict CV</span>
<span class="plumedtooltip" style="color:green">ENVIRONMENTSIMILARITY<span class="right">Measure how similar the environment around atoms is to that found in some reference crystal structure. <a href="https://www.plumed.org/doc-master/user-doc/html/ENVIRONMENTSIMILARITY" style="color:green">More details</a><i></i></span></span> ...
 <span class="plumedtooltip">SPECIES<span class="right">this keyword is used for colvars such as coordination number<i></i></span></span>=1-1728:3
 <span class="plumedtooltip">SIGMA<span class="right"> the width to use for the gaussian kernels<i></i></span></span>=0.070
 <span class="plumedtooltip">CRYSTAL_STRUCTURE<span class="right"> Targeted crystal structure<i></i></span></span>=CUSTOM
 <span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/IceIh-Liquid/4-BiasedCoexistence/COEX_0.0atm/265.0K/plumed.strict.datrefcv2" onclick='showPath("data/IceIh-Liquid/4-BiasedCoexistence/COEX_0.0atm/265.0K/plumed.strict.dat","data/IceIh-Liquid/4-BiasedCoexistence/COEX_0.0atm/265.0K/plumed.strict.datrefcv2","data/IceIh-Liquid/4-BiasedCoexistence/COEX_0.0atm/265.0K/plumed.strict.datrefcv2","brown")'>refcv2</b>
 <span class="plumedtooltip">REFERENCE_1<span class="right">PDB files with relative distances from central atom<i></i></span></span>=env1h.pdb
 <span class="plumedtooltip">REFERENCE_2<span class="right">PDB files with relative distances from central atom<i></i></span></span>=env2h.pdb
 <span class="plumedtooltip">REFERENCE_3<span class="right">PDB files with relative distances from central atom<i></i></span></span>=env3h.pdb
 <span class="plumedtooltip">REFERENCE_4<span class="right">PDB files with relative distances from central atom<i></i></span></span>=env4h.pdb
 <span class="plumedtooltip">MORE_THAN<span class="right">calculate the number of variables that are more than a certain target value. Options for this keyword are explained in the documentation for <a href="https://www.plumed.org/doc-master/user-doc/html/MORE_THAN">MORE_THAN</a>.<i></i></span></span>={CUBIC D_0=0.7275 D_MAX=0.7276} <span style="color:blue" class="comment"># Change this value to the point where distributions meet</span>
 <span class="plumedtooltip">MEAN<span class="right"> calculate the mean of all the quantities<i></i></span></span>
... ENVIRONMENTSIMILARITY
<span style="display:none;" id="data/IceIh-Liquid/4-BiasedCoexistence/COEX_0.0atm/265.0K/plumed.strict.datrefcv2">The ENVIRONMENTSIMILARITY action with label <b>refcv2</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">refcv2.value</td><td>the environmental similar parameter for each of the input atoms</td></tr><tr><td width="5%">refcv2.morethan</td><td>the number of colvars that have a value more than a threshold</td></tr><tr><td width="5%">refcv2.mean</td><td>the mean of the colvars</td></tr></table></span></pre></div>

{% endraw %}
