**Project ID:** [plumID:19.000]({{ '/' | absolute_url }}eggs/19/000/)  
Stderr for source:  sodium/plumed-metad.dat   
Download: [zipped raw stdout](plumed-metad.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed-metad.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: using a legacy ActionRegister.h include path, please use <<#include "core/ActionRegister.h">>
DebyeStructureFactor.17hRJ2.cpp: In constructor ‘PLMD::colvar::DebyeStructureFactor::DebyeStructureFactor(const PLMD::ActionOptions&)’:
DebyeStructureFactor.17hRJ2.cpp:287:41: warning: ‘int PLMD::PlumedMain::DeprecatedAtoms::getNatoms() const’ is deprecated [-Wdeprecated-declarations]
287 |     NumAtom_=plumed.getAtoms().getNatoms();
|              ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~
In file included from DebyeStructureFactor.17hRJ2.cpp:24:
/home/runner/opt/include/plumed/core/PlumedMain.h:106:9: note: declared here
106 |     int getNatoms() const ;
|         ^~~~~~~~~
DebyeStructureFactor.17hRJ2.cpp:341:108: warning: ‘int PLMD::PlumedMain::DeprecatedAtoms::getNatoms() const’ is deprecated [-Wdeprecated-declarations]
341 |   log.printf("  over a total of N_tot=%d, considering a number of atoms N=%d\n",plumed.getAtoms().getNatoms(),NumAtom_);
|                                                                                 ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~
/home/runner/opt/include/plumed/core/PlumedMain.h:106:9: note: declared here
106 |     int getNatoms() const ;
|         ^~~~~~~~~
DebyeStructureFactor.17hRJ2.cpp: In member function ‘virtual void PLMD::colvar::DebyeStructureFactor::calculate()’:
DebyeStructureFactor.17hRJ2.cpp:489:25: warning: ‘base_cos’ may be used uninitialized [-Wmaybe-uninitialized]
489 |           cosQR=base_cos*prev_cos-base_sin*prev_sin;
|                 ~~~~~~~~^~~~~~~~~
DebyeStructureFactor.17hRJ2.cpp:471:14: note: ‘base_cos’ was declared here
471 |       double base_cos; //this throws a warning, but is correct (and faster)
|              ^~~~~~~~
DebyeStructureFactor.17hRJ2.cpp:489:43: warning: ‘base_sin’ may be used uninitialized [-Wmaybe-uninitialized]
489 |           cosQR=base_cos*prev_cos-base_sin*prev_sin;
|                                   ~~~~~~~~^~~~~~~~~
DebyeStructureFactor.17hRJ2.cpp:472:14: note: ‘base_sin’ was declared here
472 |       double base_sin;
|              ^~~~~~~~
DebyeStructureFactor.17hRJ2.cpp:489:25: warning: ‘prev_cos’ may be used uninitialized [-Wmaybe-uninitialized]
489 |           cosQR=base_cos*prev_cos-base_sin*prev_sin;
|                 ~~~~~~~~^~~~~~~~~
DebyeStructureFactor.17hRJ2.cpp:473:14: note: ‘prev_cos’ was declared here
473 |       double prev_cos;
|              ^~~~~~~~
DebyeStructureFactor.17hRJ2.cpp:489:43: warning: ‘prev_sin’ may be used uninitialized [-Wmaybe-uninitialized]
489 |           cosQR=base_cos*prev_cos-base_sin*prev_sin;
|                                   ~~~~~~~~^~~~~~~~~
DebyeStructureFactor.17hRJ2.cpp:474:14: note: ‘prev_sin’ was declared here
474 |       double prev_sin;
|              ^~~~~~~~
</pre>
{% endraw %}
