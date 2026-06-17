**Project ID:** [plumID:25.009]({{ '/' | absolute_url }}eggs/25/009/)  
Stderr for source:  T1_MetaD/hills/plumed-reweight-time-dependent-w1.dat   
Download: [zipped raw stdout](plumed-reweight-time-dependent-w1.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed-reweight-time-dependent-w1.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @23 : keyword ARG is compulsory for this action
[runnervm1li68:05386] *** Process received signal ***
[runnervm1li68:05386] Signal: Aborted (6)
[runnervm1li68:05386] Signal code:  (-6)
[runnervm1li68:05386] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f9bf6c45330]
[runnervm1li68:05386] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f9bf6c9eb2c]
[runnervm1li68:05386] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f9bf6c4527e]
[runnervm1li68:05386] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f9bf6c288ff]
[runnervm1li68:05386] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f9bf70a5ff5]
[runnervm1li68:05386] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f9bf70bb0da]
[runnervm1li68:05386] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f9bf70a5a55]
[runnervm1li68:05386] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f9bf70a5a6f]
[runnervm1li68:05386] [ 8] plumed_master(+0x146dd)[0x562e680a66dd]
[runnervm1li68:05386] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f9bf6c2a1ca]
[runnervm1li68:05386] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f9bf6c2a28b]
[runnervm1li68:05386] [11] plumed_master(+0x15365)[0x562e680a7365]
[runnervm1li68:05386] *** End of error message ***
</pre>
{% endraw %}
