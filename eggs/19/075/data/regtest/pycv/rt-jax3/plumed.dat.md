**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
**Source:** regtest/pycv/rt-jax3/plumed.dat  
**Originally used with PLUMED version:** 2.5.2-mod  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div class="plumedInputContainer">
<div class="plumedpreheader">
<div class="headerInfo" id="value_details_data/regtest/pycv/rt-jax3/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div class="containerBadge">
<div class="headerBadge"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-failed-red.svg" alt="tested onv2.10" /></a></div>
<div class="headerBadge"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-failed-red.svg" alt="tested onmaster" /></a></div>
</div>
</div>
<pre class="plumedlisting">
<b name="data/regtest/pycv/rt-jax3/plumed.datr" onclick='showPath("data/regtest/pycv/rt-jax3/plumed.dat","data/regtest/pycv/rt-jax3/plumed.datr","data/regtest/pycv/rt-jax3/plumed.datr","brown")'>r</b>:  <span class="plumedtooltip" style="color:green">PYTHONCV<span class="right">This action is not part of PLUMED and was included by using a LOAD command <a href="https://www.plumed.org/doc-master/user-doc/html/LOAD" style="color:green">More details</a><i></i></span></span> ATOMS=1,2,3 IMPORT=curvature FUNCTION=r
<b name="data/regtest/pycv/rt-jax3/plumed.datir" onclick='showPath("data/regtest/pycv/rt-jax3/plumed.dat","data/regtest/pycv/rt-jax3/plumed.datir","data/regtest/pycv/rt-jax3/plumed.datir","brown")'>ir</b>: <span class="plumedtooltip" style="color:green">PYTHONFUNCTION<span class="right">This action is not part of PLUMED and was included by using a LOAD command <a href="https://www.plumed.org/doc-master/user-doc/html/LOAD" style="color:green">More details</a><i></i></span></span> ARG=r IMPORT=curvature FUNCTION=inv  PERIODIC=NO


<span class="plumedtooltip" style="color:green">DUMPDERIVATIVES<span class="right">Dump the derivatives with respect to the input parameters for scalar values (generally CVs, functions or biases). <a href="https://www.plumed.org/doc-master/user-doc/html/DUMPDERIVATIVES" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the labels of the values whose derivatives should be output<i></i></span></span>=r  <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output the derivatives<i></i></span></span>=GRADIENT_r  <span class="plumedtooltip">FMT<span class="right"> the format with which the derivatives should be output<i></i></span></span>=%8.4f
<span style="color:blue" class="comment"># DUMPDERIVATIVES ARG=ir FILE=GRADIENT_ir FMT=%8.4f</span>
<br/><span style="display:none;" id="data/regtest/pycv/rt-jax3/plumed.dat">The DUMPDERIVATIVES action with label <b></b> calculates something</span><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/PRINT" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=COLVAR <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=* <span class="plumedtooltip">FMT<span class="right"> the format that should be used to output real numbers<i></i></span></span>=%8.4f
</pre></div>

{% endraw %}
