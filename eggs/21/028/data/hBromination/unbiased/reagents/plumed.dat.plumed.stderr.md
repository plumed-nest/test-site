**Project ID:** [plumID:21.028]({{ '/' | absolute_url }}eggs/21/028/)  
Stderr for source:  hBromination/unbiased/reagents/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Keywords.cpp:263) void PLMD::Keywords::addFlag(const std::string&, bool, const std::string&)
+++ assertion failed: !def
the second argument to addFlag must be false COMPONENTS
[runnervm1li68:10692] *** Process received signal ***
[runnervm1li68:10692] Signal: Aborted (6)
[runnervm1li68:10692] Signal code:  (-6)
[runnervm1li68:10692] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f66fb245330]
[runnervm1li68:10692] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f66fb29eb2c]
[runnervm1li68:10692] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f66fb24527e]
[runnervm1li68:10692] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f66fb2288ff]
[runnervm1li68:10692] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f66fb6a5ff5]
[runnervm1li68:10692] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f66fb6bb0da]
[runnervm1li68:10692] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f66fb6a5a55]
[runnervm1li68:10692] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f66fb6a5a6f]
[runnervm1li68:10692] [ 8] plumed(+0x146dd)[0x55bef56fe6dd]
[runnervm1li68:10692] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f66fb22a1ca]
[runnervm1li68:10692] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f66fb22a28b]
[runnervm1li68:10692] [11] plumed(+0x15365)[0x55bef56ff365]
[runnervm1li68:10692] *** End of error message ***
</pre>
{% endraw %}
