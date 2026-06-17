**Project ID:** [plumID:20.028]({{ '/' | absolute_url }}eggs/20/028/)  
Stderr for source:  oncogenic/plumed-1.dat   
Download: [zipped raw stdout](plumed-1.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed-1.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Tools.h:173) static void PLMD::Tools::convert(const T&, U&) [with T = std::__cxx11::basic_string<char>; U = double]
+++ assertion failed: convertNoexcept(t,u)
Error converting  483  97.1
[runnervm1li68:10038] *** Process received signal ***
[runnervm1li68:10038] Signal: Aborted (6)
[runnervm1li68:10038] Signal code:  (-6)
[runnervm1li68:10038] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fe5c7045330]
[runnervm1li68:10038] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fe5c709eb2c]
[runnervm1li68:10038] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fe5c704527e]
[runnervm1li68:10038] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fe5c70288ff]
[runnervm1li68:10038] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fe5c74a5ff5]
[runnervm1li68:10038] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fe5c74bb0da]
[runnervm1li68:10038] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fe5c74a5a55]
[runnervm1li68:10038] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fe5c74a5a6f]
[runnervm1li68:10038] [ 8] plumed_master(+0x146dd)[0x55d3547936dd]
[runnervm1li68:10038] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fe5c702a1ca]
[runnervm1li68:10038] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fe5c702a28b]
[runnervm1li68:10038] [11] plumed_master(+0x15365)[0x55d354794365]
[runnervm1li68:10038] *** End of error message ***
</pre>
{% endraw %}
