**Project ID:** [plumID:21.028]({{ '/' | absolute_url }}eggs/21/028/)  
Stderr for source:  hBromination/unbiased/anti_markovnikov/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Keywords.cpp:483) void PLMD::Keywords::addFlag(std::string_view, bool, std::string_view)
+++ assertion failed: !defaultValue
the second argument to addFlag must be false COMPONENTS
[runnervm1li68:10598] *** Process received signal ***
[runnervm1li68:10598] Signal: Aborted (6)
[runnervm1li68:10598] Signal code:  (-6)
[runnervm1li68:10598] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fddc5a45330]
[runnervm1li68:10598] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fddc5a9eb2c]
[runnervm1li68:10598] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fddc5a4527e]
[runnervm1li68:10598] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fddc5a288ff]
[runnervm1li68:10598] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fddc5ea5ff5]
[runnervm1li68:10598] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fddc5ebb0da]
[runnervm1li68:10598] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fddc5ea5a55]
[runnervm1li68:10598] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fddc5ea5a6f]
[runnervm1li68:10598] [ 8] plumed_master(+0x146dd)[0x561f72b2a6dd]
[runnervm1li68:10598] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fddc5a2a1ca]
[runnervm1li68:10598] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fddc5a2a28b]
[runnervm1li68:10598] [11] plumed_master(+0x15365)[0x561f72b2b365]
[runnervm1li68:10598] *** End of error message ***
</pre>
{% endraw %}
