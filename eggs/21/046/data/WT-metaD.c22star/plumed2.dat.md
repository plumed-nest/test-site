**Project ID:** [plumID:21.046]({{ '/' | absolute_url }}eggs/21/046/)  
**Source:** WT-metaD.c22star/plumed2.dat  
**Originally used with PLUMED version:** 2.3  
**Stable:** [zipped raw stdout](plumed2.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed2.dat.plumed.stderr.txt.zip) - [stderr](plumed2.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed2.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed2.dat.plumed_master.stderr.txt.zip) - [stderr](plumed2.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/WT-metaD.c22star/plumed2.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed2.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed2.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<div class="tooltip" style="color:green">WHOLEMOLECULES<div class="right">This action is used to rebuild molecules that can become split by the periodic boundary conditions. <a href="https://www.plumed.org/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ENTITY0<div class="right">the atoms that make up a molecule that you wish to align<i></i></div></div>=5,12,24,43,54,61,78,89,100,119,131,142,157,183,195,205,219,230,241,248,258,277,284,295,307,326,333,345,355,372,383,398,413,425,442,461,478,488,498,514,528,545,556,575,590,604,620,644,658,670,689,711,725,740,747,769
<br/><span style="display:none;" id="data/WT-metaD.c22star/plumed2.dat">The WHOLEMOLECULES action with label <b></b> calculates something</span><b name="data/WT-metaD.c22star/plumed2.datall" onclick='showPath("data/WT-metaD.c22star/plumed2.dat","data/WT-metaD.c22star/plumed2.datall","data/WT-metaD.c22star/plumed2.datall","violet")'>all</b><span style="display:none;" id="data/WT-metaD.c22star/plumed2.datall">The GROUP action with label <b>all</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">all</td><td width="5%"><font color="violet">atoms</font></td><td>indices of atoms specified in GROUP</td></tr></table></span>:  <div class="tooltip" style="color:green">GROUP<div class="right">Define a group of atoms so that a particular list of atoms can be referenced with a single label in definitions of CVs or virtual atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_g_r_o_u_p.html" style="color:green">More details</a><i></i></div></div>     <div class="tooltip">ATOMS<div class="right">the numerical indexes for the set of atoms in the group<i></i></div></div>=5,12,24,43,54,61,78,89,100,119,131,142,157,183,195,205,219,230,241,248,258,277,284,295,307,326,333,345,355,372,383,398,413,425,442,461,478,488,498,514,528,545,556,575,590,604,620,644,658,670,689,711,725,740,747,769
<br/><b name="data/WT-metaD.c22star/plumed2.datrg" onclick='showPath("data/WT-metaD.c22star/plumed2.dat","data/WT-metaD.c22star/plumed2.datrg","data/WT-metaD.c22star/plumed2.datrg","black")'>rg</b><span style="display:none;" id="data/WT-metaD.c22star/plumed2.datrg">The GYRATION action with label <b>rg</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">rg</td><td width="5%"><font color="black">scalar</font></td><td>the radius of gyration</td></tr></table></span>:   <div class="tooltip" style="color:green">GYRATION<div class="right">Calculate the radius of gyration, or other properties related to it. <a href="https://www.plumed.org/doc-master/user-doc/html/_g_y_r_a_t_i_o_n.html" style="color:green">More details</a><i></i></div></div>  <div class="tooltip">ATOMS<div class="right">the group of atoms that you are calculating the Gyration Tensor for<i></i></div></div>=<b name="data/WT-metaD.c22star/plumed2.datall">all</b>
<div class="tooltip" style="color:green">UPPER_WALLS<div class="right">Defines a wall for the value of one or more collective variables, <a href="https://www.plumed.org/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the arguments on which the bias is acting<i></i></div></div>=<b name="data/WT-metaD.c22star/plumed2.datrg">rg</b> <div class="tooltip">AT<div class="right">the positions of the wall<i></i></div></div>=3.5 <div class="tooltip">KAPPA<div class="right">the force constant for the wall<i></i></div></div>=1000.0 <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/WT-metaD.c22star/plumed2.datuwall" onclick='showPath("data/WT-metaD.c22star/plumed2.dat","data/WT-metaD.c22star/plumed2.datuwall","data/WT-metaD.c22star/plumed2.datuwall","black")'>uwall</b><span style="display:none;" id="data/WT-metaD.c22star/plumed2.datuwall">The UPPER_WALLS action with label <b>uwall</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">uwall.bias</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">uwall.force2</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the squared force due to this bias potential</td></tr></table></span>
<div class="tooltip" style="color:green">LOWER_WALLS<div class="right">Defines a wall for the value of one or more collective variables, <a href="https://www.plumed.org/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the arguments on which the bias is acting<i></i></div></div>=<b name="data/WT-metaD.c22star/plumed2.datrg">rg</b> <div class="tooltip">AT<div class="right">the positions of the wall<i></i></div></div>=0.8 <div class="tooltip">KAPPA<div class="right">the force constant for the wall<i></i></div></div>=1000.0 <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/WT-metaD.c22star/plumed2.datlwall" onclick='showPath("data/WT-metaD.c22star/plumed2.dat","data/WT-metaD.c22star/plumed2.datlwall","data/WT-metaD.c22star/plumed2.datlwall","black")'>lwall</b><span style="display:none;" id="data/WT-metaD.c22star/plumed2.datlwall">The LOWER_WALLS action with label <b>lwall</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">lwall.bias</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">lwall.force2</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the squared force due to this bias potential</td></tr></table></span>
<br/><span id="data/WT-metaD.c22star/plumed2.datab_short"><div class="tooltip" style="color:green">ALPHABETA<div class="right">Calculate the alpha beta CV This action is <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/WT-metaD.c22star/plumed2.datab");'>a shortcut</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_a_l_p_h_a_b_e_t_a.html">More details</a><i></i></div></div> ...
<div class="tooltip">ATOMS1<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=1,5,8,10    <div class="tooltip">REFERENCE<div class="right">the reference values for each of the torsional angles<i></i></div></div>=-0.78540
<div class="tooltip">ATOMS2<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=10,12,20,22
<div class="tooltip">ATOMS3<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=22,24,39,41
<div class="tooltip">ATOMS4<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=41,43,50,52
<div class="tooltip">ATOMS5<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=52,54,57,59
<div class="tooltip">ATOMS6<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=59,61,74,76
<div class="tooltip">ATOMS7<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=76,78,85,87
<div class="tooltip">ATOMS8<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=87,89,96,98
<div class="tooltip">ATOMS9<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=98,100,113,115
<div class="tooltip">ATOMS10<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=115,119,127,129
<div class="tooltip">ATOMS11<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=129,131,138,140
<div class="tooltip">ATOMS12<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=140,142,153,155
<div class="tooltip">ATOMS13<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=155,157,177,179
<div class="tooltip">ATOMS14<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=179,183,191,193
<div class="tooltip">ATOMS15<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=193,195,201,203
<div class="tooltip">ATOMS16<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=203,205,215,217
<div class="tooltip">ATOMS17<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=217,219,226,228
<div class="tooltip">ATOMS18<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=228,230,237,239
<div class="tooltip">ATOMS19<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=239,241,244,246
<div class="tooltip">ATOMS20<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=246,248,254,256
<div class="tooltip">ATOMS21<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=256,258,273,275
<div class="tooltip">ATOMS22<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=275,277,280,282
<div class="tooltip">ATOMS23<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=282,284,291,293
<div class="tooltip">ATOMS24<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=293,295,303,305
<div class="tooltip">ATOMS25<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=305,307,322,324
<div class="tooltip">ATOMS26<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=324,326,329,331
<div class="tooltip">ATOMS27<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=331,333,341,343
<div class="tooltip">ATOMS28<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=343,345,351,353
<div class="tooltip">ATOMS29<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=353,355,368,370
<div class="tooltip">ATOMS30<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=370,372,379,381
<div class="tooltip">ATOMS31<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=381,383,394,396
<div class="tooltip">ATOMS32<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=396,398,409,411
<div class="tooltip">ATOMS33<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=411,413,421,423
<div class="tooltip">ATOMS34<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=423,425,438,440
<div class="tooltip">ATOMS35<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=440,442,457,459
<div class="tooltip">ATOMS36<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=459,461,474,476
<div class="tooltip">ATOMS37<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=476,478,484,486
<div class="tooltip">ATOMS38<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=486,488,494,496
<div class="tooltip">ATOMS39<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=496,498,510,512
<div class="tooltip">ATOMS40<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=512,514,524,526
<div class="tooltip">ATOMS41<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=526,528,541,543
<div class="tooltip">ATOMS42<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=543,545,552,554
<div class="tooltip">ATOMS43<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=554,556,571,573
<div class="tooltip">ATOMS44<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=573,575,586,588
<div class="tooltip">ATOMS45<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=588,590,600,602
<div class="tooltip">ATOMS46<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=602,604,616,618
<div class="tooltip">ATOMS47<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=618,620,640,642
<div class="tooltip">ATOMS48<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=642,644,654,656
<div class="tooltip">ATOMS49<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=656,658,666,668
<div class="tooltip">ATOMS50<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=668,670,685,687
<div class="tooltip">ATOMS51<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=687,689,707,709
<div class="tooltip">ATOMS52<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=709,711,721,723
<div class="tooltip">ATOMS53<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=723,725,736,738
<div class="tooltip">ATOMS54<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=738,740,743,745
<div class="tooltip">ATOMS55<div class="right">the atoms involved for each of the torsions you wish to calculate<i></i></div></div>=745,747,765,767
 <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/WT-metaD.c22star/plumed2.datab" onclick='showPath("data/WT-metaD.c22star/plumed2.dat","data/WT-metaD.c22star/plumed2.datab","data/WT-metaD.c22star/plumed2.datab_shortcut","black")'>ab</b><span style="display:none;" id="data/WT-metaD.c22star/plumed2.datab_shortcut">The ALPHABETA action with label <b>ab</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ab</td><td width="5%"><font color="black">scalar</font></td><td>the alpha beta CV</td></tr></table></span>
... ALPHABETA
</span><span id="data/WT-metaD.c22star/plumed2.datab_long" style="display:none;"><span style="color:blue" class="comment"># PLUMED interprets the command:
</span><span class="toggler" style="color:red" onclick='toggleDisplay("data/WT-metaD.c22star/plumed2.datab")'># ALPHABETA ...</span>
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
<b name="data/WT-metaD.c22star/plumed2.datab_torsions" onclick='showPath("data/WT-metaD.c22star/plumed2.dat","data/WT-metaD.c22star/plumed2.datab_torsions","data/WT-metaD.c22star/plumed2.datab_torsions","blue")'>ab_torsions</b><span style="display:none;" id="data/WT-metaD.c22star/plumed2.datab_torsions">The TORSION action with label <b>ab_torsions</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ab_torsions</td><td width="5%"><font color="blue">vector</font></td><td>the TORSION for each set of specified atoms</td></tr></table></span>: <div class="tooltip" style="color:green">TORSION<div class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS1<div class="right">the four atoms involved in the torsional angle<i></i></div></div>=1,5,8,10 <div class="tooltip">ATOMS2<div class="right">the four atoms involved in the torsional angle<i></i></div></div>=10,12,20,22 <div class="tooltip">ATOMS3<div class="right">the four atoms involved in the torsional angle<i></i></div></div>=22,24,39,41 <div class="tooltip">ATOMS4<div class="right">the four atoms involved in the torsional angle<i></i></div></div>=41,43,50,52 <div class="tooltip">ATOMS5<div class="right">the four atoms involved in the torsional angle<i></i></div></div>=52,54,57,59     <span style="color:blue" class="comment"># Action input conctinues with 50 further ATOMSn keywords, </span>
<b name="data/WT-metaD.c22star/plumed2.datab_ref" onclick='showPath("data/WT-metaD.c22star/plumed2.dat","data/WT-metaD.c22star/plumed2.datab_ref","data/WT-metaD.c22star/plumed2.datab_ref","blue")'>ab_ref</b><span style="display:none;" id="data/WT-metaD.c22star/plumed2.datab_ref">The CONSTANT action with label <b>ab_ref</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ab_ref</td><td width="5%"><font color="blue">vector</font></td><td>the constant value that was read from the plumed input</td></tr></table></span>: <div class="tooltip" style="color:green">CONSTANT<div class="right">Create a constant value that can be passed to actions <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">VALUES<div class="right">the numbers that are in your constant value<i></i></div></div>=-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540,-0.78540
<b name="data/WT-metaD.c22star/plumed2.datab_coeff" onclick='showPath("data/WT-metaD.c22star/plumed2.dat","data/WT-metaD.c22star/plumed2.datab_coeff","data/WT-metaD.c22star/plumed2.datab_coeff","blue")'>ab_coeff</b><span style="display:none;" id="data/WT-metaD.c22star/plumed2.datab_coeff">The CONSTANT action with label <b>ab_coeff</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ab_coeff</td><td width="5%"><font color="blue">vector</font></td><td>the constant value that was read from the plumed input</td></tr></table></span>: <div class="tooltip" style="color:green">CONSTANT<div class="right">Create a constant value that can be passed to actions <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_n_s_t_a_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">VALUES<div class="right">the numbers that are in your constant value<i></i></div></div>=1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1
<b name="data/WT-metaD.c22star/plumed2.datab_comb" onclick='showPath("data/WT-metaD.c22star/plumed2.dat","data/WT-metaD.c22star/plumed2.datab_comb","data/WT-metaD.c22star/plumed2.datab_comb","blue")'>ab_comb</b><span style="display:none;" id="data/WT-metaD.c22star/plumed2.datab_comb">The COMBINE action with label <b>ab_comb</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ab_comb</td><td width="5%"><font color="blue">vector</font></td><td>the vector obtained by doing an element-wise application of a linear compbination to the input vectors</td></tr></table></span>: <div class="tooltip" style="color:green">COMBINE<div class="right">Calculate a polynomial combination of a set of other variables. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_m_b_i_n_e.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input to this function<i></i></div></div>=<b name="data/WT-metaD.c22star/plumed2.datab_torsions">ab_torsions</b>,<b name="data/WT-metaD.c22star/plumed2.datab_ref">ab_ref</b> <div class="tooltip">COEFFICIENTS<div class="right"> the coefficients of the arguments in your function<i></i></div></div>=1,-1 <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO 
<b name="data/WT-metaD.c22star/plumed2.datab_cos" onclick='showPath("data/WT-metaD.c22star/plumed2.dat","data/WT-metaD.c22star/plumed2.datab_cos","data/WT-metaD.c22star/plumed2.datab_cos","blue")'>ab_cos</b><span style="display:none;" id="data/WT-metaD.c22star/plumed2.datab_cos">The CUSTOM action with label <b>ab_cos</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ab_cos</td><td width="5%"><font color="blue">vector</font></td><td>the vector obtained by doing an element-wise application of an arbitrary function to the input vectors</td></tr></table></span>: <div class="tooltip" style="color:green">CUSTOM<div class="right">Calculate a combination of variables using a custom expression. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_u_s_t_o_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input to this function<i></i></div></div>=<b name="data/WT-metaD.c22star/plumed2.datab_comb">ab_comb</b>,<b name="data/WT-metaD.c22star/plumed2.datab_coeff">ab_coeff</b> <div class="tooltip">FUNC<div class="right">the function you wish to evaluate<i></i></div></div>=y*(0.5+0.5*cos(x <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO 
<b name="data/WT-metaD.c22star/plumed2.datab" onclick='showPath("data/WT-metaD.c22star/plumed2.dat","data/WT-metaD.c22star/plumed2.datab","data/WT-metaD.c22star/plumed2.datab","black")'>ab</b><span style="display:none;" id="data/WT-metaD.c22star/plumed2.datab">The SUM action with label <b>ab</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ab</td><td width="5%"><font color="black">scalar</font></td><td>the sum of all the elements in the input vector</td></tr></table></span>: <div class="tooltip" style="color:green">SUM<div class="right">Calculate the sum of the arguments <a href="https://www.plumed.org/doc-master/user-doc/html/_s_u_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input to this function<i></i></div></div>=<b name="data/WT-metaD.c22star/plumed2.datab_cos">ab_cos</b> <div class="tooltip">PERIODIC<div class="right">if the output of your function is periodic then you should specify the periodicity of the function<i></i></div></div>=NO 
<span style="color:blue"># --- End of included input --- </span></span><br/><span id="data/WT-metaD.c22star/plumed2.datdefmeta_short"><div class="tooltip" style="color:green">METAD<div class="right">Used to performed metadynamics on one or more collective variables. This action has <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/WT-metaD.c22star/plumed2.datdefmeta");'>hidden defaults</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_e_t_a_d.html">More details</a><i></i></div></div> ...
  <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/WT-metaD.c22star/plumed2.datmeta" onclick='showPath("data/WT-metaD.c22star/plumed2.dat","data/WT-metaD.c22star/plumed2.datmeta","data/WT-metaD.c22star/plumed2.datmeta","black")'>meta</b><span style="display:none;" id="data/WT-metaD.c22star/plumed2.datmeta">The METAD action with label <b>meta</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">meta.bias</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the bias potential</td></tr></table></span>
  <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/WT-metaD.c22star/plumed2.datrg">rg</b>,<b name="data/WT-metaD.c22star/plumed2.datab">ab</b> <div class="tooltip">SIGMA<div class="right">the widths of the Gaussian hills<i></i></div></div>=0.2,1.0 <div class="tooltip">HEIGHT<div class="right">the heights of the Gaussian hills<i></i></div></div>=0.5 <div class="tooltip">PACE<div class="right">the frequency for hill addition<i></i></div></div>=1000
  <div class="tooltip">BIASFACTOR<div class="right">use well tempered metadynamics and use this bias factor<i></i></div></div>=4 <div class="tooltip">TEMP<div class="right">the system temperature - this is only needed if you are doing well-tempered metadynamics<i></i></div></div>=298
... METAD
</span><span id="data/WT-metaD.c22star/plumed2.datdefmeta_long" style="display:none;"><div class="tooltip" style="color:green">METAD<div class="right">Used to performed metadynamics on one or more collective variables. This action uses the <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/WT-metaD.c22star/plumed2.datdefmeta");'>defaults shown here</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_m_e_t_a_d.html">More details</a><i></i></div></div> ...
  <div class="tooltip">LABEL<div class="right">a label for the action so that its output can be referenced in the input to other actions<i></i></div></div>=<b name="data/WT-metaD.c22star/plumed2.datmeta" onclick='showPath("data/WT-metaD.c22star/plumed2.dat","data/WT-metaD.c22star/plumed2.datmeta","data/WT-metaD.c22star/plumed2.datmeta","black")'>meta</b>
  <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/WT-metaD.c22star/plumed2.datrg">rg</b>,<b name="data/WT-metaD.c22star/plumed2.datab">ab</b> <div class="tooltip">SIGMA<div class="right">the widths of the Gaussian hills<i></i></div></div>=0.2,1.0 <div class="tooltip">HEIGHT<div class="right">the heights of the Gaussian hills<i></i></div></div>=0.5 <div class="tooltip">PACE<div class="right">the frequency for hill addition<i></i></div></div>=1000
  <div class="tooltip">BIASFACTOR<div class="right">use well tempered metadynamics and use this bias factor<i></i></div></div>=4 <div class="tooltip">TEMP<div class="right">the system temperature - this is only needed if you are doing well-tempered metadynamics<i></i></div></div>=298
 <div class="tooltip">FILE<div class="right"> a file in which the list of added hills is stored<i></i></div></div>=HILLS
... METAD
</span><br/><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/WT-metaD.c22star/plumed2.datrg">rg</b>,<b name="data/WT-metaD.c22star/plumed2.datab">ab</b>,<b name="data/WT-metaD.c22star/plumed2.datmeta">meta.bias</b> <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=1000 <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=COLVAR
<br/><div class="tooltip" style="color:green">ENDPLUMED<div class="right">Terminate plumed input. <a href="https://www.plumed.org/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html" style="color:green">More details</a><i></i></div></div><span style="color:blue" class="comment">

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
115    119    127    129    -0.78540
129    131    138    140    -0.78540
140    142    153    155    -0.78540
155    157    177    179    -0.78540
179    183    191    193    -0.78540
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
119
131
142
157
183
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
