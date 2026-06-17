**Project ID:** [plumID:19.081]({{ '/' | absolute_url }}eggs/19/081/)  
Stderr for source:  Na/02_References/Example/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
../../../RefCV.u1fXW8.cpp:22:10: fatal error: multicolvar/MultiColvarBase.h: No such file or directory
22 | #include "multicolvar/MultiColvarBase.h"
|          ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1494) void PLMD::PlumedMain::load(const std::string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed_master' PLUMED_VERSION='2.11.0-dev' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed_master' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed_master' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh -n -o ./../../../RefCV.2.11.0-dev.so ../../../RefCV.cpp

[runnervm1li68:10366] *** Process received signal ***
[runnervm1li68:10366] Signal: Aborted (6)
[runnervm1li68:10366] Signal code:  (-6)
[runnervm1li68:10366] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fa454e45330]
[runnervm1li68:10366] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fa454e9eb2c]
[runnervm1li68:10366] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fa454e4527e]
[runnervm1li68:10366] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fa454e288ff]
[runnervm1li68:10366] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fa4552a5ff5]
[runnervm1li68:10366] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fa4552bb0da]
[runnervm1li68:10366] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fa4552a5a55]
[runnervm1li68:10366] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fa4552a5a6f]
[runnervm1li68:10366] [ 8] plumed_master(+0x146dd)[0x559dc60f46dd]
[runnervm1li68:10366] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fa454e2a1ca]
[runnervm1li68:10366] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fa454e2a28b]
[runnervm1li68:10366] [11] plumed_master(+0x15365)[0x559dc60f5365]
[runnervm1li68:10366] *** End of error message ***
</pre>
{% endraw %}
