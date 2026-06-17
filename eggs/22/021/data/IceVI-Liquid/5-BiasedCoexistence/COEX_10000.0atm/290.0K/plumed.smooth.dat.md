**Project ID:** [plumID:22.021]({{ '/' | absolute_url }}eggs/22/021/)  
**Source:** IceVI-Liquid/5-BiasedCoexistence/COEX_10000.0atm/290.0K/plumed.smooth.dat  
**Originally used with PLUMED version:** 2.8  
**Stable:** [zipped raw stdout](plumed.smooth.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.smooth.dat.plumed.stderr.txt.zip) - [stderr](plumed.smooth.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.smooth.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.smooth.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.smooth.dat.plumed_master.stderr)  

{% raw %}
<div class="plumedInputContainer">
<div class="plumedpreheader">
<div class="headerInfo" id="value_details_data/IceVI-Liquid/5-BiasedCoexistence/COEX_10000.0atm/290.0K/plumed.smooth.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div class="containerBadge">
<div class="headerBadge"><a href="plumed.smooth.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-passing-green.svg" alt="tested onv2.10" /></a></div>
<div class="headerBadge"><a href="plumed.smooth.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></div>
</div>
</div>
<pre class="plumedlisting">
<span class="plumedtooltip" style="color:green">ENVIRONMENTSIMILARITY<span class="right">Measure how similar the environment around atoms is to that found in some reference crystal structure. <a href="https://www.plumed.org/doc-master/user-doc/html/ENVIRONMENTSIMILARITY" style="color:green">More details</a><i></i></span></span> ...
 <span class="plumedtooltip">SPECIES<span class="right">this keyword is used for colvars such as coordination number<i></i></span></span>=1-3840:3
 <span class="plumedtooltip">SIGMA<span class="right"> the width to use for the gaussian kernels<i></i></span></span>=0.0575
 <span class="plumedtooltip">CRYSTAL_STRUCTURE<span class="right"> Targeted crystal structure<i></i></span></span>=CUSTOM
 <span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/IceVI-Liquid/5-BiasedCoexistence/COEX_10000.0atm/290.0K/plumed.smooth.datrefcv" onclick='showPath("data/IceVI-Liquid/5-BiasedCoexistence/COEX_10000.0atm/290.0K/plumed.smooth.dat","data/IceVI-Liquid/5-BiasedCoexistence/COEX_10000.0atm/290.0K/plumed.smooth.datrefcv","data/IceVI-Liquid/5-BiasedCoexistence/COEX_10000.0atm/290.0K/plumed.smooth.datrefcv","brown")'>refcv</b>
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
 <span class="plumedtooltip">MORE_THAN<span class="right">calculate the number of variables that are more than a certain target value. Options for this keyword are explained in the documentation for <a href="https://www.plumed.org/doc-master/user-doc/html/MORE_THAN">MORE_THAN</a>.<i></i></span></span>={CUBIC D_0=0.60 D_MAX=0.85}
 <span class="plumedtooltip">MEAN<span class="right"> calculate the mean of all the quantities<i></i></span></span>
... ENVIRONMENTSIMILARITY
<span style="display:none;" id="data/IceVI-Liquid/5-BiasedCoexistence/COEX_10000.0atm/290.0K/plumed.smooth.datrefcv">The ENVIRONMENTSIMILARITY action with label <b>refcv</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">refcv.value</td><td>the environmental similar parameter for each of the input atoms</td></tr><tr><td width="5%">refcv.morethan</td><td>the number of colvars that have a value more than a threshold</td></tr><tr><td width="5%">refcv.mean</td><td>the mean of the colvars</td></tr></table></span></pre></div>

{% endraw %}
