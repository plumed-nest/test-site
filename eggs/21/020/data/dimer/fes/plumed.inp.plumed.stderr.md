**Project ID:** [plumID:21.020]({{ '/' | absolute_url }}eggs/21/020/)  
Stderr for source:  dimer/fes/plumed.inp   
Download: [zipped raw stdout](plumed.inp.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action HISTOGRAM with label @s19 : set NORMALIZATION=true/false when using LOGWEIGHTS as otherwise the weights are ignored. Alternatively, learn to use the new syntax for histograms with KDE/ACCUMULATE to have more control over what PLUMED is calculating
[runnervm1li68:09053] *** Process received signal ***
[runnervm1li68:09053] Signal: Aborted (6)
[runnervm1li68:09053] Signal code:  (-6)
[runnervm1li68:09053] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f4077e45330]
[runnervm1li68:09053] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f4077e9eb2c]
[runnervm1li68:09053] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f4077e4527e]
[runnervm1li68:09053] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f4077e288ff]
[runnervm1li68:09053] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f40782a5ff5]
[runnervm1li68:09053] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f40782bb0da]
[runnervm1li68:09053] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f40782a5a55]
[runnervm1li68:09053] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f40782a5a6f]
[runnervm1li68:09053] [ 8] plumed(+0x146dd)[0x560390f186dd]
[runnervm1li68:09053] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f4077e2a1ca]
[runnervm1li68:09053] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f4077e2a28b]
[runnervm1li68:09053] [11] plumed(+0x15365)[0x560390f19365]
[runnervm1li68:09053] *** End of error message ***
</pre>
{% endraw %}
