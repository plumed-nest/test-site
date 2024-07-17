**Project ID:** [plumID:23.027]({{ '/' | absolute_url }}eggs/23/027/)  
Stderr for source:  plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
Cmumd.cpp: In member function ‘virtual void PLMD::colvar::Cmumd::calculate()’:
Cmumd.cpp:494:17: warning: ‘w_out’ may be used uninitialized in this function [-Wmaybe-uninitialized]
494 |             zout=(com_solv[i][2]-ZCRlout)/w_out;
|             ~~~~^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Cmumd.cpp:493:16: warning: ‘w_in’ may be used uninitialized in this function [-Wmaybe-uninitialized]
493 |             zin=(com_solv[i][2]-ZCRlin)/w_in;
|             ~~~^~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Cmumd.cpp:515:46: warning: ‘w_force’ may be used uninitialized in this function [-Wmaybe-uninitialized]
515 |             dr=(-dsig(zr,co_f)-dsig(zr+LBC[2]/w_force,co_f))/w_force;
|                                        ~~~~~~^~~~~~~~
Cmumd.cpp:458:14: warning: ‘D_F’ may be used uninitialized in this function [-Wmaybe-uninitialized]
458 |       ZFright=zright+D_F;
|       ~~~~~~~^~~~~~~~~~~
Cmumd.cpp:457:14: warning: ‘CR_Size’ may be used uninitialized in this function [-Wmaybe-uninitialized]
457 |       ZCRrout=zright+D_CR+CR_Size;
|       ~~~~~~~^~~~~~~~~~~~~~~~~~~~
Cmumd.cpp:456:13: warning: ‘D_CR’ may be used uninitialized in this function [-Wmaybe-uninitialized]
456 |       ZCRrin=zright+D_CR;
|       ~~~~~~^~~~~~~~~~~~
</pre>
{% endraw %}
