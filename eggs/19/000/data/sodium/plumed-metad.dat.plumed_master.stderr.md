**Project ID:** [plumID:19.000]({{ '/' | absolute_url }}eggs/19/000/)  
Stderr for source:  sodium/plumed-metad.dat   
Download: [zipped raw stdout](plumed-metad.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed-metad.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: using a legacy ActionRegister.h include path, please use <<#include "core/ActionRegister.h">>
DebyeStructureFactor.kdmMdw.cpp: In static member function ‘static void PLMD::colvar::DebyeStructureFactor::registerKeywords(PLMD::Keywords&)’:
DebyeStructureFactor.kdmMdw.cpp:138:26: warning: ‘void PLMD::Keywords::addOutputComponent(const std::string&, const std::string&, const std::string&)’ is deprecated: Use addOutputComponent with four argument and specify valid types for value from scalar/vector/matrix/grid [-Wdeprecated-declarations]
138 |   keys.addOutputComponent("ds","default","the instantaneous Debye Structure Factor at a given frequency q (or angle 2theta)");
|   ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
In file included from /home/runner/opt/include/plumed_master/colvar/../core/Action.h:27,
from /home/runner/opt/include/plumed_master/colvar/../core/ActionAtomistic.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/Colvar.h:25,
from /home/runner/opt/include/plumed_master/colvar/Colvar.h:24,
from DebyeStructureFactor.kdmMdw.cpp:22:
/home/runner/opt/include/plumed_master/colvar/../core/../tools/Keywords.h:256:8: note: declared here
256 |   void addOutputComponent( const std::string& name, const std::string& key, const std::string& descr );
|        ^~~~~~~~~~~~~~~~~~
DebyeStructureFactor.kdmMdw.cpp: In constructor ‘PLMD::colvar::DebyeStructureFactor::DebyeStructureFactor(const PLMD::ActionOptions&)’:
DebyeStructureFactor.kdmMdw.cpp:287:41: warning: ‘int PLMD::PlumedMain::DeprecatedAtoms::getNatoms() const’ is deprecated [-Wdeprecated-declarations]
287 |     NumAtom_=plumed.getAtoms().getNatoms();
|              ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~
In file included from DebyeStructureFactor.kdmMdw.cpp:24:
/home/runner/opt/include/plumed_master/core/PlumedMain.h:106:9: note: declared here
106 |     int getNatoms() const ;
|         ^~~~~~~~~
DebyeStructureFactor.kdmMdw.cpp:341:108: warning: ‘int PLMD::PlumedMain::DeprecatedAtoms::getNatoms() const’ is deprecated [-Wdeprecated-declarations]
341 |   log.printf("  over a total of N_tot=%d, considering a number of atoms N=%d\n",plumed.getAtoms().getNatoms(),NumAtom_);
|                                                                                 ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~
/home/runner/opt/include/plumed_master/core/PlumedMain.h:106:9: note: declared here
106 |     int getNatoms() const ;
|         ^~~~~~~~~
DebyeStructureFactor.kdmMdw.cpp: In member function ‘virtual void PLMD::colvar::DebyeStructureFactor::calculate()’:
DebyeStructureFactor.kdmMdw.cpp:489:25: warning: ‘base_cos’ may be used uninitialized [-Wmaybe-uninitialized]
489 |           cosQR=base_cos*prev_cos-base_sin*prev_sin;
|                 ~~~~~~~~^~~~~~~~~
DebyeStructureFactor.kdmMdw.cpp:471:14: note: ‘base_cos’ was declared here
471 |       double base_cos; //this throws a warning, but is correct (and faster)
|              ^~~~~~~~
DebyeStructureFactor.kdmMdw.cpp:489:43: warning: ‘base_sin’ may be used uninitialized [-Wmaybe-uninitialized]
489 |           cosQR=base_cos*prev_cos-base_sin*prev_sin;
|                                   ~~~~~~~~^~~~~~~~~
DebyeStructureFactor.kdmMdw.cpp:472:14: note: ‘base_sin’ was declared here
472 |       double base_sin;
|              ^~~~~~~~
DebyeStructureFactor.kdmMdw.cpp:489:25: warning: ‘prev_cos’ may be used uninitialized [-Wmaybe-uninitialized]
489 |           cosQR=base_cos*prev_cos-base_sin*prev_sin;
|                 ~~~~~~~~^~~~~~~~~
DebyeStructureFactor.kdmMdw.cpp:473:14: note: ‘prev_cos’ was declared here
473 |       double prev_cos;
|              ^~~~~~~~
DebyeStructureFactor.kdmMdw.cpp:489:43: warning: ‘prev_sin’ may be used uninitialized [-Wmaybe-uninitialized]
489 |           cosQR=base_cos*prev_cos-base_sin*prev_sin;
|                                   ~~~~~~~~^~~~~~~~~
DebyeStructureFactor.kdmMdw.cpp:474:14: note: ‘prev_sin’ was declared here
474 |       double prev_sin;
|              ^~~~~~~~
</pre>
{% endraw %}
