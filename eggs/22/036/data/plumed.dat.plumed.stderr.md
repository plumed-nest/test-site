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
[fv-az774-16:70737] *** Process received signal ***
[fv-az774-16:70737] Signal: Aborted (6)
[fv-az774-16:70737] Signal code:  (-6)
[fv-az774-16:70737] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f9337242520]
[fv-az774-16:70737] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f93372969fc]
[fv-az774-16:70737] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f9337242476]
[fv-az774-16:70737] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f93372287f3]
[fv-az774-16:70737] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f93376a2b9e]
[fv-az774-16:70737] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f93376ae20c]
[fv-az774-16:70737] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f93376ae277]
[fv-az774-16:70737] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f93376ae52b]
[fv-az774-16:70737] [ 8] plumed(+0x12f48)[0x558f42459f48]
[fv-az774-16:70737] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f9337229d90]
[fv-az774-16:70737] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f9337229e40]
[fv-az774-16:70737] [11] plumed(+0x131e5)[0x558f4245a1e5]
[fv-az774-16:70737] *** End of error message ***
</pre>
{% endraw %}
