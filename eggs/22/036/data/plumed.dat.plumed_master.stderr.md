**Project ID:** [plumID:22.036]({{ '/' | absolute_url }}eggs/22/036/)  
Stderr for source:  plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: using a legacy ActionRegister.h include path, please use <<#include "core/ActionRegister.h">>
WARNING: "core/Atoms.h" does not exist anymore in  version >=2.10, you should change your code.
In file included from /home/runner/opt/include/plumed_master/colvar/../core/../tools/Keywords.h:29,
from /home/runner/opt/include/plumed_master/colvar/../core/Action.h:27,
from /home/runner/opt/include/plumed_master/colvar/../core/ActionAtomistic.h:25,
from /home/runner/opt/include/plumed_master/colvar/../core/Colvar.h:25,
from /home/runner/opt/include/plumed_master/colvar/Colvar.h:24,
from /home/runner/opt/include/plumed_master/colvar/CoordinationBase.h:24,
from ./GHBFIX.D6Dt1H.cpp:22:
./GHBFIX.D6Dt1H.cpp: In constructor ‘PLMD::colvar::GHBFIX::GHBFIX(const PLMD::ActionOptions&)’:
./GHBFIX.D6Dt1H.cpp:139:23: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
139 |       plumed_assert(it<n)<<"itype ="<<it<<", should be smaller than "<<n;
|                     ~~^~
/home/runner/opt/include/plumed_master/colvar/../core/../tools/Exception.h:373:34: note: in definition of macro ‘plumed_assert’
373 | #define plumed_assert(test) if(!(test)) plumed_error() << PLMD::Exception::Assertion(#test)
|                                  ^~~~
./GHBFIX.D6Dt1H.cpp:140:23: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
140 |       plumed_assert(jt<n)<<"jtype ="<<jt<<", should be smaller than "<<n;
|                     ~~^~
/home/runner/opt/include/plumed_master/colvar/../core/../tools/Exception.h:373:34: note: in definition of macro ‘plumed_assert’
373 | #define plumed_assert(test) if(!(test)) plumed_error() << PLMD::Exception::Assertion(#test)
|                                  ^~~~
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label metad : The GRID file you want to read: GRID, cannot be found!
[fv-az774-16:70757] *** Process received signal ***
[fv-az774-16:70757] Signal: Aborted (6)
[fv-az774-16:70757] Signal code:  (-6)
[fv-az774-16:70757] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f1809e42520]
[fv-az774-16:70757] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f1809e969fc]
[fv-az774-16:70757] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f1809e42476]
[fv-az774-16:70757] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f1809e287f3]
[fv-az774-16:70757] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f180a2a2b9e]
[fv-az774-16:70757] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f180a2ae20c]
[fv-az774-16:70757] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f180a2ae277]
[fv-az774-16:70757] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f180a2ae52b]
[fv-az774-16:70757] [ 8] plumed_master(+0x14274)[0x56449fb82274]
[fv-az774-16:70757] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f1809e29d90]
[fv-az774-16:70757] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f1809e29e40]
[fv-az774-16:70757] [11] plumed_master(+0x14ed5)[0x56449fb82ed5]
[fv-az774-16:70757] *** End of error message ***
</pre>
{% endraw %}