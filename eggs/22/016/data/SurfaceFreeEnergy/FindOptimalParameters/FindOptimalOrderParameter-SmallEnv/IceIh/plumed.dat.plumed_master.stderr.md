**Project ID:** [plumID:22.016]({{ '/' | absolute_url }}eggs/22/016/)  
Stderr for source:  SurfaceFreeEnergy/FindOptimalParameters/FindOptimalOrderParameter-SmallEnv/IceIh/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @45 : keyword ARG is compulsory for this action
[runnervm1li68:06993] *** Process received signal ***
[runnervm1li68:06993] Signal: Aborted (6)
[runnervm1li68:06993] Signal code:  (-6)
[runnervm1li68:06993] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fdbe3845330]
[runnervm1li68:06993] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fdbe389eb2c]
[runnervm1li68:06993] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fdbe384527e]
[runnervm1li68:06993] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fdbe38288ff]
[runnervm1li68:06993] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fdbe3ca5ff5]
[runnervm1li68:06993] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fdbe3cbb0da]
[runnervm1li68:06993] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fdbe3ca5a55]
[runnervm1li68:06993] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fdbe3ca5a6f]
[runnervm1li68:06993] [ 8] plumed_master(+0x146dd)[0x56511deb06dd]
[runnervm1li68:06993] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fdbe382a1ca]
[runnervm1li68:06993] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fdbe382a28b]
[runnervm1li68:06993] [11] plumed_master(+0x15365)[0x56511deb1365]
[runnervm1li68:06993] *** End of error message ***
</pre>
{% endraw %}
