**Project ID:** [plumID:24.032]({{ '/' | absolute_url }}eggs/24/032/)  
Stderr for source:  analysis/PremiR21/OPES/plumed_DeepLNE.dat   
Download: [zipped raw stdout](plumed_DeepLNE.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_DeepLNE.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: using a legacy ActionRegister.h include path, please use <<#include "core/ActionRegister.h">>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Keywords.cpp:378) void PLMD::Keywords::use(std::string_view)
+++ assertion failed: reserved(k)
the ARG keyword is not reserved
[runnervm1li68:05040] *** Process received signal ***
[runnervm1li68:05040] Signal: Aborted (6)
[runnervm1li68:05040] Signal code:  (-6)
[runnervm1li68:05040] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f5fe4245330]
[runnervm1li68:05040] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f5fe429eb2c]
[runnervm1li68:05040] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f5fe424527e]
[runnervm1li68:05040] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f5fe42288ff]
[runnervm1li68:05040] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f5fe46a5ff5]
[runnervm1li68:05040] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f5fe46bb0da]
[runnervm1li68:05040] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f5fe46a5a55]
[runnervm1li68:05040] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f5fe46a5a6f]
[runnervm1li68:05040] [ 8] plumed_master(+0x146dd)[0x55852a5c36dd]
[runnervm1li68:05040] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f5fe422a1ca]
[runnervm1li68:05040] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f5fe422a28b]
[runnervm1li68:05040] [11] plumed_master(+0x15365)[0x55852a5c4365]
[runnervm1li68:05040] *** End of error message ***
</pre>
{% endraw %}
