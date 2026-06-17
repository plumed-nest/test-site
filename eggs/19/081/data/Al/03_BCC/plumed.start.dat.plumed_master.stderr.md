**Project ID:** [plumID:19.081]({{ '/' | absolute_url }}eggs/19/081/)  
Stderr for source:  Al/03_BCC/plumed.start.dat   
Download: [zipped raw stdout](plumed.start.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.start.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
../../RefCV.G9oFjF.cpp:22:10: fatal error: multicolvar/MultiColvarBase.h: No such file or directory
22 | #include "multicolvar/MultiColvarBase.h"
|          ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1494) void PLMD::PlumedMain::load(const std::string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed_master' PLUMED_VERSION='2.11.0-dev' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed_master' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed_master' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh -n -o ./../../RefCV.2.11.0-dev.so ../../RefCV.cpp

[runnervm1li68:10058] *** Process received signal ***
[runnervm1li68:10058] Signal: Aborted (6)
[runnervm1li68:10058] Signal code:  (-6)
[runnervm1li68:10058] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f8010045330]
[runnervm1li68:10058] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f801009eb2c]
[runnervm1li68:10058] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f801004527e]
[runnervm1li68:10058] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f80100288ff]
[runnervm1li68:10058] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f80104a5ff5]
[runnervm1li68:10058] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f80104bb0da]
[runnervm1li68:10058] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f80104a5a55]
[runnervm1li68:10058] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f80104a5a6f]
[runnervm1li68:10058] [ 8] plumed_master(+0x146dd)[0x56098a56c6dd]
[runnervm1li68:10058] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f801002a1ca]
[runnervm1li68:10058] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f801002a28b]
[runnervm1li68:10058] [11] plumed_master(+0x15365)[0x56098a56d365]
[runnervm1li68:10058] *** End of error message ***
</pre>
{% endraw %}
