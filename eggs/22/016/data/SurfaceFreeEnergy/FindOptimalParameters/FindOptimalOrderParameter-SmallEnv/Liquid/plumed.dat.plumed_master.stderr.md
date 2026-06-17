**Project ID:** [plumID:22.016]({{ '/' | absolute_url }}eggs/22/016/)  
Stderr for source:  SurfaceFreeEnergy/FindOptimalParameters/FindOptimalOrderParameter-SmallEnv/Liquid/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @45 : keyword ARG is compulsory for this action
[runnervm1li68:07070] *** Process received signal ***
[runnervm1li68:07070] Signal: Aborted (6)
[runnervm1li68:07070] Signal code:  (-6)
[runnervm1li68:07070] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f24ecc45330]
[runnervm1li68:07070] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f24ecc9eb2c]
[runnervm1li68:07070] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f24ecc4527e]
[runnervm1li68:07070] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f24ecc288ff]
[runnervm1li68:07070] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f24ed0a5ff5]
[runnervm1li68:07070] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f24ed0bb0da]
[runnervm1li68:07070] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f24ed0a5a55]
[runnervm1li68:07070] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f24ed0a5a6f]
[runnervm1li68:07070] [ 8] plumed_master(+0x146dd)[0x5624624436dd]
[runnervm1li68:07070] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f24ecc2a1ca]
[runnervm1li68:07070] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f24ecc2a28b]
[runnervm1li68:07070] [11] plumed_master(+0x15365)[0x562462444365]
[runnervm1li68:07070] *** End of error message ***
</pre>
{% endraw %}
