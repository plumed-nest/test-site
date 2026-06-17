**Project ID:** [plumID:21.036]({{ '/' | absolute_url }}eggs/21/036/)  
**Source:** DHH1N_sampling/BEMD/CV8/plumed.7.dat  
**Originally used with PLUMED version:** 2.5.2  
**Stable:** [zipped raw stdout](plumed.7.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.7.dat.plumed.stderr.txt.zip) - [stderr](plumed.7.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.7.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.7.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.7.dat.plumed_master.stderr)  

{% raw %}
<div class="plumedInputContainer">
<div class="plumedpreheader">
<div class="headerInfo" id="value_details_data/DHH1N_sampling/BEMD/CV8/plumed.7.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div class="containerBadge">
<div class="headerBadge"><a href="plumed.7.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-passing-green.svg" alt="tested onv2.10" /></a></div>
<div class="headerBadge"><a href="plumed.7.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></div>
</div>
</div>
<pre class="plumedlisting">
<span style="color:blue" class="comment">#RESTART</span>
<br/><span class="plumedtooltip" style="color:green">MOLINFO<span class="right">This command is used to provide information on the molecules that are present in your system. <a href="https://www.plumed.org/doc-master/user-doc/html/MOLINFO" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">STRUCTURE<span class="right">a file in pdb format containing a reference structure<i></i></span></span>=Protein.pdb <span class="plumedtooltip">MOLTYPE<span class="right"> what kind of molecule is contained in the pdb file - usually not needed since protein/RNA/DNA are compatible<i></i></span></span>=protein

<span style="display:none;" id="data/DHH1N_sampling/BEMD/CV8/plumed.7.dat">The MOLINFO action with label <b></b> calculates something</span><span class="plumedtooltip" style="color:green">WHOLEMOLECULES<span class="right">This action is used to rebuild molecules that can become split by the periodic boundary conditions. <a href="https://www.plumed.org/doc-master/user-doc/html/WHOLEMOLECULES" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ENTITY0<span class="right">the atoms that make up a molecule that you wish to align<i></i></span></span>=1-709

<span class="plumedtooltip" style="color:green">RANDOM_EXCHANGES<span class="right">Set random pattern for exchanges. <a href="https://www.plumed.org/doc-master/user-doc/html/RANDOM_EXCHANGES" style="color:green">More details</a><i></i></span></span>
</pre></div>

{% endraw %}
