**Project ID:** [plumID:19.032]({{ '/' | absolute_url }}eggs/19/032/)  
**Source:** plumed.dat  
**Originally used with PLUMED version:** 2.4  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue">#</span>
<span style="color:blue"># example of input: metadynamics simulation connecting formamide with CO+NH3</span>
<span style="color:blue"># units are nm and kJ/mol</span>
<span style="color:blue">#</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_r_e_s_t_a_r_t.html">RESTART</a>
<a href="https://plumed.github.io/doc-master/user-doc/html/_f_l_u_s_h.html">FLUSH</a> STRIDE=10

<span style="color:blue"># here below we set a coordination table with 3 rows (O1,C2,N3) and 4 columns (all O,C,N,H)</span>

<span style="color:blue"># the coordination functions are typically chosen so that covalent bond ~0.9, second neighbors < 0.2</span>
<span style="color:blue"># (note that X-X is longer than X-H, with X=O,C,N)</span>

O1O: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=1 GROUPB=1,7-68     LESS_THAN={RATIONAL R_0=0.18 NN=6 MM=12} 
O1C: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=1 GROUPB=2          LESS_THAN={RATIONAL R_0=0.18 NN=6 MM=12} 
O1N: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=1 GROUPB=3          LESS_THAN={RATIONAL R_0=0.18 NN=6 MM=12} 
O1H: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=1 GROUPB=4-6,69-192 LESS_THAN={RATIONAL R_0=0.15 NN=6 MM=12} 

C2O: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=2 GROUPB=1,7-68     LESS_THAN={RATIONAL R_0=0.18 NN=6 MM=12} 
C2C: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=2 GROUPB=2          LESS_THAN={RATIONAL R_0=0.18 NN=6 MM=12} 
C2N: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=2 GROUPB=3          LESS_THAN={RATIONAL R_0=0.18 NN=6 MM=12} 
C2H: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=2 GROUPB=4-6,69-192 LESS_THAN={RATIONAL R_0=0.15 NN=6 MM=12} 

N3O: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=3 GROUPB=1,7-68     LESS_THAN={RATIONAL R_0=0.18 NN=6 MM=12} 
N3C: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=3 GROUPB=2          LESS_THAN={RATIONAL R_0=0.18 NN=6 MM=12} 
N3N: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=3 GROUPB=3          LESS_THAN={RATIONAL R_0=0.18 NN=6 MM=12} 
N3H: <a href="https://plumed.github.io/doc-master/user-doc/html/_d_i_s_t_a_n_c_e_s.html">DISTANCES</a> GROUPA=3 GROUPB=4-6,69-192 LESS_THAN={RATIONAL R_0=0.15 NN=6 MM=12} 

<span style="color:blue"># here below are defined path collective variables s,z based on coordination patterns:</span>
<span style="color:blue"># the switching function is (1-(dist/R_0)**NN)/(1-(dist/R_0)**MM) </span>
<span style="color:blue"># LAMBDA is chosen so that the distance (sum of squares of coord. num. differences) between ref. structures is about 2.3</span>
<span style="color:blue"># the two ref. structures are specified in file path.pdb (more than 2 references can also be used)</span>

pp: <a href="https://plumed.github.io/doc-master/user-doc/html/_p_a_t_h.html">PATH</a> REFERENCE=path.pdb TYPE=EUCLIDEAN LAMBDA=0.78  

<span style="color:blue"># a wall may be used to limit to limit the largest z coordinates explored, as here below</span>

uwall: <a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=pp.zpath AT=0.7 KAPPA=10000.0 EXP=2 

<span style="color:blue"># metadynamics is performed on s,z:</span>

metad: <a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=pp.spath,pp.zpath SIGMA=0.025,0.1 HEIGHT=10 PACE=100 

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=pp.spath,pp.zpath,metad.bias,uwall.bias STRIDE=10 FILE=COLVAR




</pre>{% endraw %}
