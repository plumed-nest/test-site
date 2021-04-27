**Project ID:** [plumID:19.035]({{ '/' | absolute_url }}eggs/19/035/)  
**Source:** plumed.dat  
**Originally used with PLUMED version:** 2.2.3  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue">###</span>
<span style="color:blue">### CENTER OF MASS DEFINITIONS</span>
<span style="color:blue">###</span>

<span style="color:blue"># COM of both protomers (only BB atoms)</span>
COM1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=1,3,5,7,8,10,12,14,16,17,19,23,25,27,29,31,33,35,36,38,42,43,45,49,51,53,55,59,61,63,65,68,72,74,77,79,82,84,85,87,89,91,95,97,101,103,105,106,108,109,111,112,114,115,117,119,121,123,125,129,131,133,135,137,141,143,145,146,148,153,155,159,160,162,164,166,168,171,173,175,177,179,181,183,187,191,193,195,199,201,203,205,209,211,213,215,217,219,221,223,225,228,232,234,235,237,243,247,249,251,254,255,257,259,263,266,268,270,273,275,276,279,281,283,285,287,289,291,296,298,300,302,304,305,307,308,310,312,314,316,320,322,323,325,327,330,334,337,339,340,342,344,346,348,350,352,354,358,360,364,366,368,373,377,382,384,386,388,390,393,395,397,399,403,405,409,410,414,416,418,420,422,424,426,428,430,432,434,438,439,441,443,445,447,450,452,455,457,459,462,464,466,468,469,471,474,476,479,481,484,486,488,491,494,496,498,501,503,505,507,509,511,513,514,516,520,522,524,526,531,533,535,537,541,543,547,549,551,553,556,557,559,561,563,565,567,569,571,573,577,579,581,583,585,590,594,598,600,602,603,605,606,610,612,614,616,618,620,622,624,626,628,632,633,637,639,641,643,645,649,652,655,657,661,664,666,670,672
COM2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=674,676,678,680,681,683,685,687,689,690,692,696,698,700,702,704,706,708,709,711,715,716,718,722,724,726,728,732,734,736,738,741,745,747,750,752,755,757,758,760,762,764,768,770,774,776,778,779,781,782,784,785,787,788,790,792,794,796,798,802,804,806,808,810,814,816,818,819,821,826,828,832,833,835,837,839,841,844,846,848,850,852,854,856,860,864,866,868,872,874,876,878,882,884,886,888,890,892,894,896,898,901,905,907,908,910,916,920,922,924,927,928,930,932,936,939,941,943,946,948,949,952,954,956,958,960,962,964,969,971,973,975,977,978,980,981,983,985,987,989,993,995,996,998,1000,1003,1007,1010,1012,1013,1015,1017,1019,1021,1023,1025,1027,1031,1033,1037,1039,1041,1046,1050,1055,1057,1059,1061,1063,1066,1068,1070,1072,1076,1078,1082,1083,1087,1089,1091,1093,1095,1097,1099,1101,1103,1105,1107,1111,1112,1114,1116,1118,1120,1123,1125,1128,1130,1132,1135,1137,1139,1141,1142,1144,1147,1149,1152,1154,1157,1159,1161,1164,1167,1169,1171,1174,1176,1178,1180,1182,1184,1186,1187,1189,1193,1195,1197,1199,1204,1206,1208,1210,1214,1216,1220,1222,1224,1226,1229,1230,1232,1234,1236,1238,1240,1242,1244,1246,1250,1252,1254,1256,1258,1263,1267,1271,1273,1275,1276,1278,1279,1283,1285,1287,1289,1291,1293,1295,1297,1299,1301,1305,1306,1310,1312,1314,1316,1318,1322,1325,1328,1330,1334,1337,1339,1343,1345
<span style="color:blue"># COM of Helix 1 for both protomers (only BB atoms)</span>
HCOM1: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=1,3,5,7,8,10,12,14,16,17,19,23,25,27,29,31,33,35,36,38,42,43,45,49,51,53,55,59,61,63,65
HCOM2: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=674,676,678,680,681,683,685,687,689,690,692,696,698,700,702,704,706,708,709,711,715,716,718,722,724,726,728,732,734,736,738

<span style="color:blue">###</span>
<span style="color:blue">### DEFINITION DUMMY ATOMS</span>
<span style="color:blue">###</span>

DUM1: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=20424
DUM2: <a href="https://plumed.github.io/doc-master/user-doc/html/_g_r_o_u_p.html">GROUP</a> ATOMS=20425
ZAXE: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=DUM1,DUM2 COMPONENTS

<span style="color:blue">###</span>
<span style="color:blue">### DEFINITION OF DISTANCE AND ANGLES</span>
<span style="color:blue">###</span>

DIST: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=COM1,COM2 
ANG1: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=HCOM1,COM1 AXIS=DUM1,DUM2 VECTOR2=COM2,COM1
ANG2: <a href="https://plumed.github.io/doc-master/user-doc/html/_t_o_r_s_i_o_n.html">TORSION</a> VECTOR1=HCOM2,COM2 AXIS=DUM1,DUM2 VECTOR2=COM1,COM2

<span style="color:blue">###</span>
<span style="color:blue">### DEFINITION OF UMBRELLA SAMPLING RESTRAINTS</span>
<span style="color:blue">###</span>

RESTUS: <a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_r_a_i_n_t.html">RESTRAINT</a> ARG=DIST,ANG1,ANG2 KAPPA=250.0,100.0,100.0 AT=4.400,-1.581,-1.284

<span style="color:blue">###</span>
<span style="color:blue">### PRINTING OUT</span>
<span style="color:blue">###</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=ZAXE.x,ZAXE.y,ZAXE.z STRIDE=25000 FILE=ZAXE.dat
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=DIST,ANG1,ANG2       STRIDE=25000 FILE=COLVALS.dat
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=RESTUS.bias          STRIDE=25000 FILE=EBIAS.dat

</pre>{% endraw %}
