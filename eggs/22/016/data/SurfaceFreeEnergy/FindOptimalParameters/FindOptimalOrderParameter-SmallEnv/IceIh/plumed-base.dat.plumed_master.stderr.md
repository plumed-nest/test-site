**Project ID:** [plumID:22.016]({{ '/' | absolute_url }}eggs/22/016/)  
Stderr for source:  SurfaceFreeEnergy/FindOptimalParameters/FindOptimalOrderParameter-SmallEnv/IceIh/plumed-base.dat   
Download: [zipped raw stdout](plumed-base.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed-base.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @45 : keyword ARG is compulsory for this action
[runnervm1li68:06955] *** Process received signal ***
[runnervm1li68:06955] Signal: Aborted (6)
[runnervm1li68:06955] Signal code:  (-6)
[runnervm1li68:06955] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f9152445330]
[runnervm1li68:06955] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f915249eb2c]
[runnervm1li68:06955] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f915244527e]
[runnervm1li68:06955] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f91524288ff]
[runnervm1li68:06955] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f91528a5ff5]
[runnervm1li68:06955] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f91528bb0da]
[runnervm1li68:06955] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f91528a5a55]
[runnervm1li68:06955] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f91528a5a6f]
[runnervm1li68:06955] [ 8] plumed_master(+0x146dd)[0x557cd07186dd]
[runnervm1li68:06955] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f915242a1ca]
[runnervm1li68:06955] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f915242a28b]
[runnervm1li68:06955] [11] plumed_master(+0x15365)[0x557cd0719365]
[runnervm1li68:06955] *** End of error message ***
</pre>
{% endraw %}
