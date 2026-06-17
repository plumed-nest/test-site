**Project ID:** [plumID:20.024]({{ '/' | absolute_url }}eggs/20/024/)  
Stderr for source:  Alanine-dipeptide/static_bias/plumed.dat   
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
[runnervm1li68:10232] *** Process received signal ***
[runnervm1li68:10232] Signal: Aborted (6)
[runnervm1li68:10232] Signal code:  (-6)
[runnervm1li68:10232] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f1a99c45330]
[runnervm1li68:10232] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f1a99c9eb2c]
[runnervm1li68:10232] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f1a99c4527e]
[runnervm1li68:10232] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f1a99c288ff]
[runnervm1li68:10232] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f1a9a0a5ff5]
[runnervm1li68:10232] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f1a9a0bb0da]
[runnervm1li68:10232] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f1a9a0a5a55]
[runnervm1li68:10232] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f1a9a0a5a6f]
[runnervm1li68:10232] [ 8] plumed_master(+0x146dd)[0x55bfbc6dc6dd]
[runnervm1li68:10232] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f1a99c2a1ca]
[runnervm1li68:10232] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f1a99c2a28b]
[runnervm1li68:10232] [11] plumed_master(+0x15365)[0x55bfbc6dd365]
[runnervm1li68:10232] *** End of error message ***
</pre>
{% endraw %}
