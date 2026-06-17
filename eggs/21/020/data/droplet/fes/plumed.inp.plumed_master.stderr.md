**Project ID:** [plumID:21.020]({{ '/' | absolute_url }}eggs/21/020/)  
Stderr for source:  droplet/fes/plumed.inp   
Download: [zipped raw stdout](plumed.inp.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Keywords.cpp:378) void PLMD::Keywords::use(std::string_view)
+++ assertion failed: reserved(k)
the ARG keyword is not reserved
[runnervm1li68:08940] *** Process received signal ***
[runnervm1li68:08940] Signal: Aborted (6)
[runnervm1li68:08940] Signal code:  (-6)
[runnervm1li68:08940] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7faed1245330]
[runnervm1li68:08940] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7faed129eb2c]
[runnervm1li68:08940] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7faed124527e]
[runnervm1li68:08940] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7faed12288ff]
[runnervm1li68:08940] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7faed16a5ff5]
[runnervm1li68:08940] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7faed16bb0da]
[runnervm1li68:08940] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7faed16a5a55]
[runnervm1li68:08940] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7faed16a5a6f]
[runnervm1li68:08940] [ 8] plumed_master(+0x146dd)[0x5598081926dd]
[runnervm1li68:08940] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7faed122a1ca]
[runnervm1li68:08940] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7faed122a28b]
[runnervm1li68:08940] [11] plumed_master(+0x15365)[0x559808193365]
[runnervm1li68:08940] *** End of error message ***
</pre>
{% endraw %}
