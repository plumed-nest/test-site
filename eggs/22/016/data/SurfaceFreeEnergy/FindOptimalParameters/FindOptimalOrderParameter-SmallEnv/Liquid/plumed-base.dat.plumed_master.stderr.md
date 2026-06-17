**Project ID:** [plumID:22.016]({{ '/' | absolute_url }}eggs/22/016/)  
Stderr for source:  SurfaceFreeEnergy/FindOptimalParameters/FindOptimalOrderParameter-SmallEnv/Liquid/plumed-base.dat   
Download: [zipped raw stdout](plumed-base.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed-base.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @45 : keyword ARG is compulsory for this action
[runnervm1li68:07031] *** Process received signal ***
[runnervm1li68:07031] Signal: Aborted (6)
[runnervm1li68:07031] Signal code:  (-6)
[runnervm1li68:07031] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f9bd5c45330]
[runnervm1li68:07031] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f9bd5c9eb2c]
[runnervm1li68:07031] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f9bd5c4527e]
[runnervm1li68:07031] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f9bd5c288ff]
[runnervm1li68:07031] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f9bd60a5ff5]
[runnervm1li68:07031] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f9bd60bb0da]
[runnervm1li68:07031] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f9bd60a5a55]
[runnervm1li68:07031] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f9bd60a5a6f]
[runnervm1li68:07031] [ 8] plumed_master(+0x146dd)[0x55ab4aa666dd]
[runnervm1li68:07031] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f9bd5c2a1ca]
[runnervm1li68:07031] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f9bd5c2a28b]
[runnervm1li68:07031] [11] plumed_master(+0x15365)[0x55ab4aa67365]
[runnervm1li68:07031] *** End of error message ***
</pre>
{% endraw %}
