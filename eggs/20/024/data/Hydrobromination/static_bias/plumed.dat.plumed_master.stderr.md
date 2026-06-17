**Project ID:** [plumID:20.024]({{ '/' | absolute_url }}eggs/20/024/)  
Stderr for source:  Hydrobromination/static_bias/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Keywords.cpp:378) void PLMD::Keywords::use(std::string_view)
+++ assertion failed: reserved(k)
the ARG keyword is not reserved
[runnervm1li68:10318] *** Process received signal ***
[runnervm1li68:10318] Signal: Aborted (6)
[runnervm1li68:10318] Signal code:  (-6)
[runnervm1li68:10318] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fcc74845330]
[runnervm1li68:10318] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fcc7489eb2c]
[runnervm1li68:10318] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fcc7484527e]
[runnervm1li68:10318] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fcc748288ff]
[runnervm1li68:10318] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fcc74ca5ff5]
[runnervm1li68:10318] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fcc74cbb0da]
[runnervm1li68:10318] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fcc74ca5a55]
[runnervm1li68:10318] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fcc74ca5a6f]
[runnervm1li68:10318] [ 8] plumed_master(+0x146dd)[0x558938f1c6dd]
[runnervm1li68:10318] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fcc7482a1ca]
[runnervm1li68:10318] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fcc7482a28b]
[runnervm1li68:10318] [11] plumed_master(+0x15365)[0x558938f1d365]
[runnervm1li68:10318] *** End of error message ***
</pre>
{% endraw %}
