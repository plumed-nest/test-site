**Project ID:** [plumID:25.030]({{ '/' | absolute_url }}eggs/25/030/)  
**Source:** plumed_mtd.dat  
**Originally used with PLUMED version:** 2.5.2  
**Stable:** [zipped raw stdout](plumed_mtd.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_mtd.dat.plumed.stderr.txt.zip) - [stderr](plumed_mtd.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed_mtd.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_mtd.dat.plumed_master.stderr.txt.zip) - [stderr](plumed_mtd.dat.plumed_master.stderr)  

{% raw %}
<div class="plumedInputContainer">
<div class="plumedpreheader">
<div class="headerInfo" id="value_details_data/plumed_mtd.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div class="containerBadge">
<div class="headerBadge"><a href="plumed_mtd.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-failed-red.svg" alt="tested onv2.10" /></a></div>
<div class="headerBadge"><a href="plumed_mtd.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-failed-red.svg" alt="tested onmaster" /></a></div>
</div>
</div>
<pre class="plumedlisting">
<span class="plumedtooltip" style="color:green">UNITS<span class="right">This command sets the internal units for the code. <a href="https://www.plumed.org/doc-master/user-doc/html/UNITS" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">LENGTH<span class="right">the units of lengths<i></i></span></span>=A
<span style="display:none;" id="data/plumed_mtd.dat">The UNITS action with label <b></b> calculates something</span><b name="data/plumed_mtd.datcv1" onclick='showPath("data/plumed_mtd.dat","data/plumed_mtd.datcv1","data/plumed_mtd.datcv1","brown")'>cv1</b>: <span class="plumedtooltip" style="color:green">PYTHONCV<span class="right">This action is not part of PLUMED and was included by using a LOAD command <a href="https://www.plumed.org/doc-master/user-doc/html/LOAD" style="color:green">More details</a><i></i></span></span> ATOMS=1-500 IMPORT=Model_pe_3 FUNCTION=cv1 COMPONENTS=BCC,FCC


<b name="data/plumed_mtd.datres" onclick='showPath("data/plumed_mtd.dat","data/plumed_mtd.datres","data/plumed_mtd.datres","brown")'>res</b>: <span class="plumedtooltip" style="color:green">METAD<span class="right">Used to performed metadynamics on one or more collective variables. <a href="https://www.plumed.org/doc-master/user-doc/html/METAD" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the labels of the scalars on which the bias will act<i></i></span></span>=cv1.py-FCC,cv1.py-BCC <span class="plumedtooltip">SIGMA<span class="right">the widths of the Gaussian hills<i></i></span></span>=0.014,0.010 <span class="plumedtooltip">HEIGHT<span class="right">the heights of the Gaussian hills<i></i></span></span>=0.5 <span class="plumedtooltip">BIASFACTOR<span class="right">use well tempered metadynamics and use this bias factor<i></i></span></span>=75 <span class="plumedtooltip">TEMP<span class="right">the system temperature - this is only needed if you are doing well-tempered metadynamics<i></i></span></span>=1100 <span class="plumedtooltip">PACE<span class="right">the frequency for hill addition<i></i></span></span>=1000 <span class="plumedtooltip">GRID_MIN<span class="right">the lower bounds for the grid<i></i></span></span>=-0.5,-0.5 <span class="plumedtooltip">GRID_MAX<span class="right">the upper bounds for the grid<i></i></span></span>=1.5,1.5 <span class="plumedtooltip">GRID_BIN<span class="right">the number of bins for the grid<i></i></span></span>=200,200

<span style="display:none;" id="data/plumed_mtd.datres">The METAD action with label <b>res</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">res.bias</td><td>the instantaneous value of the bias potential</td></tr></table></span><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/PRINT" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=colvar.out <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=* <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=250
</pre></div>

{% endraw %}
