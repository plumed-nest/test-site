**Project ID:** [plumID:22.016]({{ '/' | absolute_url }}eggs/22/016/)  
Stderr for source:  SurfaceFreeEnergy/FindOptimalParameters/FindOptimalOrderParameter/Liquid/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @45 : keyword ARG is compulsory for this action
[runnervm1li68:06916] *** Process received signal ***
[runnervm1li68:06916] Signal: Aborted (6)
[runnervm1li68:06916] Signal code:  (-6)
[runnervm1li68:06916] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fecf2e45330]
[runnervm1li68:06916] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fecf2e9eb2c]
[runnervm1li68:06916] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fecf2e4527e]
[runnervm1li68:06916] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fecf2e288ff]
[runnervm1li68:06916] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fecf32a5ff5]
[runnervm1li68:06916] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fecf32bb0da]
[runnervm1li68:06916] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fecf32a5a55]
[runnervm1li68:06916] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fecf32a5a6f]
[runnervm1li68:06916] [ 8] plumed_master(+0x146dd)[0x562ae59876dd]
[runnervm1li68:06916] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fecf2e2a1ca]
[runnervm1li68:06916] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fecf2e2a28b]
[runnervm1li68:06916] [11] plumed_master(+0x15365)[0x562ae5988365]
[runnervm1li68:06916] *** End of error message ***
</pre>
{% endraw %}
