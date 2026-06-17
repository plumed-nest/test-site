**Project ID:** [plumID:21.028]({{ '/' | absolute_url }}eggs/21/028/)  
Stderr for source:  hBromination/unbiased/markovnikov/plumed.dat   
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
[runnervm1li68:10636] *** Process received signal ***
[runnervm1li68:10636] Signal: Aborted (6)
[runnervm1li68:10636] Signal code:  (-6)
[runnervm1li68:10636] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fde9d445330]
[runnervm1li68:10636] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fde9d49eb2c]
[runnervm1li68:10636] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fde9d44527e]
[runnervm1li68:10636] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fde9d4288ff]
[runnervm1li68:10636] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fde9d8a5ff5]
[runnervm1li68:10636] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fde9d8bb0da]
[runnervm1li68:10636] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fde9d8a5a55]
[runnervm1li68:10636] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fde9d8a5a6f]
[runnervm1li68:10636] [ 8] plumed(+0x146dd)[0x55a0f4fa76dd]
[runnervm1li68:10636] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fde9d42a1ca]
[runnervm1li68:10636] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fde9d42a28b]
[runnervm1li68:10636] [11] plumed(+0x15365)[0x55a0f4fa8365]
[runnervm1li68:10636] *** End of error message ***
</pre>
{% endraw %}
