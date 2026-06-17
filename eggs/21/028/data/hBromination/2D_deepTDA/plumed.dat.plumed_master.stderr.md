**Project ID:** [plumID:21.028]({{ '/' | absolute_url }}eggs/21/028/)  
Stderr for source:  hBromination/2D_deepTDA/plumed.dat   
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
[runnervm1li68:10543] *** Process received signal ***
[runnervm1li68:10543] Signal: Aborted (6)
[runnervm1li68:10543] Signal code:  (-6)
[runnervm1li68:10543] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fc33ea45330]
[runnervm1li68:10543] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fc33ea9eb2c]
[runnervm1li68:10543] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fc33ea4527e]
[runnervm1li68:10543] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fc33ea288ff]
[runnervm1li68:10543] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fc33eea5ff5]
[runnervm1li68:10543] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fc33eebb0da]
[runnervm1li68:10543] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fc33eea5a55]
[runnervm1li68:10543] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fc33eea5a6f]
[runnervm1li68:10543] [ 8] plumed_master(+0x146dd)[0x558d5fe576dd]
[runnervm1li68:10543] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fc33ea2a1ca]
[runnervm1li68:10543] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fc33ea2a28b]
[runnervm1li68:10543] [11] plumed_master(+0x15365)[0x558d5fe58365]
[runnervm1li68:10543] *** End of error message ***
</pre>
{% endraw %}
