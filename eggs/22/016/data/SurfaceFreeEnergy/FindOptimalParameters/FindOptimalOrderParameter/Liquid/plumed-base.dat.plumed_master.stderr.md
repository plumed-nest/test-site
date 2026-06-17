**Project ID:** [plumID:22.016]({{ '/' | absolute_url }}eggs/22/016/)  
Stderr for source:  SurfaceFreeEnergy/FindOptimalParameters/FindOptimalOrderParameter/Liquid/plumed-base.dat   
Download: [zipped raw stdout](plumed-base.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed-base.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @45 : keyword ARG is compulsory for this action
[runnervm1li68:06874] *** Process received signal ***
[runnervm1li68:06874] Signal: Aborted (6)
[runnervm1li68:06874] Signal code:  (-6)
[runnervm1li68:06874] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fd640245330]
[runnervm1li68:06874] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fd64029eb2c]
[runnervm1li68:06874] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fd64024527e]
[runnervm1li68:06874] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fd6402288ff]
[runnervm1li68:06874] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fd6406a5ff5]
[runnervm1li68:06874] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fd6406bb0da]
[runnervm1li68:06874] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fd6406a5a55]
[runnervm1li68:06874] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fd6406a5a6f]
[runnervm1li68:06874] [ 8] plumed_master(+0x146dd)[0x55daa030f6dd]
[runnervm1li68:06874] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fd64022a1ca]
[runnervm1li68:06874] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fd64022a28b]
[runnervm1li68:06874] [11] plumed_master(+0x15365)[0x55daa0310365]
[runnervm1li68:06874] *** End of error message ***
</pre>
{% endraw %}
