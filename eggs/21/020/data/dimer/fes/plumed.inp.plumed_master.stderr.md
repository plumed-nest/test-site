**Project ID:** [plumID:21.020]({{ '/' | absolute_url }}eggs/21/020/)  
Stderr for source:  dimer/fes/plumed.inp   
Download: [zipped raw stdout](plumed.inp.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action HISTOGRAM with label @s19 : set NORMALIZATION=true/false when using LOGWEIGHTS as otherwise the weights are ignored. Alternatively, learn to use the new syntax for histograms with KDE/ACCUMULATE to have more control over what PLUMED is calculating
[runnervm1li68:09069] *** Process received signal ***
[runnervm1li68:09069] Signal: Aborted (6)
[runnervm1li68:09069] Signal code:  (-6)
[runnervm1li68:09069] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f4aafc45330]
[runnervm1li68:09069] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f4aafc9eb2c]
[runnervm1li68:09069] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f4aafc4527e]
[runnervm1li68:09069] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f4aafc288ff]
[runnervm1li68:09069] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f4ab00a5ff5]
[runnervm1li68:09069] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f4ab00bb0da]
[runnervm1li68:09069] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f4ab00a5a55]
[runnervm1li68:09069] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f4ab00a5a6f]
[runnervm1li68:09069] [ 8] plumed_master(+0x146dd)[0x55e7729006dd]
[runnervm1li68:09069] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f4aafc2a1ca]
[runnervm1li68:09069] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f4aafc2a28b]
[runnervm1li68:09069] [11] plumed_master(+0x15365)[0x55e772901365]
[runnervm1li68:09069] *** End of error message ***
</pre>
{% endraw %}
