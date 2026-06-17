**Project ID:** [plumID:21.046]({{ '/' | absolute_url }}eggs/21/046/)  
**Source:** WT-metaD.a03ws/plumed2.dat  
**Originally used with PLUMED version:** 2.3  
**Stable:** [zipped raw stdout](plumed2.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed2.dat.plumed.stderr.txt.zip) - [stderr](plumed2.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed2.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed2.dat.plumed_master.stderr.txt.zip) - [stderr](plumed2.dat.plumed_master.stderr)  

{% raw %}
<div class="plumedInputContainer">
<div class="plumedpreheader">
<div class="headerInfo" id="value_details_data/WT-metaD.a03ws/plumed2.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div class="containerBadge">
<div class="headerBadge"><a href="plumed2.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-passing-green.svg" alt="tested onv2.10" /></a></div>
<div class="headerBadge"><a href="plumed2.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></div>
</div>
</div>
<pre class="plumedlisting">
<span class="plumedtooltip" style="color:green">WHOLEMOLECULES<span class="right">This action is used to rebuild molecules that can become split by the periodic boundary conditions. <a href="https://www.plumed.org/doc-master/user-doc/html/WHOLEMOLECULES" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ENTITY0<span class="right">the atoms that make up a molecule that you wish to align<i></i></span></span>=5,12,24,43,54,61,78,89,100,119,131,142,157,183,195,205,219,230,241,248,258,277,284,295,307,326,333,345,355,372,383,398,413,425,442,461,478,488,498,514,528,545,556,575,590,604,620,644,658,670,689,711,725,740,747,769

<span style="display:none;" id="data/WT-metaD.a03ws/plumed2.dat">The WHOLEMOLECULES action with label <b></b> calculates something</span><b name="data/WT-metaD.a03ws/plumed2.datall" onclick='showPath("data/WT-metaD.a03ws/plumed2.dat","data/WT-metaD.a03ws/plumed2.datall","data/WT-metaD.a03ws/plumed2.datall","brown")'>all</b>:  <span class="plumedtooltip" style="color:green">GROUP<span class="right">Define a group of atoms so that a particular list of atoms can be referenced with a single label in definitions of CVs or virtual atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/GROUP" style="color:green">More details</a><i></i></span></span>     <span class="plumedtooltip">ATOMS<span class="right">the numerical indexes for the set of atoms in the group<i></i></span></span>=5,12,24,43,54,61,78,89,100,119,131,142,157,183,195,205,219,230,241,248,258,277,284,295,307,326,333,345,355,372,383,398,413,425,442,461,478,488,498,514,528,545,556,575,590,604,620,644,658,670,689,711,725,740,747,769

<span style="display:none;" id="data/WT-metaD.a03ws/plumed2.datall">The GROUP action with label <b>all</b> calculates something</span><b name="data/WT-metaD.a03ws/plumed2.datrg" onclick='showPath("data/WT-metaD.a03ws/plumed2.dat","data/WT-metaD.a03ws/plumed2.datrg","data/WT-metaD.a03ws/plumed2.datrg","brown")'>rg</b>:   <span class="plumedtooltip" style="color:green">GYRATION<span class="right">Calculate the radius of gyration, or other properties related to it. <a href="https://www.plumed.org/doc-master/user-doc/html/GYRATION" style="color:green">More details</a><i></i></span></span>  <span class="plumedtooltip">ATOMS<span class="right">the group of atoms that you are calculating the Gyration Tensor for<i></i></span></span>=<b name="data/WT-metaD.a03ws/plumed2.datall">all</b>
<span style="display:none;" id="data/WT-metaD.a03ws/plumed2.datrg">The GYRATION action with label <b>rg</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">rg.value</td><td>the radius that was computed from the weights</td></tr></table></span><span class="plumedtooltip" style="color:green">UPPER_WALLS<span class="right">Defines a wall for the value of one or more collective variables, <a href="https://www.plumed.org/doc-master/user-doc/html/UPPER_WALLS" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the arguments on which the bias is acting<i></i></span></span>=<b name="data/WT-metaD.a03ws/plumed2.datrg">rg</b> <span class="plumedtooltip">AT<span class="right">the positions of the wall<i></i></span></span>=3.5 <span class="plumedtooltip">KAPPA<span class="right">the force constant for the wall<i></i></span></span>=1000.0 <span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/WT-metaD.a03ws/plumed2.datuwall" onclick='showPath("data/WT-metaD.a03ws/plumed2.dat","data/WT-metaD.a03ws/plumed2.datuwall","data/WT-metaD.a03ws/plumed2.datuwall","brown")'>uwall</b>
<span style="display:none;" id="data/WT-metaD.a03ws/plumed2.datuwall">The UPPER_WALLS action with label <b>uwall</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">uwall.bias</td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">uwall.force2</td><td>the instantaneous value of the squared force due to this bias potential</td></tr></table></span><span class="plumedtooltip" style="color:green">LOWER_WALLS<span class="right">Defines a wall for the value of one or more collective variables, <a href="https://www.plumed.org/doc-master/user-doc/html/LOWER_WALLS" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the arguments on which the bias is acting<i></i></span></span>=<b name="data/WT-metaD.a03ws/plumed2.datrg">rg</b> <span class="plumedtooltip">AT<span class="right">the positions of the wall<i></i></span></span>=0.8 <span class="plumedtooltip">KAPPA<span class="right">the force constant for the wall<i></i></span></span>=1000.0 <span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/WT-metaD.a03ws/plumed2.datlwall" onclick='showPath("data/WT-metaD.a03ws/plumed2.dat","data/WT-metaD.a03ws/plumed2.datlwall","data/WT-metaD.a03ws/plumed2.datlwall","brown")'>lwall</b>
<br/><span style="display:none;" id="data/WT-metaD.a03ws/plumed2.datlwall">The LOWER_WALLS action with label <b>lwall</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">lwall.bias</td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">lwall.force2</td><td>the instantaneous value of the squared force due to this bias potential</td></tr></table></span><span class="plumedtooltip" style="color:green">ALPHABETA<span class="right">Measures a distance including pbc between the instantaneous values of a set of torsional angles and set of reference values. <a href="https://www.plumed.org/doc-master/user-doc/html/ALPHABETA" style="color:green">More details</a><i></i></span></span> ...
<span class="plumedtooltip">ATOMS1<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=1,5,8,10    <span class="plumedtooltip">REFERENCE<span class="right">the reference values for each of the torsional angles<i></i></span></span>=-0.78540
<span class="plumedtooltip">ATOMS2<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=10,12,20,22
<span class="plumedtooltip">ATOMS3<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=22,24,39,41
<span class="plumedtooltip">ATOMS4<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=41,43,50,52
<span class="plumedtooltip">ATOMS5<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=52,54,57,59
<span class="plumedtooltip">ATOMS6<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=59,61,74,76
<span class="plumedtooltip">ATOMS7<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=76,78,85,87
<span class="plumedtooltip">ATOMS8<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=87,89,96,98
<span class="plumedtooltip">ATOMS9<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=98,100,113,115
<span class="plumedtooltip">ATOMS10<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=115,119,127,129
<span class="plumedtooltip">ATOMS11<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=129,131,138,140
<span class="plumedtooltip">ATOMS12<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=140,142,153,155
<span class="plumedtooltip">ATOMS13<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=155,157,177,179
<span class="plumedtooltip">ATOMS14<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=179,183,191,193
<span class="plumedtooltip">ATOMS15<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=193,195,201,203
<span class="plumedtooltip">ATOMS16<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=203,205,215,217
<span class="plumedtooltip">ATOMS17<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=217,219,226,228
<span class="plumedtooltip">ATOMS18<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=228,230,237,239
<span class="plumedtooltip">ATOMS19<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=239,241,244,246
<span class="plumedtooltip">ATOMS20<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=246,248,254,256
<span class="plumedtooltip">ATOMS21<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=256,258,273,275
<span class="plumedtooltip">ATOMS22<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=275,277,280,282
<span class="plumedtooltip">ATOMS23<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=282,284,291,293
<span class="plumedtooltip">ATOMS24<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=293,295,303,305
<span class="plumedtooltip">ATOMS25<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=305,307,322,324
<span class="plumedtooltip">ATOMS26<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=324,326,329,331
<span class="plumedtooltip">ATOMS27<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=331,333,341,343
<span class="plumedtooltip">ATOMS28<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=343,345,351,353
<span class="plumedtooltip">ATOMS29<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=353,355,368,370
<span class="plumedtooltip">ATOMS30<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=370,372,379,381
<span class="plumedtooltip">ATOMS31<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=381,383,394,396
<span class="plumedtooltip">ATOMS32<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=396,398,409,411
<span class="plumedtooltip">ATOMS33<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=411,413,421,423
<span class="plumedtooltip">ATOMS34<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=423,425,438,440
<span class="plumedtooltip">ATOMS35<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=440,442,457,459
<span class="plumedtooltip">ATOMS36<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=459,461,474,476
<span class="plumedtooltip">ATOMS37<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=476,478,484,486
<span class="plumedtooltip">ATOMS38<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=486,488,494,496
<span class="plumedtooltip">ATOMS39<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=496,498,510,512
<span class="plumedtooltip">ATOMS40<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=512,514,524,526
<span class="plumedtooltip">ATOMS41<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=526,528,541,543
<span class="plumedtooltip">ATOMS42<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=543,545,552,554
<span class="plumedtooltip">ATOMS43<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=554,556,571,573
<span class="plumedtooltip">ATOMS44<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=573,575,586,588
<span class="plumedtooltip">ATOMS45<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=588,590,600,602
<span class="plumedtooltip">ATOMS46<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=602,604,616,618
<span class="plumedtooltip">ATOMS47<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=618,620,640,642
<span class="plumedtooltip">ATOMS48<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=642,644,654,656
<span class="plumedtooltip">ATOMS49<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=656,658,666,668
<span class="plumedtooltip">ATOMS50<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=668,670,685,687
<span class="plumedtooltip">ATOMS51<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=687,689,707,709
<span class="plumedtooltip">ATOMS52<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=709,711,721,723
<span class="plumedtooltip">ATOMS53<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=723,725,736,738
<span class="plumedtooltip">ATOMS54<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=738,740,743,745
<span class="plumedtooltip">ATOMS55<span class="right">the atoms involved for each of the torsions you wish to calculate<i></i></span></span>=745,747,765,767
 <span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/WT-metaD.a03ws/plumed2.datab" onclick='showPath("data/WT-metaD.a03ws/plumed2.dat","data/WT-metaD.a03ws/plumed2.datab","data/WT-metaD.a03ws/plumed2.datab","brown")'>ab</b>
... ALPHABETA
<br/><span style="display:none;" id="data/WT-metaD.a03ws/plumed2.datab">The ALPHABETA action with label <b>ab</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ab.value</td><td>the alpha beta CV</td></tr></table></span><span class="plumedtooltip" style="color:green">METAD<span class="right">Used to performed metadynamics on one or more collective variables. <a href="https://www.plumed.org/doc-master/user-doc/html/METAD" style="color:green">More details</a><i></i></span></span> ...
  <span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/WT-metaD.a03ws/plumed2.datmeta" onclick='showPath("data/WT-metaD.a03ws/plumed2.dat","data/WT-metaD.a03ws/plumed2.datmeta","data/WT-metaD.a03ws/plumed2.datmeta","brown")'>meta</b>
  <span class="plumedtooltip">ARG<span class="right">the labels of the scalars on which the bias will act<i></i></span></span>=<b name="data/WT-metaD.a03ws/plumed2.datrg">rg</b>,<b name="data/WT-metaD.a03ws/plumed2.datab">ab</b> <span class="plumedtooltip">SIGMA<span class="right">the widths of the Gaussian hills<i></i></span></span>=0.2,1.0 <span class="plumedtooltip">HEIGHT<span class="right">the heights of the Gaussian hills<i></i></span></span>=0.5 <span class="plumedtooltip">PACE<span class="right">the frequency for hill addition<i></i></span></span>=1000
  <span class="plumedtooltip">BIASFACTOR<span class="right">use well tempered metadynamics and use this bias factor<i></i></span></span>=4 <span class="plumedtooltip">TEMP<span class="right">the system temperature - this is only needed if you are doing well-tempered metadynamics<i></i></span></span>=298
... METAD
<br/><span style="display:none;" id="data/WT-metaD.a03ws/plumed2.datmeta">The METAD action with label <b>meta</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">meta.bias</td><td>the instantaneous value of the bias potential</td></tr></table></span><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/PRINT" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=<b name="data/WT-metaD.a03ws/plumed2.datrg">rg</b>,<b name="data/WT-metaD.a03ws/plumed2.datab">ab</b>,<b name="data/WT-metaD.a03ws/plumed2.datmeta">meta.bias</b> <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=1000 <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=COLVAR

<span class="plumedtooltip" style="color:green">ENDPLUMED<span class="right">Terminate plumed input. <a href="https://www.plumed.org/doc-master/user-doc/html/ENDPLUMED" style="color:green">More details</a><i></i></span></span><span style="color:blue" class="comment">

# original input file with plumed 1 syntax follows

HILLS HEIGHT 0.5  W_STRIDE 1000 RESTART 

WELLTEMPERED SIMTEMP 298  BIASFACTOR 4 

#PTMETAD

PRINT W_STRIDE 1000

ALIGN_ATOMS LIST &lt;all&gt;


#CV1 Rg CA

RGYR LIST &lt;all&gt; SIGMA 0.2

#CV4
ALPHABETA NDIH 55 SIGMA 1.0
1    5    8    10    -0.78540
10    12    20    22    -0.78540
22    24    39    41    -0.78540
41    43    50    52    -0.78540
52    54    57    59    -0.78540
59    61    74    76    -0.78540
76    78    85    87    -0.78540
87    89    96    98    -0.78540
98    100    113    115    -0.78540
115    125    127    129    -0.78540
129    131    138    140    -0.78540
140    142    153    155    -0.78540
155    157    177    179    -0.78540
179    189    191    193    -0.78540
193    195    201    203    -0.78540
203    205    215    217    -0.78540
217    219    226    228    -0.78540
228    230    237    239    -0.78540
239    241    244    246    -0.78540
246    248    254    256    -0.78540
256    258    273    275    -0.78540
275    277    280    282    -0.78540
282    284    291    293    -0.78540
293    295    303    305    -0.78540
305    307    322    324    -0.78540
324    326    329    331    -0.78540
331    333    341    343    -0.78540
343    345    351    353    -0.78540
353    355    368    370    -0.78540
370    372    379    381    -0.78540
381    383    394    396    -0.78540
396    398    409    411    -0.78540
411    413    421    423    -0.78540
423    425    438    440    -0.78540
440    442    457    459    -0.78540
459    461    474    476    -0.78540
476    478    484    486    -0.78540
486    488    494    496    -0.78540
496    498    510    512    -0.78540
512    514    524    526    -0.78540
526    528    541    543    -0.78540
543    545    552    554    -0.78540
554    556    571    573    -0.78540
573    575    586    588    -0.78540
588    590    600    602    -0.78540
602    604    616    618    -0.78540
618    620    640    642    -0.78540
642    644    654    656    -0.78540
656    658    666    668    -0.78540
668    670    685    687    -0.78540
687    689    707    709    -0.78540
709    711    721    723    -0.78540
723    725    736    738    -0.78540
738    740    743    745    -0.78540
745    747    765    767    -0.78540

#UWALL CV 1 LIMIT 2.2 KAPPA 1000.0
#UWALL CV 2 LIMIT 0.6 KAPPA 1000.0
LWALL CV 1 LIMIT 0.8 KAPPA 1000.0
UWALL CV 1 LIMIT 3.5 KAPPA 1000.0 

all-&gt;
5
12
24
43
54
61
78
89
100
125
131
142
157
189
195
205
219
230
241
248
258
277
284
295
307
326
333
345
355
372
383
398
413
425
442
461
478
488
498
514
528
545
556
575
590
604
620
644
658
670
689
711
725
740
747
769
all&lt;-


ENDMETA
</span></pre></div>

{% endraw %}
