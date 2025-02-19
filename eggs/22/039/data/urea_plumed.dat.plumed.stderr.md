**Project ID:** [plumID:22.039]({{ '/' | absolute_url }}eggs/22/039/)  
Stderr for source:  urea_plumed.dat   
Download: [zipped raw stdout](urea_plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](urea_plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: using a legacy ActionRegister.h include path, please use <<#include "core/ActionRegister.h">>
PairEntropy.uYXvZa.cpp: In member function ‘virtual void PLMD::colvar::PairEntropy::calculate()’:
PairEntropy.uYXvZa.cpp:264:21: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
264 |          if (minBin > (nhist-1)) minBin=nhist-1;
|              ~~~~~~~^~~~~~~~~~~
PairEntropy.uYXvZa.cpp:266:21: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
266 |          if (maxBin > (nhist-1)) maxBin=nhist-1;
|              ~~~~~~~^~~~~~~~~~~
WARNING: using a legacy ActionRegister.h include path, please use <<#include "core/ActionRegister.h">>
ManyAngle.LyPmRm.cpp: In constructor ‘PLMD::colvar::ManyAngle::ManyAngle(const PLMD::ActionOptions&)’:
ManyAngle.LyPmRm.cpp:68:27: warning: ‘PLMD::colvar::ManyAngle::moment2’ will be initialized after [-Wreorder]
68 |   bool pbc, serial, mean, moment2;
|                           ^~~~~~~
ManyAngle.LyPmRm.cpp:68:13: warning:   ‘bool PLMD::colvar::ManyAngle::serial’ [-Wreorder]
68 |   bool pbc, serial, mean, moment2;
|             ^~~~~~
ManyAngle.LyPmRm.cpp:100:1: warning:   when initialized here [-Wreorder]
100 | ManyAngle::ManyAngle(const ActionOptions&ao):
| ^~~~~~~~~
ManyAngle.LyPmRm.cpp:124:3: warning: this ‘if’ clause does not guard... [-Wmisleading-indentation]
124 |   if(mean) addComponentWithDerivatives("mean"); componentIsNotPeriodic("mean"); moments[0]=getPntrToComponent("mean"); // (Z)
|   ^~
ManyAngle.LyPmRm.cpp:124:49: note: ...this statement, but the latter is misleadingly indented as if it were guarded by the ‘if’
124 |   if(mean) addComponentWithDerivatives("mean"); componentIsNotPeriodic("mean"); moments[0]=getPntrToComponent("mean"); // (Z)
|                                                 ^~~~~~~~~~~~~~~~~~~~~~
ManyAngle.LyPmRm.cpp:125:3: warning: this ‘if’ clause does not guard... [-Wmisleading-indentation]
125 |   if(moment2) addComponentWithDerivatives("moment2"); componentIsNotPeriodic("moment2"); moments[1]=getPntrToComponent("moment2"); // (Z)
|   ^~
ManyAngle.LyPmRm.cpp:125:55: note: ...this statement, but the latter is misleadingly indented as if it were guarded by the ‘if’
125 |   if(moment2) addComponentWithDerivatives("moment2"); componentIsNotPeriodic("moment2"); moments[1]=getPntrToComponent("moment2"); // (Z)
|                                                       ^~~~~~~~~~~~~~~~~~~~~~
</pre>
{% endraw %}
