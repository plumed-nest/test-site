**Project ID:** [plumID:19.081]({{ '/' | absolute_url }}eggs/19/081/)  
Stderr for source:  Al/02_FCC/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
../../RefCV.c3WJee.cpp:22:10: fatal error: multicolvar/MultiColvarBase.h: No such file or directory
22 | #include "multicolvar/MultiColvarBase.h"
|          ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1494) void PLMD::PlumedMain::load(const std::string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed' PLUMED_VERSION='2.10.0' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed"/scripts/mklib.sh -n -o ./../../RefCV.2.10.0.so ../../RefCV.cpp

[runnervm1li68:09767] *** Process received signal ***
[runnervm1li68:09767] Signal: Aborted (6)
[runnervm1li68:09767] Signal code:  (-6)
[runnervm1li68:09767] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f9acce45330]
[runnervm1li68:09767] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f9acce9eb2c]
[runnervm1li68:09767] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f9acce4527e]
[runnervm1li68:09767] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f9acce288ff]
[runnervm1li68:09767] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f9acd2a5ff5]
[runnervm1li68:09767] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f9acd2bb0da]
[runnervm1li68:09767] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f9acd2a5a55]
[runnervm1li68:09767] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f9acd2a5a6f]
[runnervm1li68:09767] [ 8] plumed(+0x146dd)[0x559b070446dd]
[runnervm1li68:09767] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f9acce2a1ca]
[runnervm1li68:09767] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f9acce2a28b]
[runnervm1li68:09767] [11] plumed(+0x15365)[0x559b07045365]
[runnervm1li68:09767] *** End of error message ***
</pre>
{% endraw %}
