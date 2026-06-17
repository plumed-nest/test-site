**Project ID:** [plumID:21.002]({{ '/' | absolute_url }}eggs/21/002/)  
**Source:** CoexistenceSimulations/CoexistenceNNP/IceIc/Analyze/plumed.dat  
**Originally used with PLUMED version:** 2.8  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div class="plumedInputContainer">
<div class="plumedpreheader">
<div class="headerInfo" id="value_details_data/CoexistenceSimulations/CoexistenceNNP/IceIc/Analyze/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div class="containerBadge">
<div class="headerBadge"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-passing-green.svg" alt="tested onv2.10" /></a></div>
<div class="headerBadge"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></div>
</div>
</div>
<pre class="plumedlisting">
<span style="color:blue" class="comment">#SETTINGS NREPLICAS=2</span>
<span class="plumedtooltip" style="color:blue"># vim:ft=plumed<span class="right">Enables syntax highlighting for PLUMED files in vim. See <a href="https://www.plumed.org/doc-master/user-doc/html/vim">here for more details. </a><i></i></span></span>
<br/><span class="plumedtooltip" style="color:green">ENVIRONMENTSIMILARITY<span class="right">Measure how similar the environment around atoms is to that found in some reference crystal structure. <a href="https://www.plumed.org/doc-master/user-doc/html/ENVIRONMENTSIMILARITY" style="color:green">More details</a><i></i></span></span> ...
 <span class="plumedtooltip">SPECIES<span class="right">this keyword is used for colvars such as coordination number<i></i></span></span>=1-1728:3
 <span class="plumedtooltip">SIGMA<span class="right"> the width to use for the gaussian kernels<i></i></span></span>=0.05
 <span class="plumedtooltip">CRYSTAL_STRUCTURE<span class="right"> Targeted crystal structure<i></i></span></span>=CUSTOM
 <span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/CoexistenceSimulations/CoexistenceNNP/IceIc/Analyze/plumed.datrefcv" onclick='showPath("data/CoexistenceSimulations/CoexistenceNNP/IceIc/Analyze/plumed.dat","data/CoexistenceSimulations/CoexistenceNNP/IceIc/Analyze/plumed.datrefcv","data/CoexistenceSimulations/CoexistenceNNP/IceIc/Analyze/plumed.datrefcv","brown")'>refcv</b>
 <span class="plumedtooltip">REFERENCE_1<span class="right">PDB files with relative distances from central atom<i></i></span></span>=env1c.pdb
 <span class="plumedtooltip">REFERENCE_2<span class="right">PDB files with relative distances from central atom<i></i></span></span>=env2c.pdb
 <span class="plumedtooltip">MORE_THAN<span class="right">calculate the number of variables that are more than a certain target value. Options for this keyword are explained in the documentation for <a href="https://www.plumed.org/doc-master/user-doc/html/MORE_THAN">MORE_THAN</a>.<i></i></span></span>={RATIONAL R_0=0.5 NN=8 MM=16}
 <span class="plumedtooltip">MEAN<span class="right"> calculate the mean of all the quantities<i></i></span></span>
... ENVIRONMENTSIMILARITY
<br/><span style="display:none;" id="data/CoexistenceSimulations/CoexistenceNNP/IceIc/Analyze/plumed.datrefcv">The ENVIRONMENTSIMILARITY action with label <b>refcv</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">refcv.value</td><td>the environmental similar parameter for each of the input atoms</td></tr><tr><td width="5%">refcv.morethan</td><td>the number of colvars that have a value more than a threshold</td></tr><tr><td width="5%">refcv.mean</td><td>the mean of the colvars</td></tr></table></span><b name="data/CoexistenceSimulations/CoexistenceNNP/IceIc/Analyze/plumed.datenergy" onclick='showPath("data/CoexistenceSimulations/CoexistenceNNP/IceIc/Analyze/plumed.dat","data/CoexistenceSimulations/CoexistenceNNP/IceIc/Analyze/plumed.datenergy","data/CoexistenceSimulations/CoexistenceNNP/IceIc/Analyze/plumed.datenergy","brown")'>energy</b>: <span class="plumedtooltip" style="color:green">ENERGY<span class="right">Calculate the total potential energy of the simulation box. <a href="https://www.plumed.org/doc-master/user-doc/html/ENERGY" style="color:green">More details</a><i></i></span></span>
<span style="display:none;" id="data/CoexistenceSimulations/CoexistenceNNP/IceIc/Analyze/plumed.datenergy">The ENERGY action with label <b>energy</b> calculates something</span><b name="data/CoexistenceSimulations/CoexistenceNNP/IceIc/Analyze/plumed.datvol" onclick='showPath("data/CoexistenceSimulations/CoexistenceNNP/IceIc/Analyze/plumed.dat","data/CoexistenceSimulations/CoexistenceNNP/IceIc/Analyze/plumed.datvol","data/CoexistenceSimulations/CoexistenceNNP/IceIc/Analyze/plumed.datvol","brown")'>vol</b>: <span class="plumedtooltip" style="color:green">VOLUME<span class="right">Calculate the volume the simulation box. <a href="https://www.plumed.org/doc-master/user-doc/html/VOLUME" style="color:green">More details</a><i></i></span></span>
<br/><span style="display:none;" id="data/CoexistenceSimulations/CoexistenceNNP/IceIc/Analyze/plumed.datvol">The VOLUME action with label <b>vol</b> calculates the volume of simulation box</span><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/PRINT" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=500  <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=* <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=COLVAR
</pre></div>

{% endraw %}
