**Project ID:** [plumID:24.033]({{ '/' | absolute_url }}eggs/24/033/)  
Stderr for source:  Plumed-nest/7q4m/plumed_analysis.dat   
Download: [zipped raw stdout](plumed_analysis.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_analysis.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action PRINT with label @252 : cannot use argument parabeta0_both.struct-1 in input as not all elements are computed
[runnervm1li68:05419] *** Process received signal ***
[runnervm1li68:05419] Signal: Aborted (6)
[runnervm1li68:05419] Signal code:  (-6)
[runnervm1li68:05419] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f2c73445330]
[runnervm1li68:05419] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f2c7349eb2c]
[runnervm1li68:05419] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f2c7344527e]
[runnervm1li68:05419] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f2c734288ff]
[runnervm1li68:05419] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f2c738a5ff5]
[runnervm1li68:05419] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f2c738bb0da]
[runnervm1li68:05419] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f2c738a5a55]
[runnervm1li68:05419] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f2c738a5a6f]
[runnervm1li68:05419] [ 8] plumed_master(+0x146dd)[0x56447693a6dd]
[runnervm1li68:05419] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f2c7342a1ca]
[runnervm1li68:05419] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f2c7342a28b]
[runnervm1li68:05419] [11] plumed_master(+0x15365)[0x56447693b365]
[runnervm1li68:05419] *** End of error message ***
</pre>
{% endraw %}
