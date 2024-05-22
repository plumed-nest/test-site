**Project ID:** [plumID:22.036]({{ '/' | absolute_url }}eggs/22/036/)  
Stderr for source:  plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
In file included from /home/runner/opt/include/plumed/colvar/../core/../tools/Keywords.h:29,
from /home/runner/opt/include/plumed/colvar/../core/Action.h:27,
from /home/runner/opt/include/plumed/colvar/../core/ActionAtomistic.h:25,
from /home/runner/opt/include/plumed/colvar/../core/Colvar.h:25,
from /home/runner/opt/include/plumed/colvar/Colvar.h:24,
from /home/runner/opt/include/plumed/colvar/CoordinationBase.h:24,
from ./GHBFIX.cpp:22:
./GHBFIX.cpp: In constructor ‘PLMD::colvar::GHBFIX::GHBFIX(const PLMD::ActionOptions&)’:
./GHBFIX.cpp:140:23: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
140 |       plumed_assert(it<n)<<"itype ="<<it<<", should be smaller than "<<n;
|                     ~~^~
/home/runner/opt/include/plumed/colvar/../core/../tools/Exception.h:373:34: note: in definition of macro ‘plumed_assert’
373 | #define plumed_assert(test) if(!(test)) plumed_error() << PLMD::Exception::Assertion(#test)
|                                  ^~~~
./GHBFIX.cpp:141:23: warning: comparison of integer expressions of different signedness: ‘int’ and ‘unsigned int’ [-Wsign-compare]
141 |       plumed_assert(jt<n)<<"jtype ="<<jt<<", should be smaller than "<<n;
|                     ~~^~
/home/runner/opt/include/plumed/colvar/../core/../tools/Exception.h:373:34: note: in definition of macro ‘plumed_assert’
373 | #define plumed_assert(test) if(!(test)) plumed_error() << PLMD::Exception::Assertion(#test)
|                                  ^~~~
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: GHBFIX LABEL=group_1 PAIR GROUPA=20,18,494,492,1036,1034,1503,1505,1508,240,242,244,274,272,1252,1254,1257,1288,1286 GROUPB=1007,1005,1540,1538,2017,2015,523,525,527,779,781,784,1760,1758,1790,1792,1794,752,750 D_0=0.23 D_MAX=0.33 C=0.8 TYPES=typesTable.dat PARAMS=scalingParameters.dat
Maybe a missing space or a typo?
[fv-az1106-239:40297] *** Process received signal ***
[fv-az1106-239:40297] Signal: Aborted (6)
[fv-az1106-239:40297] Signal code:  (-6)
[fv-az1106-239:40297] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fd6b7c42520]
[fv-az1106-239:40297] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fd6b7c969fc]
[fv-az1106-239:40297] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fd6b7c42476]
[fv-az1106-239:40297] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fd6b7c287f3]
[fv-az1106-239:40297] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fd6b80a2b9e]
[fv-az1106-239:40297] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fd6b80ae20c]
[fv-az1106-239:40297] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fd6b80ae277]
[fv-az1106-239:40297] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fd6b80ae52b]
[fv-az1106-239:40297] [ 8] plumed(+0x12f48)[0x55b9a4695f48]
[fv-az1106-239:40297] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fd6b7c29d90]
[fv-az1106-239:40297] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fd6b7c29e40]
[fv-az1106-239:40297] [11] plumed(+0x131e5)[0x55b9a46961e5]
[fv-az1106-239:40297] *** End of error message ***
</pre>
{% endraw %}
