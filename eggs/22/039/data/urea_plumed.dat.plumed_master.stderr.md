**Project ID:** [plumID:22.039]({{ '/' | absolute_url }}eggs/22/039/)  
Stderr for source:  urea_plumed.dat   
Download: [zipped raw stdout](urea_plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](urea_plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: using a legacy ActionRegister.h include path, please use <<#include "core/ActionRegister.h">>
PairEntropy.FsgYTI.cpp: In member function ‘virtual void PLMD::colvar::PairEntropy::calculate()’:
PairEntropy.FsgYTI.cpp:264:21: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
264 |          if (minBin > (nhist-1)) minBin=nhist-1;
|              ~~~~~~~^~~~~~~~~~~
PairEntropy.FsgYTI.cpp:266:21: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
266 |          if (maxBin > (nhist-1)) maxBin=nhist-1;
|              ~~~~~~~^~~~~~~~~~~
WARNING: using a legacy ActionRegister.h include path, please use <<#include "core/ActionRegister.h">>
ManyAngle.ZR9AH8.cpp: In static member function ‘static void PLMD::colvar::ManyAngle::registerKeywords(PLMD::Keywords&)’:
ManyAngle.ZR9AH8.cpp:96:26: warning: ‘void PLMD::Keywords::addOutputComponent(const std::string&, const std::string&, const std::string&)’ is deprecated: Use addOutputComponent with four argument and specify valid types for value from scalar/vector/matrix/grid [-Wdeprecated-declarations]
96 |   keys.addOutputComponent("mean","default","Return the 1st moment of angle variable"); //(Z)
|   ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
In file included from /home/runner/opt/include/plumed_master/colvar/../core/Action.h:27,
from /home/runner/opt/include/plumed_master/colvar/../core/ActionAtomistic.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/Colvar.h:25,
from /home/runner/opt/include/plumed_master/colvar/Colvar.h:24,
from ManyAngle.ZR9AH8.cpp:22:
/home/runner/opt/include/plumed_master/colvar/../core/../tools/Keywords.h:256:8: note: declared here
256 |   void addOutputComponent( const std::string& name, const std::string& key, const std::string& descr );
|        ^~~~~~~~~~~~~~~~~~
ManyAngle.ZR9AH8.cpp:97:26: warning: ‘void PLMD::Keywords::addOutputComponent(const std::string&, const std::string&, const std::string&)’ is deprecated: Use addOutputComponent with four argument and specify valid types for value from scalar/vector/matrix/grid [-Wdeprecated-declarations]
97 |   keys.addOutputComponent("moment2","default","Return the 2nd moment of angle variable"); //(Z)
|   ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/home/runner/opt/include/plumed_master/colvar/../core/../tools/Keywords.h:256:8: note: declared here
256 |   void addOutputComponent( const std::string& name, const std::string& key, const std::string& descr );
|        ^~~~~~~~~~~~~~~~~~
ManyAngle.ZR9AH8.cpp: In constructor ‘PLMD::colvar::ManyAngle::ManyAngle(const PLMD::ActionOptions&)’:
ManyAngle.ZR9AH8.cpp:68:27: warning: ‘PLMD::colvar::ManyAngle::moment2’ will be initialized after [-Wreorder]
68 |   bool pbc, serial, mean, moment2;
|                           ^~~~~~~
ManyAngle.ZR9AH8.cpp:68:13: warning:   ‘bool PLMD::colvar::ManyAngle::serial’ [-Wreorder]
68 |   bool pbc, serial, mean, moment2;
|             ^~~~~~
ManyAngle.ZR9AH8.cpp:100:1: warning:   when initialized here [-Wreorder]
100 | ManyAngle::ManyAngle(const ActionOptions&ao):
| ^~~~~~~~~
ManyAngle.ZR9AH8.cpp:124:3: warning: this ‘if’ clause does not guard... [-Wmisleading-indentation]
124 |   if(mean) addComponentWithDerivatives("mean"); componentIsNotPeriodic("mean"); moments[0]=getPntrToComponent("mean"); // (Z)
|   ^~
ManyAngle.ZR9AH8.cpp:124:49: note: ...this statement, but the latter is misleadingly indented as if it were guarded by the ‘if’
124 |   if(mean) addComponentWithDerivatives("mean"); componentIsNotPeriodic("mean"); moments[0]=getPntrToComponent("mean"); // (Z)
|                                                 ^~~~~~~~~~~~~~~~~~~~~~
ManyAngle.ZR9AH8.cpp:125:3: warning: this ‘if’ clause does not guard... [-Wmisleading-indentation]
125 |   if(moment2) addComponentWithDerivatives("moment2"); componentIsNotPeriodic("moment2"); moments[1]=getPntrToComponent("moment2"); // (Z)
|   ^~
ManyAngle.ZR9AH8.cpp:125:55: note: ...this statement, but the latter is misleadingly indented as if it were guarded by the ‘if’
125 |   if(moment2) addComponentWithDerivatives("moment2"); componentIsNotPeriodic("moment2"); moments[1]=getPntrToComponent("moment2"); // (Z)
|                                                       ^~~~~~~~~~~~~~~~~~~~~~
</pre>
{% endraw %}
