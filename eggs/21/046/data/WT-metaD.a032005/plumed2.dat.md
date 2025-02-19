**Project ID:** [plumID:21.046]({{ '/' | absolute_url }}eggs/21/046/)  
**Source:** WT-metaD.a032005/plumed2.dat  
**Originally used with PLUMED version:** 2.3  
**Stable:** [zipped raw stdout](plumed2.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed2.dat.plumed.stderr.txt.zip) - [stderr](plumed2.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed2.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed2.dat.plumed_master.stderr.txt.zip) - [stderr](plumed2.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/WT-metaD.a032005/plumed2.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed2.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.10-passing-green.svg" alt="tested onv2.10" /></a></td></tr><tr><td style="padding:1px"><a href="plumed2.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span class="plumedtooltip" style="color:green">WHOLEMOLECULES<span class="right">This action is used to rebuild molecules that can become split by the periodic boundary conditions. <a href="https://www.plumed.org/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ENTITY0<span class="right">the atoms that make up a molecule that you wish to align<i></i></span></span>=5,12,24,43,54,61,78,89,100,119,131,142,157,183,195,205,219,230,241,248,258,277,284,295,307,326,333,345,355,372,383,398,413,425,442,461,478,488,498,514,528,545,556,575,590,604,620,644,658,670,689,711,725,740,747,769

<span style="display:none;" id="data/WT-metaD.a032005/plumed2.dat">The WHOLEMOLECULES action with label <b></b> calculates something</span><b name="data/WT-metaD.a032005/plumed2.datall" onclick='showPath("data/WT-metaD.a032005/plumed2.dat","data/WT-metaD.a032005/plumed2.datall","data/WT-metaD.a032005/plumed2.datall","violet")'>all</b><span style="display:none;" id="data/WT-metaD.a032005/plumed2.datall">The GROUP action with label <b>all</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">all</td><td width="5%"><font color="violet">atoms</font></td><td>indices of atoms specified in GROUP</td></tr></table></span>:  <span class="plumedtooltip" style="color:green">GROUP<span class="right">Define a group of atoms so that a particular list of atoms can be referenced with a single label in definitions of CVs or virtual atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_g_r_o_u_p.html" style="color:green">More details</a><i></i></span></span>     <span class="plumedtooltip">ATOMS<span class="right">the numerical indexes for the set of atoms in the group<i></i></span></span>=5,12,24,43,54,61,78,89,100,119,131,142,157,183,195,205,219,230,241,248,258,277,284,295,307,326,333,345,355,372,383,398,413,425,442,461,478,488,498,514,528,545,556,575,590,604,620,644,658,670,689,711,725,740,747,769

<b name="data/WT-metaD.a032005/plumed2.datrg" onclick='showPath("data/WT-metaD.a032005/plumed2.dat","data/WT-metaD.a032005/plumed2.datrg","data/WT-metaD.a032005/plumed2.datrg","black")'>rg</b><span style="display:none;" id="data/WT-metaD.a032005/plumed2.datrg">The GYRATION action with label <b>rg</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">rg</td><td width="5%"><font color="black">scalar</font></td><td>the radius of gyration</td></tr></table></span>:   <span class="plumedtooltip" style="color:green">GYRATION<span class="right">Calculate the radius of gyration, or other properties related to it. <a href="https://www.plumed.org/doc-master/user-doc/html/_g_y_r_a_t_i_o_n.html" style="color:green">More details</a><i></i></span></span>  <span class="plumedtooltip">ATOMS<span class="right">the group of atoms that you are calculating the Gyration Tensor for<i></i></span></span>=<b name="data/WT-metaD.a032005/plumed2.datall">all</b>
<span class="plumedtooltip" style="color:green">UPPER_WALLS<span class="right">Defines a wall for the value of one or more collective variables, <a href="https://www.plumed.org/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the arguments on which the bias is acting<i></i></span></span>=<b name="data/WT-metaD.a032005/plumed2.datrg">rg</b> <span class="plumedtooltip">AT<span class="right">the positions of the wall<i></i></span></span>=3.5 <span class="plumedtooltip">KAPPA<span class="right">the force constant for the wall<i></i></span></span>=1000.0 <span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/WT-metaD.a032005/plumed2.datuwall" onclick='showPath("data/WT-metaD.a032005/plumed2.dat","data/WT-metaD.a032005/plumed2.datuwall","data/WT-metaD.a032005/plumed2.datuwall","black")'>uwall</b><span style="display:none;" id="data/WT-metaD.a032005/plumed2.datuwall">The UPPER_WALLS action with label <b>uwall</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">uwall.bias</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">uwall.force2</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the squared force due to this bias potential</td></tr></table></span>
<span class="plumedtooltip" style="color:green">LOWER_WALLS<span class="right">Defines a wall for the value of one or more collective variables, <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the arguments on which the bias is acting<i></i></span></span>=<b name="data/WT-metaD.a032005/plumed2.datrg">rg</b> <span class="plumedtooltip">AT<span class="right">the positions of the wall<i></i></span></span>=0.8 <span class="plumedtooltip">KAPPA<span class="right">the force constant for the wall<i></i></span></span>=1000.0 <span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/WT-metaD.a032005/plumed2.datlwall" onclick='showPath("data/WT-metaD.a032005/plumed2.dat","data/WT-metaD.a032005/plumed2.datlwall","data/WT-metaD.a032005/plumed2.datlwall","black")'>lwall</b><span style="display:none;" id="data/WT-metaD.a032005/plumed2.datlwall">The LOWER_WALLS action with label <b>lwall</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">lwall.bias</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">lwall.force2</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the squared force due to this bias potential</td></tr></table></span>
<br/><span id="data/WT-metaD.a032005/plumed2.datab_short"><span class="plumedtooltip" style="color:green">ALPHABETA<span class="right">Calculate the alpha beta CV This action is <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/WT-metaD.a032005/plumed2.datab");'>a shortcut</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_a_l_p_h_a_b_e_t_a.html">More details</a><i></i></span></span> ...
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
 <span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/WT-metaD.a032005/plumed2.datab" onclick='showPath("data/WT-metaD.a032005/plumed2.dat","data/WT-metaD.a032005/plumed2.datab","data/WT-metaD.a032005/plumed2.datab_shortcut","black")'>ab</b><span style="display:none;" id="data/WT-metaD.a032005/plumed2.datab_shortcut">The ALPHABETA action with label <b>ab</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ab</td><td width="5%"><font color="black">scalar</font></td><td>the alpha beta CV</td></tr></table></span>
... ALPHABETA
</span><span id="data/WT-metaD.a032005/plumed2.datab_long" style="display:none;"><span style="color:blue" class="comment"># PLUMED interprets the command:
</span><span class="toggler" style="color:red" onclick='toggleDisplay("data/WT-metaD.a032005/plumed2.datab")'># ALPHABETA ...</span>
<span style="color:blue" class="comment"># ATOMS1=1,5,8,10    REFERENCE=-0.78540</span>
<span style="color:blue" class="comment"># ATOMS2=10,12,20,22</span>
<span style="color:blue" class="comment"># ATOMS3=22,24,39,41</span>
<span style="color:blue" class="comment"># ATOMS4=41,43,50,52</span>
<span style="color:blue" class="comment"># ATOMS5=52,54,57,59</span>
<span style="color:blue" class="comment"># ATOMS6=59,61,74,76</span>
<span style="color:blue" class="comment"># ATOMS7=76,78,85,87</span>
<span style="color:blue" class="comment"># ATOMS8=87,89,96,98</span>
<span style="color:blue" class="comment"># ATOMS9=98,100,113,115</span>
<span style="color:blue" class="comment"># ATOMS10=115,119,127,129</span>
<span style="color:blue" class="comment"># ATOMS11=129,131,138,140</span>
<span style="color:blue" class="comment"># ATOMS12=140,142,153,155</span>
<span style="color:blue" class="comment"># ATOMS13=155,157,177,179</span>
<span style="color:blue" class="comment"># ATOMS14=179,183,191,193</span>
<span style="color:blue" class="comment"># ATOMS15=193,195,201,203</span>
<span style="color:blue" class="comment"># ATOMS16=203,205,215,217</span>
<span style="color:blue" class="comment"># ATOMS17=217,219,226,228</span>
<span style="color:blue" class="comment"># ATOMS18=228,230,237,239</span>
<span style="color:blue" class="comment"># ATOMS19=239,241,244,246</span>
<span style="color:blue" class="comment"># ATOMS20=246,248,254,256</span>
<span style="color:blue" class="comment"># ATOMS21=256,258,273,275</span>
<span style="color:blue" class="comment"># ATOMS22=275,277,280,282</span>
<span style="color:blue" class="comment"># ATOMS23=282,284,291,293</span>
<span style="color:blue" class="comment"># ATOMS24=293,295,303,305</span>
<span style="color:blue" class="comment"># ATOMS25=305,307,322,324</span>
<span style="color:blue" class="comment"># ATOMS26=324,326,329,331</span>
<span style="color:blue" class="comment"># ATOMS27=331,333,341,343</span>
<span style="color:blue" class="comment"># ATOMS28=343,345,351,353</span>
<span style="color:blue" class="comment"># ATOMS29=353,355,368,370</span>
<span style="color:blue" class="comment"># ATOMS30=370,372,379,381</span>
<span style="color:blue" class="comment"># ATOMS31=381,383,394,396</span>
<span style="color:blue" class="comment"># ATOMS32=396,398,409,411</span>
<span style="color:blue" class="comment"># ATOMS33=411,413,421,423</span>
<span style="color:blue" class="comment"># ATOMS34=423,425,438,440</span>
<span style="color:blue" class="comment"># ATOMS35=440,442,457,459</span>
<span style="color:blue" class="comment"># ATOMS36=459,461,474,476</span>
<span style="color:blue" class="comment"># ATOMS37=476,478,484,486</span>
<span style="color:blue" class="comment"># ATOMS38=486,488,494,496</span>
<span style="color:blue" class="comment"># ATOMS39=496,498,510,512</span>
<span style="color:blue" class="comment"># ATOMS40=512,514,524,526</span>
<span style="color:blue" class="comment"># ATOMS41=526,528,541,543</span>
<span style="color:blue" class="comment"># ATOMS42=543,545,552,554</span>
<span style="color:blue" class="comment"># ATOMS43=554,556,571,573</span>
<span style="color:blue" class="comment"># ATOMS44=573,575,586,588</span>
<span style="color:blue" class="comment"># ATOMS45=588,590,600,602</span>
<span style="color:blue" class="comment"># ATOMS46=602,604,616,618</span>
<span style="color:blue" class="comment"># ATOMS47=618,620,640,642</span>
<span style="color:blue" class="comment"># ATOMS48=642,644,654,656</span>
<span style="color:blue" class="comment"># ATOMS49=656,658,666,668</span>
<span style="color:blue" class="comment"># ATOMS50=668,670,685,687</span>
<span style="color:blue" class="comment"># ATOMS51=687,689,707,709</span>
<span style="color:blue" class="comment"># ATOMS52=709,711,721,723</span>
<span style="color:blue" class="comment"># ATOMS53=723,725,736,738</span>
<span style="color:blue" class="comment"># ATOMS54=738,740,743,745</span>
<span style="color:blue" class="comment"># ATOMS55=745,747,765,767</span>
<span style="color:blue" class="comment">#  LABEL=ab</span>
<span style="color:blue" class="comment"># ... ALPHABETA</span>
<span style="color:blue" class="comment"># as follows (Click the red comment above to revert to the short version of the input):</span>
<b name="data/WT-metaD.a032005/plumed2.datab_torsions" onclick='showPath("data/WT-metaD.a032005/plumed2.dat","data/WT-metaD.a032005/plumed2.datab_torsions","data/WT-metaD.a032005/plumed2.datab_torsions","blue")'>ab_torsions</b><span style="display:none;" id="data/WT-metaD.a032005/plumed2.datab_torsions">The TORSION action with label <b>ab_torsions</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ab_torsions</td><td width="5%"><font color="blue">vector</font></td><td>the TORSION for each set of specified atoms</td></tr></table></span>: <span class="plumedtooltip" style="color:green">TORSION<span class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ATOMS1<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=1,5,8,10 <span class="plumedtooltip">ATOMS2<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=10,12,20,22 <span class="plumedtooltip">ATOMS3<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=22,24,39,41 <span class="plumedtooltip">ATOMS4<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=41,43,50,52 <span class="plumedtooltip">ATOMS5<span class="right">the four atoms involved in the torsional angle<i></i></span></span>=52,54,57,59     <span style="color:blue" class="comment"># Action input conctinues with 50 further ATOMSn keywords, </span>
<b name="data/WT-metaD.a032005/plumed2.datab_ref" onclick='showPath("data/WT-metaD.a032005/plumed2.dat","data/WT-metaD.a032005/plumed2.datab_ref","data/WT-metaD.a032005/plumed2.datab_ref","blue")'>ab_ref</b><span style="display:none;" id="data/WT-metaD.a032005/plumed2.datab_ref">The CONSTANT action with label <b>ab_ref</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ab_ref</td><td width="5%"><font color="blue">vector</font></td><td>the constant value that was read from the plumed input</td></tr></table></span>: <span class="plumedtooltip" style="color:green">CONSTANT<span class="right">Create a constant value that can be passed to actions <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">VALUES<span class="right">the numbers that are in your constant value<i></i></span></span>=-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540
<b name="data/WT-metaD.a032005/plumed2.datab_coeff" onclick='showPath("data/WT-metaD.a032005/plumed2.dat","data/WT-metaD.a032005/plumed2.datab_coeff","data/WT-metaD.a032005/plumed2.datab_coeff","blue")'>ab_coeff</b><span style="display:none;" id="data/WT-metaD.a032005/plumed2.datab_coeff">The CONSTANT action with label <b>ab_coeff</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ab_coeff</td><td width="5%"><font color="blue">vector</font></td><td>the constant value that was read from the plumed input</td></tr></table></span>: <span class="plumedtooltip" style="color:green">CONSTANT<span class="right">Create a constant value that can be passed to actions <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">VALUES<span class="right">the numbers that are in your constant value<i></i></span></span>=1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1
<b name="data/WT-metaD.a032005/plumed2.datab_comb" onclick='showPath("data/WT-metaD.a032005/plumed2.dat","data/WT-metaD.a032005/plumed2.datab_comb","data/WT-metaD.a032005/plumed2.datab_comb","blue")'>ab_comb</b><span style="display:none;" id="data/WT-metaD.a032005/plumed2.datab_comb">The COMBINE action with label <b>ab_comb</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ab_comb</td><td width="5%"><font color="blue">vector</font></td><td>the vector obtained by doing an element-wise application of a linear compbination to the input vectors</td></tr></table></span>: <span class="plumedtooltip" style="color:green">COMBINE<span class="right">Calculate a polynomial combination of a set of other variables. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_m_b_i_n_e.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the values input to this function<i></i></span></span>=<b name="data/WT-metaD.a032005/plumed2.datab_torsions">ab_torsions</b>,<b name="data/WT-metaD.a032005/plumed2.datab_ref">ab_ref</b> <span class="plumedtooltip">COEFFICIENTS<span class="right"> the coefficients of the arguments in your function<i></i></span></span>=1,-1 <span class="plumedtooltip">PERIODIC<span class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></span></span>=NO
<b name="data/WT-metaD.a032005/plumed2.datab_cos" onclick='showPath("data/WT-metaD.a032005/plumed2.dat","data/WT-metaD.a032005/plumed2.datab_cos","data/WT-metaD.a032005/plumed2.datab_cos","blue")'>ab_cos</b><span style="display:none;" id="data/WT-metaD.a032005/plumed2.datab_cos">The CUSTOM action with label <b>ab_cos</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ab_cos</td><td width="5%"><font color="blue">vector</font></td><td>the vector obtained by doing an element-wise application of an arbitrary function to the input vectors</td></tr></table></span>: <span class="plumedtooltip" style="color:green">CUSTOM<span class="right">Calculate a combination of variables using a custom expression. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_u_s_t_o_m.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the values input to this function<i></i></span></span>=<b name="data/WT-metaD.a032005/plumed2.datab_comb">ab_comb</b>,<b name="data/WT-metaD.a032005/plumed2.datab_coeff">ab_coeff</b> <span class="plumedtooltip">FUNC<span class="right">the function you wish to evaluate<i></i></span></span>=y*(0.5+0.5*cos(x)) <span class="plumedtooltip">PERIODIC<span class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></span></span>=NO
<b name="data/WT-metaD.a032005/plumed2.datab" onclick='showPath("data/WT-metaD.a032005/plumed2.dat","data/WT-metaD.a032005/plumed2.datab","data/WT-metaD.a032005/plumed2.datab","black")'>ab</b><span style="display:none;" id="data/WT-metaD.a032005/plumed2.datab">The SUM action with label <b>ab</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ab</td><td width="5%"><font color="black">scalar</font></td><td>the sum of all the elements in the input vector</td></tr></table></span>: <span class="plumedtooltip" style="color:green">SUM<span class="right">Calculate the sum of the arguments <a href="https://www.plumed.org/doc-master/user-doc/html/_s_u_m.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the values input to this function<i></i></span></span>=<b name="data/WT-metaD.a032005/plumed2.datab_cos">ab_cos</b> <span class="plumedtooltip">PERIODIC<span class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></span></span>=NO
<span style="color:blue"># --- End of included input --- </span></span><br/><span id="data/WT-metaD.a032005/plumed2.datdefmeta_short"><span class="plumedtooltip" style="color:green">METAD<span class="right">Used to performed metadynamics on one or more collective variables. This action has <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/WT-metaD.a032005/plumed2.datdefmeta");'>hidden defaults</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_e_t_a_d.html">More details</a><i></i></span></span> ...
  <span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/WT-metaD.a032005/plumed2.datmeta" onclick='showPath("data/WT-metaD.a032005/plumed2.dat","data/WT-metaD.a032005/plumed2.datmeta","data/WT-metaD.a032005/plumed2.datmeta","black")'>meta</b><span style="display:none;" id="data/WT-metaD.a032005/plumed2.datmeta">The METAD action with label <b>meta</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">meta.bias</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the bias potential</td></tr></table></span>
  <span class="plumedtooltip">ARG<span class="right">the labels of the scalars on which the bias will act<i></i></span></span>=<b name="data/WT-metaD.a032005/plumed2.datrg">rg</b>,<b name="data/WT-metaD.a032005/plumed2.datab">ab</b> <span class="plumedtooltip">SIGMA<span class="right">the widths of the Gaussian hills<i></i></span></span>=0.2,1.0 <span class="plumedtooltip">HEIGHT<span class="right">the heights of the Gaussian hills<i></i></span></span>=0.5 <span class="plumedtooltip">PACE<span class="right">the frequency for hill addition<i></i></span></span>=1000
  <span class="plumedtooltip">BIASFACTOR<span class="right">use well tempered metadynamics and use this bias factor<i></i></span></span>=4 <span class="plumedtooltip">TEMP<span class="right">the system temperature - this is only needed if you are doing well-tempered metadynamics<i></i></span></span>=298
... METAD
</span><span id="data/WT-metaD.a032005/plumed2.datdefmeta_long" style="display:none;"><span class="plumedtooltip" style="color:green">METAD<span class="right">Used to performed metadynamics on one or more collective variables. This action uses the <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/WT-metaD.a032005/plumed2.datdefmeta");'>defaults shown here</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_e_t_a_d.html">More details</a><i></i></span></span> ...
  <span class="plumedtooltip">LABEL<span class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></span></span>=<b name="data/WT-metaD.a032005/plumed2.datmeta" onclick='showPath("data/WT-metaD.a032005/plumed2.dat","data/WT-metaD.a032005/plumed2.datmeta","data/WT-metaD.a032005/plumed2.datmeta","black")'>meta</b>
  <span class="plumedtooltip">ARG<span class="right">the labels of the scalars on which the bias will act<i></i></span></span>=<b name="data/WT-metaD.a032005/plumed2.datrg">rg</b>,<b name="data/WT-metaD.a032005/plumed2.datab">ab</b> <span class="plumedtooltip">SIGMA<span class="right">the widths of the Gaussian hills<i></i></span></span>=0.2,1.0 <span class="plumedtooltip">HEIGHT<span class="right">the heights of the Gaussian hills<i></i></span></span>=0.5 <span class="plumedtooltip">PACE<span class="right">the frequency for hill addition<i></i></span></span>=1000
  <span class="plumedtooltip">BIASFACTOR<span class="right">use well tempered metadynamics and use this bias factor<i></i></span></span>=4 <span class="plumedtooltip">TEMP<span class="right">the system temperature - this is only needed if you are doing well-tempered metadynamics<i></i></span></span>=298
 <span class="plumedtooltip">FILE<span class="right"> a file in which the list of added hills is stored<i></i></span></span>=HILLS
... METAD
</span><br/><span class="plumedtooltip" style="color:green">PRINT<span class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></span></span> <span class="plumedtooltip">ARG<span class="right">the labels of the values that you would like to print to the file<i></i></span></span>=<b name="data/WT-metaD.a032005/plumed2.datrg">rg</b>,<b name="data/WT-metaD.a032005/plumed2.datab">ab</b>,<b name="data/WT-metaD.a032005/plumed2.datmeta">meta.bias</b> <span class="plumedtooltip">STRIDE<span class="right"> the frequency with which the quantities of interest should be output<i></i></span></span>=1000 <span class="plumedtooltip">FILE<span class="right">the name of the file on which to output these quantities<i></i></span></span>=COLVAR

<span class="plumedtooltip" style="color:green">ENDPLUMED<span class="right">Terminate plumed input. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html" style="color:green">More details</a><i></i></span></span><span style="color:blue" class="comment">

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
</span></pre>
{% endraw %}
