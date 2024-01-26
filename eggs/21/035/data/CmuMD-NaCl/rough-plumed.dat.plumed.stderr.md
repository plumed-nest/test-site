**Project ID:** [plumID:21.035]({{ '/' | absolute_url }}eggs/21/035/)  
Stderr for source:  CmuMD-NaCl/rough-plumed.dat   
Download: [zipped raw stdout](rough-plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](rough-plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
Cmumd.cpp: In member function ‘virtual void PLMD::colvar::CmuMD::calculate()’:
Cmumd.cpp:482:17: warning: ‘w_out’ may be used uninitialized in this function [-Wmaybe-uninitialized]
482 |             zout=(com_solv[i][2]-ZCRlout)/w_out;
|             ~~~~^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Cmumd.cpp:481:16: warning: ‘w_in’ may be used uninitialized in this function [-Wmaybe-uninitialized]
481 |             zin=(com_solv[i][2]-ZCRlin)/w_in;
|             ~~~^~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Cmumd.cpp:499:46: warning: ‘w_force’ may be used uninitialized in this function [-Wmaybe-uninitialized]
499 |             dr=(-dsig(zr,co_f)-dsig(zr+LBC[2]/w_force,co_f))/w_force;
|                                        ~~~~~~^~~~~~~~
Cmumd.cpp:449:14: warning: ‘D_F’ may be used uninitialized in this function [-Wmaybe-uninitialized]
449 |       ZFright=zright+D_F;
|       ~~~~~~~^~~~~~~~~~~
Cmumd.cpp:348:12: warning: ‘CR_Size’ may be used uninitialized in this function [-Wmaybe-uninitialized]
348 |         VCR=LBC[0]*LBC[1]*CR_Size; //CR volume
|         ~~~^~~~~~~~~~~~~~~~~~~~~~
Cmumd.cpp:447:13: warning: ‘D_CR’ may be used uninitialized in this function [-Wmaybe-uninitialized]
447 |       ZCRrin=zright+D_CR;
|       ~~~~~~^~~~~~~~~~~~
</pre>
{% endraw %}
