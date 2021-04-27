**Project ID:** [plumID:20.005]({{ '/' | absolute_url }}eggs/20/005/)  
**Source:** input_data/classical/FA-metaD/FA-MetaD_plumed.dat  
**Originally used with PLUMED version:** 2.5  
**Stable:** [raw zipped stdout](FA-MetaD_plumed.dat.plumed.stdout.txt.zip) - [stderr](FA-MetaD_plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](FA-MetaD_plumed.dat.plumed_master.stdout.txt.zip) - [stderr](FA-MetaD_plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue">#</span>
<span style="color:blue"># This is the input file needed to perform Multiple </span>
<span style="color:blue"># Walkers WT-MetaD simulation based on the pathCV </span>
<span style="color:blue">#</span>
<span style="color:blue"># This input file can be used with all the PLUMED versions >=2.5</span>
<span style="color:blue">#</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_o_l_i_n_f_o.html">MOLINFO</a> STRUCTURE=../input_files/first.pdb
<a href="https://plumed.github.io/doc-master/user-doc/html/_w_h_o_l_e_m_o_l_e_c_u_l_e_s.html">WHOLEMOLECULES</a> ENTITY0=1-6250

<span style="color:blue"># Definition of the center of mass of the ligand, considering only its heavy atoms</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=1,5,6,10,14,17,18,19,22,23,24,25,26,29  LABEL=ixo

<span style="color:blue"># Definition of the center of mass of the pocket</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=1396,1398,1400,1403,1404,1406,1408,1409,1411,1413,1415,1416,1449,1451,1453,1456,1458,1459,1495,1497,1499,1501,1505,1509,1510,2838,2840,2842,2845,2846,2848,2850,2852,2854,2856,2857,3605,3607,3609,3612,3613,3615,3617,3618,3620,3622,3624,3625 LABEL=pkt
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=ixo,pkt LABEL=d1 COMPONENTS NOPBC

<span style="color:blue"># Restraining potential of the ligand</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e.html">DISTANCE</a> ATOMS=ixo,pkt LABEL=restr NOPBC
sphere: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=restr AT=2.5 KAPPA=1000.

<span style="color:blue">#ligand</span>
ring:    <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=23,24,25,26,29
<span style="color:blue">#ixo:     COM ATOMS=1,5,6,10,14,17,18,19,22,23,24,25,26,29</span>

<span style="color:blue"># Trimetylammonium interactions </span>
ring244: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=3971,3972,3974,3976,3979,3981
ring221: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=3614,3615,3617,3619,3622,3624
ring86:  <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=1405,1406,1408,1410,1413,1415
oxy85:   <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=1394,1395

<span style="color:blue"># Ligand ring interactions</span>
val93:   <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=1501,1503,1507
ile160:  <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=2605,2609,2612
thr169:  <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=2740,2742,2746

<span style="color:blue"># all ligand interactions</span>
trp218:  <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=3566,3567,3569,3571,3572,3574,3576,3578,3580
cys158:  <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_m.html">COM</a> ATOMS=2572,2575


<span style="color:blue"># Definition of the contact maps for the pathCV</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t_m_a_p.html">CONTACTMAP</a> ...                                                         
ATOMS1=5,ring244     SWITCH1={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE1=0.324857000 WEIGHT1=0.333 
ATOMS2=5,ring221     SWITCH2={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE2=0.326715000 WEIGHT2=0.333 
ATOMS3=5,ring86      SWITCH3={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE3=0.317481000 WEIGHT3=0.333 
ATOMS4=5,oxy85       SWITCH4={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE4=0.916788000 WEIGHT4=1. 
ATOMS5=trp218,ring   SWITCH5={RATIONAL R_0=1.0 NN=6 MM=12}  REFERENCE5=0.988975000 WEIGHT5=1. 
ATOMS6=val93,ring    SWITCH6={RATIONAL R_0=1.0 NN=6 MM=12}  REFERENCE6=0.985199000 WEIGHT6=1. 
ATOMS7=ile160,ring   SWITCH7={RATIONAL R_0=1.2 NN=6 MM=12}  REFERENCE7=0.459210000 WEIGHT7=1. 
ATOMS8=5,cys158      SWITCH8={RATIONAL R_0=1.2 NN=6 MM=10}  REFERENCE8=0.532785000 WEIGHT8=1. 
ATOMS9=thr169,ring   SWITCH9={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE9=0.151720000 WEIGHT9=1.
LABEL=cm1                                                              
CMDIST                                                                 
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t_m_a_p.html">CONTACTMAP</a>                                                         
                                                                       
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t_m_a_p.html">CONTACTMAP</a> ...                                                         
ATOMS1=5,ring244     SWITCH1={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE1=0.322060000 WEIGHT1=0.333 
ATOMS2=5,ring221     SWITCH2={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE2=0.322125000 WEIGHT2=0.333 
ATOMS3=5,ring86      SWITCH3={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE3=0.318081000 WEIGHT3=0.333 
ATOMS4=5,oxy85       SWITCH4={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE4=0.940059000 WEIGHT4=1. 
ATOMS5=trp218,ring   SWITCH5={RATIONAL R_0=1.0 NN=6 MM=12}  REFERENCE5=0.974572000 WEIGHT5=1. 
ATOMS6=val93,ring    SWITCH6={RATIONAL R_0=1.0 NN=6 MM=12}  REFERENCE6=0.912335000 WEIGHT6=1. 
ATOMS7=ile160,ring   SWITCH7={RATIONAL R_0=1.2 NN=6 MM=12}  REFERENCE7=0.641878000 WEIGHT7=1. 
ATOMS8=5,cys158      SWITCH8={RATIONAL R_0=1.2 NN=6 MM=10}  REFERENCE8=0.522181000 WEIGHT8=1. 
ATOMS9=thr169,ring   SWITCH9={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE9=0.308574000 WEIGHT9=1.
LABEL=cm2                                                              
CMDIST                                                                 
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t_m_a_p.html">CONTACTMAP</a>                                                         
                                                                       
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t_m_a_p.html">CONTACTMAP</a> ...                                                         
ATOMS1=5,ring244     SWITCH1={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE1=0.320523000 WEIGHT1=0.333 
ATOMS2=5,ring221     SWITCH2={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE2=0.324186000 WEIGHT2=0.333 
ATOMS3=5,ring86      SWITCH3={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE3=0.315741000 WEIGHT3=0.333 
ATOMS4=5,oxy85       SWITCH4={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE4=0.918387000 WEIGHT4=1. 
ATOMS5=trp218,ring   SWITCH5={RATIONAL R_0=1.0 NN=6 MM=12}  REFERENCE5=0.782751000 WEIGHT5=1. 
ATOMS6=val93,ring    SWITCH6={RATIONAL R_0=1.0 NN=6 MM=12}  REFERENCE6=0.416873000 WEIGHT6=1. 
ATOMS7=ile160,ring   SWITCH7={RATIONAL R_0=1.2 NN=6 MM=12}  REFERENCE7=0.918085000 WEIGHT7=1. 
ATOMS8=5,cys158      SWITCH8={RATIONAL R_0=1.2 NN=6 MM=10}  REFERENCE8=0.519385000 WEIGHT8=1. 
ATOMS9=thr169,ring   SWITCH9={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE9=0.736644000 WEIGHT9=1.
LABEL=cm3                                                              
CMDIST                                                                 
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t_m_a_p.html">CONTACTMAP</a>                                                         
                                                                       
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t_m_a_p.html">CONTACTMAP</a> ...                                                         
ATOMS1=5,ring244     SWITCH1={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE1=0.324818000 WEIGHT1=0.333 
ATOMS2=5,ring221     SWITCH2={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE2=0.316640000 WEIGHT2=0.333 
ATOMS3=5,ring86      SWITCH3={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE3=0.316240000 WEIGHT3=0.333 
ATOMS4=5,oxy85       SWITCH4={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE4=0.922710000 WEIGHT4=1. 
ATOMS5=trp218,ring   SWITCH5={RATIONAL R_0=1.0 NN=6 MM=12}  REFERENCE5=0.392776000 WEIGHT5=1. 
ATOMS6=val93,ring    SWITCH6={RATIONAL R_0=1.0 NN=6 MM=12}  REFERENCE6=0.178666000 WEIGHT6=1. 
ATOMS7=ile160,ring   SWITCH7={RATIONAL R_0=1.2 NN=6 MM=12}  REFERENCE7=0.919086000 WEIGHT7=1. 
ATOMS8=5,cys158      SWITCH8={RATIONAL R_0=1.2 NN=6 MM=10}  REFERENCE8=0.532663000 WEIGHT8=1. 
ATOMS9=thr169,ring   SWITCH9={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE9=0.949034000 WEIGHT9=1.
LABEL=cm4                                                              
CMDIST                                                                 
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t_m_a_p.html">CONTACTMAP</a>                                                         
                                                                       
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t_m_a_p.html">CONTACTMAP</a> ...                                                         
ATOMS1=5,ring244     SWITCH1={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE1=0.326082000 WEIGHT1=0.333 
ATOMS2=5,ring221     SWITCH2={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE2=0.325629000 WEIGHT2=0.333 
ATOMS3=5,ring86      SWITCH3={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE3=0.303538000 WEIGHT3=0.333 
ATOMS4=5,oxy85       SWITCH4={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE4=0.887596000 WEIGHT4=1. 
ATOMS5=trp218,ring   SWITCH5={RATIONAL R_0=1.0 NN=6 MM=12}  REFERENCE5=0.143690000 WEIGHT5=1. 
ATOMS6=val93,ring    SWITCH6={RATIONAL R_0=1.0 NN=6 MM=12}  REFERENCE6=0.064591000 WEIGHT6=1. 
ATOMS7=ile160,ring   SWITCH7={RATIONAL R_0=1.2 NN=6 MM=12}  REFERENCE7=0.999237000 WEIGHT7=1. 
ATOMS8=5,cys158      SWITCH8={RATIONAL R_0=1.2 NN=6 MM=10}  REFERENCE8=0.587326000 WEIGHT8=1. 
ATOMS9=thr169,ring   SWITCH9={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE9=0.878697000 WEIGHT9=1.
LABEL=cm5                                                              
CMDIST                                                                 
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t_m_a_p.html">CONTACTMAP</a>                                                         
                                                                       
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t_m_a_p.html">CONTACTMAP</a> ...                                                         
ATOMS1=5,ring244     SWITCH1={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE1=0.328269000 WEIGHT1=0.333 
ATOMS2=5,ring221     SWITCH2={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE2=0.327338000 WEIGHT2=0.333 
ATOMS3=5,ring86      SWITCH3={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE3=0.320984000 WEIGHT3=0.333 
ATOMS4=5,oxy85       SWITCH4={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE4=0.914713000 WEIGHT4=1. 
ATOMS5=trp218,ring   SWITCH5={RATIONAL R_0=1.0 NN=6 MM=12}  REFERENCE5=0.062782000 WEIGHT5=1. 
ATOMS6=val93,ring    SWITCH6={RATIONAL R_0=1.0 NN=6 MM=12}  REFERENCE6=0.033614000 WEIGHT6=1. 
ATOMS7=ile160,ring   SWITCH7={RATIONAL R_0=1.2 NN=6 MM=12}  REFERENCE7=0.998120000 WEIGHT7=1. 
ATOMS8=5,cys158      SWITCH8={RATIONAL R_0=1.2 NN=6 MM=10}  REFERENCE8=0.734615000 WEIGHT8=1. 
ATOMS9=thr169,ring   SWITCH9={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE9=0.777428000 WEIGHT9=1.
LABEL=cm6                                                              
CMDIST                                                                 
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t_m_a_p.html">CONTACTMAP</a>                                                         
                                                                       
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t_m_a_p.html">CONTACTMAP</a> ...                                                         
ATOMS1=5,ring244     SWITCH1={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE1=0.326594000 WEIGHT1=0.333 
ATOMS2=5,ring221     SWITCH2={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE2=0.326341000 WEIGHT2=0.333 
ATOMS3=5,ring86      SWITCH3={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE3=0.321865000 WEIGHT3=0.333 
ATOMS4=5,oxy85       SWITCH4={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE4=0.893738000 WEIGHT4=1. 
ATOMS5=trp218,ring   SWITCH5={RATIONAL R_0=1.0 NN=6 MM=12}  REFERENCE5=0.049625000 WEIGHT5=1. 
ATOMS6=val93,ring    SWITCH6={RATIONAL R_0=1.0 NN=6 MM=12}  REFERENCE6=0.020003000 WEIGHT6=1. 
ATOMS7=ile160,ring   SWITCH7={RATIONAL R_0=1.2 NN=6 MM=12}  REFERENCE7=0.996938000 WEIGHT7=1. 
ATOMS8=5,cys158      SWITCH8={RATIONAL R_0=1.2 NN=6 MM=10}  REFERENCE8=0.648535000 WEIGHT8=1. 
ATOMS9=thr169,ring   SWITCH9={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE9=0.469544000 WEIGHT9=1.
LABEL=cm7                                                              
CMDIST                                                                 
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t_m_a_p.html">CONTACTMAP</a>                                                         
                                                                       
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t_m_a_p.html">CONTACTMAP</a> ...                                                         
ATOMS1=5,ring244     SWITCH1={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE1=0.326402000 WEIGHT1=0.333 
ATOMS2=5,ring221     SWITCH2={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE2=0.324290000 WEIGHT2=0.333 
ATOMS3=5,ring86      SWITCH3={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE3=0.317068000 WEIGHT3=0.333 
ATOMS4=5,oxy85       SWITCH4={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE4=0.765955000 WEIGHT4=1. 
ATOMS5=trp218,ring   SWITCH5={RATIONAL R_0=1.0 NN=6 MM=12}  REFERENCE5=0.036467000 WEIGHT5=1. 
ATOMS6=val93,ring    SWITCH6={RATIONAL R_0=1.0 NN=6 MM=12}  REFERENCE6=0.015861000 WEIGHT6=1. 
ATOMS7=ile160,ring   SWITCH7={RATIONAL R_0=1.2 NN=6 MM=12}  REFERENCE7=0.990764000 WEIGHT7=1. 
ATOMS8=5,cys158      SWITCH8={RATIONAL R_0=1.2 NN=6 MM=10}  REFERENCE8=0.636723000 WEIGHT8=1. 
ATOMS9=thr169,ring   SWITCH9={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE9=0.498470000 WEIGHT9=1.
LABEL=cm8                                                              
CMDIST                                                                 
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t_m_a_p.html">CONTACTMAP</a>                                                         
                                                                       
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t_m_a_p.html">CONTACTMAP</a> ...                                                         
ATOMS1=5,ring244     SWITCH1={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE1=0.216448000 WEIGHT1=0.333 
ATOMS2=5,ring221     SWITCH2={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE2=0.239333000 WEIGHT2=0.333 
ATOMS3=5,ring86      SWITCH3={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE3=0.182106000 WEIGHT3=0.333 
ATOMS4=5,oxy85       SWITCH4={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE4=0.169182000 WEIGHT4=1. 
ATOMS5=trp218,ring   SWITCH5={RATIONAL R_0=1.0 NN=6 MM=12}  REFERENCE5=0.008046000 WEIGHT5=1. 
ATOMS6=val93,ring    SWITCH6={RATIONAL R_0=1.0 NN=6 MM=12}  REFERENCE6=0.003324000 WEIGHT6=1. 
ATOMS7=ile160,ring   SWITCH7={RATIONAL R_0=1.2 NN=6 MM=12}  REFERENCE7=0.674940000 WEIGHT7=1. 
ATOMS8=5,cys158      SWITCH8={RATIONAL R_0=1.2 NN=6 MM=10}  REFERENCE8=0.784664000 WEIGHT8=1. 
ATOMS9=thr169,ring   SWITCH9={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE9=0.083936000 WEIGHT9=1.
LABEL=cm9                                                              
CMDIST                                                                 
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t_m_a_p.html">CONTACTMAP</a>                                                         
                                                                       
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t_m_a_p.html">CONTACTMAP</a> ...                                                         
ATOMS1=5,ring244     SWITCH1={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE1=0.044800000 WEIGHT1=0.333 
ATOMS2=5,ring221     SWITCH2={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE2=0.032370000 WEIGHT2=0.333 
ATOMS3=5,ring86      SWITCH3={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE3=0.022490000 WEIGHT3=0.333 
ATOMS4=5,oxy85       SWITCH4={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE4=0.041785000 WEIGHT4=1. 
ATOMS5=trp218,ring   SWITCH5={RATIONAL R_0=1.0 NN=6 MM=12}  REFERENCE5=0.001275000 WEIGHT5=1. 
ATOMS6=val93,ring    SWITCH6={RATIONAL R_0=1.0 NN=6 MM=12}  REFERENCE6=0.000763000 WEIGHT6=1. 
ATOMS7=ile160,ring   SWITCH7={RATIONAL R_0=1.2 NN=6 MM=12}  REFERENCE7=0.067223000 WEIGHT7=1. 
ATOMS8=5,cys158      SWITCH8={RATIONAL R_0=1.2 NN=6 MM=10}  REFERENCE8=0.764340000 WEIGHT8=1. 
ATOMS9=thr169,ring   SWITCH9={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE9=0.031289000 WEIGHT9=1.
LABEL=cm10                                                             
CMDIST                                                                 
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t_m_a_p.html">CONTACTMAP</a>                                                         
                                                                       
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t_m_a_p.html">CONTACTMAP</a> ...                                                         
ATOMS1=5,ring244     SWITCH1={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE1=0.010987000 WEIGHT1=0.333 
ATOMS2=5,ring221     SWITCH2={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE2=0.010682000 WEIGHT2=0.333 
ATOMS3=5,ring86      SWITCH3={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE3=0.007535000 WEIGHT3=0.333 
ATOMS4=5,oxy85       SWITCH4={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE4=0.013361000 WEIGHT4=1. 
ATOMS5=trp218,ring   SWITCH5={RATIONAL R_0=1.0 NN=6 MM=12}  REFERENCE5=0.000552000 WEIGHT5=1. 
ATOMS6=val93,ring    SWITCH6={RATIONAL R_0=1.0 NN=6 MM=12}  REFERENCE6=0.000381000 WEIGHT6=1. 
ATOMS7=ile160,ring   SWITCH7={RATIONAL R_0=1.2 NN=6 MM=12}  REFERENCE7=0.024819000 WEIGHT7=1. 
ATOMS8=5,cys158      SWITCH8={RATIONAL R_0=1.2 NN=6 MM=10}  REFERENCE8=0.413170000 WEIGHT8=1. 
ATOMS9=thr169,ring   SWITCH9={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE9=0.018060000 WEIGHT9=1.
LABEL=cm11                                                             
CMDIST                                                                 
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t_m_a_p.html">CONTACTMAP</a>                                                         
                                                                       
<a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t_m_a_p.html">CONTACTMAP</a> ...                                                         
ATOMS1=5,ring244     SWITCH1={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE1=0.000000000 WEIGHT1=0.333 
ATOMS2=5,ring221     SWITCH2={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE2=0.000000000 WEIGHT2=0.333 
ATOMS3=5,ring86      SWITCH3={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE3=0.000000000 WEIGHT3=0.333 
ATOMS4=5,oxy85       SWITCH4={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE4=0.000000000 WEIGHT4=1. 
ATOMS5=trp218,ring   SWITCH5={RATIONAL R_0=1.0 NN=6 MM=12}  REFERENCE5=0.000000000 WEIGHT5=1. 
ATOMS6=val93,ring    SWITCH6={RATIONAL R_0=1.0 NN=6 MM=12}  REFERENCE6=0.000000000 WEIGHT6=1. 
ATOMS7=ile160,ring   SWITCH7={RATIONAL R_0=1.2 NN=6 MM=12}  REFERENCE7=0.000000000 WEIGHT7=1. 
ATOMS8=5,cys158      SWITCH8={RATIONAL R_0=1.2 NN=6 MM=10}  REFERENCE8=0.000000000 WEIGHT8=1. 
ATOMS9=thr169,ring   SWITCH9={RATIONAL R_0=0.8 NN=6 MM=10}  REFERENCE9=0.000000000 WEIGHT9=1.
LABEL=cm12                                                             
CMDIST                                                                 
... <a href="https://plumed.github.io/doc-master/user-doc/html/_c_o_n_t_a_c_t_m_a_p.html">CONTACTMAP</a>                                                         
      
<span style="color:blue"># Definition of the pathCV                                                                                                                        </span>
p1: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_u_n_c_p_a_t_h_m_s_d.html">FUNCPATHMSD</a> ARG=cm1,cm2,cm3,cm4,cm5,cm6,cm7,cm8,cm9,cm10,cm11,cm12 LAMBDA=9.778314

<span style="color:blue"># Restraining to maintain the ligand on the pathway I</span>
ort_up: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=p1.z AT=0.23 KAPPA=50000.
ort_down: <a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=p1.z AT=-0.2 KAPPA=1000.

<span style="color:blue"># Frequency-Adaptive Metadynamics</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ...
ARG=p1.s,p1.z
GRID_MIN=1.,-0.2
GRID_MAX=12.,0.4
HEIGHT=2
SIGMA=0.05,0.01
BIASFACTOR=20
LABEL=metad
TEMP=300.
CALC_RCT
ACCELERATION
FREQUENCY_ADAPTIVE
PACE=500 
FA_MAX_PACE=50000 
FA_UPDATE_FREQUENCY=5000
FA_MIN_ACCELERATION=1e2 
... <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a>


<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=p1.* FILE=path.dat STRIDE=500
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=metad.* FILE=metad_data.dat STRIDE=500 
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=d1.z FILE=distance_pocket.dat STRIDE=500
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=ort_up.*,ort_down.* FILE=barriers.dat STRIDE=500

<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=500 

<a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_d_p_l_u_m_e_d.html">ENDPLUMED</a>
<span style="color:blue"></span>
<span style="color:blue"></span>
</pre>{% endraw %}
