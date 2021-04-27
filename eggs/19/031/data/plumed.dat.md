**Project ID:** [plumID:19.031]({{ '/' | absolute_url }}eggs/19/031/)  
**Source:** plumed.dat  
**Originally used with PLUMED version:** 2.5-dev  
**Stable:** [raw zipped stdout](plumed.dat.plumed.stdout.txt.zip) - [stderr](plumed.dat.plumed.stderr)  
**Master:** [raw zipped stdout](plumed.dat.plumed_master.stdout.txt.zip) - [stderr](plumed.dat.plumed_master.stderr)  

{% raw %}<pre>
<span style="color:blue"># -----------------------------------------------------------------------------------------</span>
<span style="color:blue"># Input file for ice nucleation from the liquid, employed with the TIP4P/2005 water model.</span>
<span style="color:blue"># -----------------------------------------------------------------------------------------</span>
<span style="color:blue"># For details about the PIV-based path collective variables, and about</span>
<span style="color:blue"># this input file for ice nucleation, please read:</span>
<span style="color:blue">#   Phys. Rev. Lett. 119, 245701 (2017) https://doi.org/10.1103/PhysRevLett.119.245701</span>
<span style="color:blue">#   http://arxiv.org/abs/1703.00753</span>
<span style="color:blue"># More info about the CV syntax is given by the plumed documentation.</span>
<span style="color:blue"># </span>
<span style="color:blue"># Here below, we consider only O-O and H-H distances ("ONLYDIRECT"),</span>
<span style="color:blue"># we apply the same switching function to both cases ("SWITCH1/2"), </span>
<span style="color:blue"># we specify a reference volume in nm^3 ("VOLUME"),</span>
<span style="color:blue"># we weigh differently O-O and H-H pairs ("SFACTOR"),</span>
<span style="color:blue"># and we set the neighbor list parameters (note that neighbor list must</span>
<span style="color:blue"># be defined, even in cases like small ab initio boxes where they are not necessary).</span>
<span style="color:blue">#</span>
<span style="color:blue"># Note that pdb reference files must follow strictly the official pdb format </span>
<span style="color:blue"># (see the two examples included), with atoms in the same order as in the MD input file,</span>
<span style="color:blue"># and without any jump in atom index.</span>

<span style="color:blue"># definition of PIV distance from the first reference structure:</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_i_v.html">PIV</a> ...
LABEL=c1
REF_FILE=Liq.pdb
VOLUME=25.1264
ONLYDIRECT
PIVATOMS=2
ATOMTYPES=OW1,HW
SORT=1,1
SFACTOR=1.,0.2
SWITCH1={RATIONAL R_0=0.7 MM=12 NN=4}
SWITCH2={RATIONAL R_0=0.7 MM=12 NN=4}
PRECISION=1000
NLIST
NL_CUTOFF=1.2,1.2
NL_STRIDE=10,10
NL_SKIN=0.1,0.1
... <a href="https://plumed.github.io/doc-master/user-doc/html/_p_i_v.html">PIV</a>

<span style="color:blue"># definition of PIV distance from the second reference structure:</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_i_v.html">PIV</a> ...
LABEL=c2
REF_FILE=Ice.pdb
VOLUME=25.1264
ONLYDIRECT
PIVATOMS=2
ATOMTYPES=OW1,HW
SORT=1,1
SFACTOR=1.,0.2
SWITCH1={RATIONAL R_0=0.7 MM=12 NN=4}
SWITCH2={RATIONAL R_0=0.7 MM=12 NN=4}
PRECISION=1000
NLIST
NL_CUTOFF=1.2,1.2
NL_STRIDE=10,10
NL_SKIN=0.1,0.1
... <a href="https://plumed.github.io/doc-master/user-doc/html/_p_i_v.html">PIV</a>

<span style="color:blue"># when simulating transitions from liquids, it can be useful to apply walls</span>
<span style="color:blue">#  preventing excessive box deformations:</span>

cell: <a href="https://plumed.github.io/doc-master/user-doc/html/_c_e_l_l.html">CELL</a>

<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=cell.ax AT=2.00  KAPPA=800.0 LABEL=lax
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=cell.by AT=2.00  KAPPA=800.0 LABEL=lbx
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=cell.cz AT=2.00  KAPPA=800.0 LABEL=lcx
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=cell.ax AT=4.00  KAPPA=800.0 LABEL=uax
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=cell.by AT=4.00  KAPPA=800.0 LABEL=ubx
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=cell.cz AT=4.00  KAPPA=800.0 LABEL=ucx

<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=cell.ay AT=-0.6  KAPPA=200.0 LABEL=lay
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=cell.ay  AT=0.6  KAPPA=200.0 LABEL=uay
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=cell.az AT=-0.6  KAPPA=200.0 LABEL=laz
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=cell.az  AT=0.6  KAPPA=200.0 LABEL=uaz

<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=cell.bx AT=-0.6  KAPPA=200.0 LABEL=lby
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=cell.bx  AT=0.6  KAPPA=200.0 LABEL=uby
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=cell.bz AT=-0.6  KAPPA=200.0 LABEL=lbz
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=cell.bz  AT=0.6  KAPPA=200.0 LABEL=ubz

<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=cell.cx AT=-0.6  KAPPA=200.0 LABEL=lcy
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=cell.cx  AT=0.6  KAPPA=200.0 LABEL=ucy
<a href="https://plumed.github.io/doc-master/user-doc/html/_l_o_w_e_r__w_a_l_l_s.html">LOWER_WALLS</a> ARG=cell.cy AT=-0.6  KAPPA=200.0 LABEL=lcz
<a href="https://plumed.github.io/doc-master/user-doc/html/_u_p_p_e_r__w_a_l_l_s.html">UPPER_WALLS</a> ARG=cell.cy  AT=0.6  KAPPA=200.0 LABEL=ucz

<span style="color:blue"># definition of the path collective variables based on PIV distances c1 and c2</span>
<span style="color:blue">#  ( as customary with path CVs, lambda * dist(ref1,ref2) = 2.3, where dist is the PIV distance,</span>
<span style="color:blue">#  which results in ref1 being located at p1.s=1.1 and ref2 at p1.s=1.9 )</span>

p1: <a href="https://plumed.github.io/doc-master/user-doc/html/_f_u_n_c_p_a_t_h_m_s_d.html">FUNCPATHMSD</a> ARG=c1,c2 LAMBDA=0.0379017

<span style="color:blue"># metadynamics on the two path CVs:</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_m_e_t_a_d.html">METAD</a> ARG=p1.s,p1.z SIGMA=0.02,0.4 HEIGHT=1.5 PACE=500 LABEL=res

<span style="color:blue"># some output:</span>

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=c1,c2,p1.s,p1.z,res.bias STRIDE=500  FILE=colvar FMT=%15.6f

<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=lax.bias,lbx.bias,lcx.bias,uax.bias,ubx.bias,ucx.bias,lay.bias,uay.bias,laz.bias,uaz.bias,lby.bias,uby.bias,lbz.bias,ubz.bias,lcy.bias,ucy.bias,lcz.bias,ucz.bias STRIDE=500  FILE=cell_bias FMT=%15.6f
</pre>{% endraw %}
