**Project ID:** [plumID:19.035]({{ '/' | absolute_url }}eggs/19/035/)  
**Source:** plumed.dat  
**Originally used with PLUMED version:** 2.2.3  
**Stable:** [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}
<div style="width: 100%; float:left">
<div style="width: 90%; float:left" id="value_details_data/plumed.dat"> Click on the labels of the actions for more information on what each action computes </div>
<div style="width: 10%; float:left"><table><tr><td style="padding:1px"><a href="plumed.dat.plumed.stderr"><img src="https://img.shields.io/badge/v2.9-passing-green.svg" alt="tested onv2.9" /></a></td></tr><tr><td style="padding:1px"><a href="plumed.dat.plumed_master.stderr"><img src="https://img.shields.io/badge/master-passing-green.svg" alt="tested onmaster" /></a></td></tr></table></div></div>
<pre style="width=97%;">
<span style="color:blue" class="comment">###</span>
<span style="color:blue" class="comment">### CENTER OF MASS DEFINITIONS</span>
<span style="color:blue" class="comment">###</span>
<br/><span style="color:blue" class="comment"># COM of both protomers (only BB atoms)</span>
<b name="data/plumed.datCOM1" onclick='showPath("data/plumed.dat","data/plumed.datCOM1","data/plumed.datCOM1","violet")'>COM1</b><span style="display:none;" id="data/plumed.datCOM1">The COM action with label <b>COM1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">COM1</td><td width="5%"><font color="violet">atoms</font></td><td>virtual atom calculated by COM action</td></tr></table></span>: <div class="tooltip" style="color:green">COM<div class="right">Calculate the center of mass for a group of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the list of atoms which are involved the virtual atom's definition<i></i></div></div>=1,3,5,7,8,10,12,14,16,17,19,23,25,27,29,31,33,35,36,38,42,43,45,49,51,53,55,59,61,63,65,68,72,74,77,79,82,84,85,87,89,91,95,97,101,103,105,106,108,109,111,112,114,115,117,119,121,123,125,129,131,133,135,137,141,143,145,146,148,153,155,159,160,162,164,166,168,171,173,175,177,179,181,183,187,191,193,195,199,201,203,205,209,211,213,215,217,219,221,223,225,228,232,234,235,237,243,247,249,251,254,255,257,259,263,266,268,270,273,275,276,279,281,283,285,287,289,291,296,298,300,302,304,305,307,308,310,312,314,316,320,322,323,325,327,330,334,337,339,340,342,344,346,348,350,352,354,358,360,364,366,368,373,377,382,384,386,388,390,393,395,397,399,403,405,409,410,414,416,418,420,422,424,426,428,430,432,434,438,439,441,443,445,447,450,452,455,457,459,462,464,466,468,469,471,474,476,479,481,484,486,488,491,494,496,498,501,503,505,507,509,511,513,514,516,520,522,524,526,531,533,535,537,541,543,547,549,551,553,556,557,559,561,563,565,567,569,571,573,577,579,581,583,585,590,594,598,600,602,603,605,606,610,612,614,616,618,620,622,624,626,628,632,633,637,639,641,643,645,649,652,655,657,661,664,666,670,672
<b name="data/plumed.datCOM2" onclick='showPath("data/plumed.dat","data/plumed.datCOM2","data/plumed.datCOM2","violet")'>COM2</b><span style="display:none;" id="data/plumed.datCOM2">The COM action with label <b>COM2</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">COM2</td><td width="5%"><font color="violet">atoms</font></td><td>virtual atom calculated by COM action</td></tr></table></span>: <div class="tooltip" style="color:green">COM<div class="right">Calculate the center of mass for a group of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the list of atoms which are involved the virtual atom's definition<i></i></div></div>=674,676,678,680,681,683,685,687,689,690,692,696,698,700,702,704,706,708,709,711,715,716,718,722,724,726,728,732,734,736,738,741,745,747,750,752,755,757,758,760,762,764,768,770,774,776,778,779,781,782,784,785,787,788,790,792,794,796,798,802,804,806,808,810,814,816,818,819,821,826,828,832,833,835,837,839,841,844,846,848,850,852,854,856,860,864,866,868,872,874,876,878,882,884,886,888,890,892,894,896,898,901,905,907,908,910,916,920,922,924,927,928,930,932,936,939,941,943,946,948,949,952,954,956,958,960,962,964,969,971,973,975,977,978,980,981,983,985,987,989,993,995,996,998,1000,1003,1007,1010,1012,1013,1015,1017,1019,1021,1023,1025,1027,1031,1033,1037,1039,1041,1046,1050,1055,1057,1059,1061,1063,1066,1068,1070,1072,1076,1078,1082,1083,1087,1089,1091,1093,1095,1097,1099,1101,1103,1105,1107,1111,1112,1114,1116,1118,1120,1123,1125,1128,1130,1132,1135,1137,1139,1141,1142,1144,1147,1149,1152,1154,1157,1159,1161,1164,1167,1169,1171,1174,1176,1178,1180,1182,1184,1186,1187,1189,1193,1195,1197,1199,1204,1206,1208,1210,1214,1216,1220,1222,1224,1226,1229,1230,1232,1234,1236,1238,1240,1242,1244,1246,1250,1252,1254,1256,1258,1263,1267,1271,1273,1275,1276,1278,1279,1283,1285,1287,1289,1291,1293,1295,1297,1299,1301,1305,1306,1310,1312,1314,1316,1318,1322,1325,1328,1330,1334,1337,1339,1343,1345
<span style="color:blue" class="comment"># COM of Helix 1 for both protomers (only BB atoms)</span>
<b name="data/plumed.datHCOM1" onclick='showPath("data/plumed.dat","data/plumed.datHCOM1","data/plumed.datHCOM1","violet")'>HCOM1</b><span style="display:none;" id="data/plumed.datHCOM1">The COM action with label <b>HCOM1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">HCOM1</td><td width="5%"><font color="violet">atoms</font></td><td>virtual atom calculated by COM action</td></tr></table></span>: <div class="tooltip" style="color:green">COM<div class="right">Calculate the center of mass for a group of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the list of atoms which are involved the virtual atom's definition<i></i></div></div>=1,3,5,7,8,10,12,14,16,17,19,23,25,27,29,31,33,35,36,38,42,43,45,49,51,53,55,59,61,63,65
<b name="data/plumed.datHCOM2" onclick='showPath("data/plumed.dat","data/plumed.datHCOM2","data/plumed.datHCOM2","violet")'>HCOM2</b><span style="display:none;" id="data/plumed.datHCOM2">The COM action with label <b>HCOM2</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">HCOM2</td><td width="5%"><font color="violet">atoms</font></td><td>virtual atom calculated by COM action</td></tr></table></span>: <div class="tooltip" style="color:green">COM<div class="right">Calculate the center of mass for a group of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_c_o_m.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the list of atoms which are involved the virtual atom's definition<i></i></div></div>=674,676,678,680,681,683,685,687,689,690,692,696,698,700,702,704,706,708,709,711,715,716,718,722,724,726,728,732,734,736,738
<br/><span style="color:blue" class="comment">###</span>
<span style="color:blue" class="comment">### DEFINITION DUMMY ATOMS</span>
<span style="color:blue" class="comment">###</span>
<br/><b name="data/plumed.datDUM1" onclick='showPath("data/plumed.dat","data/plumed.datDUM1","data/plumed.datDUM1","violet")'>DUM1</b><span style="display:none;" id="data/plumed.datDUM1">The GROUP action with label <b>DUM1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">DUM1</td><td width="5%"><font color="violet">atoms</font></td><td>indices of atoms specified in GROUP</td></tr></table></span>: <div class="tooltip" style="color:green">GROUP<div class="right">Define a group of atoms so that a particular list of atoms can be referenced with a single label in definitions of CVs or virtual atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_g_r_o_u_p.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the numerical indexes for the set of atoms in the group<i></i></div></div>=20424
<b name="data/plumed.datDUM2" onclick='showPath("data/plumed.dat","data/plumed.datDUM2","data/plumed.datDUM2","violet")'>DUM2</b><span style="display:none;" id="data/plumed.datDUM2">The GROUP action with label <b>DUM2</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">DUM2</td><td width="5%"><font color="violet">atoms</font></td><td>indices of atoms specified in GROUP</td></tr></table></span>: <div class="tooltip" style="color:green">GROUP<div class="right">Define a group of atoms so that a particular list of atoms can be referenced with a single label in definitions of CVs or virtual atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_g_r_o_u_p.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the numerical indexes for the set of atoms in the group<i></i></div></div>=20425
<b name="data/plumed.datZAXE" onclick='showPath("data/plumed.dat","data/plumed.datZAXE","data/plumed.datZAXE","black")'>ZAXE</b><span style="display:none;" id="data/plumed.datZAXE">The DISTANCE action with label <b>ZAXE</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ZAXE.x</td><td width="5%"><font color="black">scalar</font></td><td>the x-component of the vector connecting the two atoms</td></tr><tr><td width="5%">ZAXE.y</td><td width="5%"><font color="black">scalar</font></td><td>the y-component of the vector connecting the two atoms</td></tr><tr><td width="5%">ZAXE.z</td><td width="5%"><font color="black">scalar</font></td><td>the z-component of the vector connecting the two atoms</td></tr></table></span>: <div class="tooltip" style="color:green">DISTANCE<div class="right">Calculate the distance between a pair of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=<b name="data/plumed.datDUM1">DUM1</b>,<b name="data/plumed.datDUM2">DUM2</b> <div class="tooltip">COMPONENTS<div class="right"> calculate the x, y and z components of the distance separately and store them as label<i></i></div></div>
<br/><span style="color:blue" class="comment">###</span>
<span style="color:blue" class="comment">### DEFINITION OF DISTANCE AND ANGLES</span>
<span style="color:blue" class="comment">###</span>
<br/><b name="data/plumed.datDIST" onclick='showPath("data/plumed.dat","data/plumed.datDIST","data/plumed.datDIST","black")'>DIST</b><span style="display:none;" id="data/plumed.datDIST">The DISTANCE action with label <b>DIST</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">DIST</td><td width="5%"><font color="black">scalar</font></td><td>the DISTANCE between this pair of atoms</td></tr></table></span>: <div class="tooltip" style="color:green">DISTANCE<div class="right">Calculate the distance between a pair of atoms. <a href="https://www.plumed.org/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ATOMS<div class="right">the pair of atom that we are calculating the distance between<i></i></div></div>=<b name="data/plumed.datCOM1">COM1</b>,<b name="data/plumed.datCOM2">COM2</b> 
<b name="data/plumed.datANG1" onclick='showPath("data/plumed.dat","data/plumed.datANG1","data/plumed.datANG1","black")'>ANG1</b><span style="display:none;" id="data/plumed.datANG1">The TORSION action with label <b>ANG1</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ANG1</td><td width="5%"><font color="black">scalar</font></td><td>the TORSION involving these atoms</td></tr></table></span>: <div class="tooltip" style="color:green">TORSION<div class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">VECTOR1<div class="right">two atoms that define a vector<i></i></div></div>=<b name="data/plumed.datHCOM1">HCOM1</b>,<b name="data/plumed.datCOM1">COM1</b> <div class="tooltip">AXIS<div class="right">two atoms that define an axis<i></i></div></div>=<b name="data/plumed.datDUM1">DUM1</b>,<b name="data/plumed.datDUM2">DUM2</b> <div class="tooltip">VECTOR2<div class="right">two atoms that define a vector<i></i></div></div>=<b name="data/plumed.datCOM2">COM2</b>,<b name="data/plumed.datCOM1">COM1</b>
<b name="data/plumed.datANG2" onclick='showPath("data/plumed.dat","data/plumed.datANG2","data/plumed.datANG2","black")'>ANG2</b><span style="display:none;" id="data/plumed.datANG2">The TORSION action with label <b>ANG2</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">ANG2</td><td width="5%"><font color="black">scalar</font></td><td>the TORSION involving these atoms</td></tr></table></span>: <div class="tooltip" style="color:green">TORSION<div class="right">Calculate a torsional angle. <a href="https://www.plumed.org/doc-master/user-doc/html/_t_o_r_s_i_o_n.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">VECTOR1<div class="right">two atoms that define a vector<i></i></div></div>=<b name="data/plumed.datHCOM2">HCOM2</b>,<b name="data/plumed.datCOM2">COM2</b> <div class="tooltip">AXIS<div class="right">two atoms that define an axis<i></i></div></div>=<b name="data/plumed.datDUM1">DUM1</b>,<b name="data/plumed.datDUM2">DUM2</b> <div class="tooltip">VECTOR2<div class="right">two atoms that define a vector<i></i></div></div>=<b name="data/plumed.datCOM1">COM1</b>,<b name="data/plumed.datCOM2">COM2</b>
<br/><span style="color:blue" class="comment">###</span>
<span style="color:blue" class="comment">### DEFINITION OF UMBRELLA SAMPLING RESTRAINTS</span>
<span style="color:blue" class="comment">###</span>
<br/><span id="data/plumed.datdefRESTUS_short"><b name="data/plumed.datRESTUS" onclick='showPath("data/plumed.dat","data/plumed.datRESTUS","data/plumed.datRESTUS","black")'>RESTUS</b><span style="display:none;" id="data/plumed.datRESTUS">The RESTRAINT action with label <b>RESTUS</b> calculates the following quantities:<table  align="center" frame="void" width="95%" cellpadding="5%"><tr><td width="5%"><b> Quantity </b>  </td><td width="5%"><b> Type </b>  </td><td><b> Description </b> </td></tr><tr><td width="5%">RESTUS.bias</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the bias potential</td></tr><tr><td width="5%">RESTUS.force2</td><td width="5%"><font color="black">scalar</font></td><td>the instantaneous value of the squared force due to this bias potential</td></tr></table></span>: <div class="tooltip" style="color:green">RESTRAINT<div class="right">Adds harmonic and/or linear restraints on one or more variables. This action has <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/plumed.datdefRESTUS");'>hidden defaults</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the arguments on which the bias is acting<i></i></div></div>=<b name="data/plumed.datDIST">DIST</b>,<b name="data/plumed.datANG1">ANG1</b>,<b name="data/plumed.datANG2">ANG2</b> <div class="tooltip">KAPPA<div class="right"> specifies that the restraint is harmonic and what the values of the force constants on each of the variables are<i></i></div></div>=250.0,100.0,100.0 <div class="tooltip">AT<div class="right">the position of the restraint<i></i></div></div>=4.400,-1.581,-1.284
</span><span id="data/plumed.datdefRESTUS_long" style="display:none;"><b name="data/plumed.datRESTUS" onclick='showPath("data/plumed.dat","data/plumed.datRESTUS","data/plumed.datRESTUS","black")'>RESTUS</b>: <div class="tooltip" style="color:green">RESTRAINT<div class="right">Adds harmonic and/or linear restraints on one or more variables. This action uses the <a class="toggler" href='javascript:;' onclick='toggleDisplay("data/plumed.datdefRESTUS");'>defaults shown here</a>. <a href="https://www.plumed.org/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the arguments on which the bias is acting<i></i></div></div>=<b name="data/plumed.datDIST">DIST</b>,<b name="data/plumed.datANG1">ANG1</b>,<b name="data/plumed.datANG2">ANG2</b> <div class="tooltip">KAPPA<div class="right"> specifies that the restraint is harmonic and what the values of the force constants on each of the variables are<i></i></div></div>=250.0,100.0,100.0 <div class="tooltip">AT<div class="right">the position of the restraint<i></i></div></div>=4.400,-1.581,-1.284  <div class="tooltip">SLOPE<div class="right"> specifies that the restraint is linear and what the values of the force constants on each of the variables are<i></i></div></div>=0.0,0.0,0.0
</span><br/><span style="color:blue" class="comment">###</span>
<span style="color:blue" class="comment">### PRINTING OUT</span>
<span style="color:blue" class="comment">###</span>
<div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/plumed.datZAXE">ZAXE.x</b>,<b name="data/plumed.datZAXE">ZAXE.y</b>,<b name="data/plumed.datZAXE">ZAXE.z</b> <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=25000 <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=<b name="data/plumed.datZAXE">ZAXE.dat</b>
<span style="display:none;" id="data/plumed.dat">The PRINT action with label <b></b> calculates something</span><div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/plumed.datDIST">DIST</b>,<b name="data/plumed.datANG1">ANG1</b>,<b name="data/plumed.datANG2">ANG2</b>       <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=25000 <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=COLVALS.dat
<div class="tooltip" style="color:green">PRINT<div class="right">Print quantities to a file. <a href="https://www.plumed.org/doc-master/user-doc/html/_p_r_i_n_t.html" style="color:green">More details</a><i></i></div></div> <div class="tooltip">ARG<div class="right">the input for this action is the scalar output from one or more other actions<i></i></div></div>=<b name="data/plumed.datRESTUS">RESTUS.bias</b>          <div class="tooltip">STRIDE<div class="right"> the frequency with which the quantities of interest should be output<i></i></div></div>=25000 <div class="tooltip">FILE<div class="right">the name of the file on which to output these quantities<i></i></div></div>=EBIAS.dat
</pre>
{% endraw %}