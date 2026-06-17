**Project ID:** [plumID:22.023]({{ '/' | absolute_url }}eggs/22/023/)  
Stderr for source:  PRODUCTION/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:93) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file ../structure.pdb
[runnervm1li68:08242] *** Process received signal ***
[runnervm1li68:08242] Signal: Aborted (6)
[runnervm1li68:08242] Signal code:  (-6)
[runnervm1li68:08242] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f2c37e45330]
[runnervm1li68:08242] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f2c37e9eb2c]
[runnervm1li68:08242] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f2c37e4527e]
[runnervm1li68:08242] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f2c37e288ff]
[runnervm1li68:08242] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f2c382a5ff5]
[runnervm1li68:08242] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f2c382bb0da]
[runnervm1li68:08242] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f2c382a5a55]
[runnervm1li68:08242] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f2c382a5a6f]
[runnervm1li68:08242] [ 8] plumed(+0x146dd)[0x5640214f46dd]
[runnervm1li68:08242] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f2c37e2a1ca]
[runnervm1li68:08242] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f2c37e2a28b]
[runnervm1li68:08242] [11] plumed(+0x15365)[0x5640214f5365]
[runnervm1li68:08242] *** End of error message ***
</pre>
{% endraw %}
