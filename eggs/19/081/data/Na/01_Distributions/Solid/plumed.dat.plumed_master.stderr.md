**Project ID:** [plumID:19.081]({{ '/' | absolute_url }}eggs/19/081/)  
Stderr for source:  Na/01_Distributions/Solid/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
../../../RefCV.oAEAvk.cpp:22:10: fatal error: multicolvar/MultiColvarBase.h: No such file or directory
22 | #include "multicolvar/MultiColvarBase.h"
|          ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1494) void PLMD::PlumedMain::load(const std::string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed_master' PLUMED_VERSION='2.11.0-dev' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed_master' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed_master' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed_master"/scripts/mklib.sh -n -o ./../../../RefCV.2.11.0-dev.so ../../../RefCV.cpp

[runnervm1li68:10229] *** Process received signal ***
[runnervm1li68:10229] Signal: Aborted (6)
[runnervm1li68:10229] Signal code:  (-6)
[runnervm1li68:10229] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f0ed5445330]
[runnervm1li68:10229] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f0ed549eb2c]
[runnervm1li68:10229] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f0ed544527e]
[runnervm1li68:10229] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f0ed54288ff]
[runnervm1li68:10229] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f0ed58a5ff5]
[runnervm1li68:10229] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f0ed58bb0da]
[runnervm1li68:10229] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f0ed58a5a55]
[runnervm1li68:10229] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f0ed58a5a6f]
[runnervm1li68:10229] [ 8] plumed_master(+0x146dd)[0x55803369e6dd]
[runnervm1li68:10229] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f0ed542a1ca]
[runnervm1li68:10229] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f0ed542a28b]
[runnervm1li68:10229] [11] plumed_master(+0x15365)[0x55803369f365]
[runnervm1li68:10229] *** End of error message ***
</pre>
{% endraw %}
