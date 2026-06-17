**Project ID:** [plumID:21.020]({{ '/' | absolute_url }}eggs/21/020/)  
Stderr for source:  hbr/fes/plumed.inp   
Download: [zipped raw stdout](plumed.inp.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action HISTOGRAM with label @s31 : set NORMALIZATION=true/false when using LOGWEIGHTS as otherwise the weights are ignored. Alternatively, learn to use the new syntax for histograms with KDE/ACCUMULATE to have more control over what PLUMED is calculating
[runnervm1li68:09207] *** Process received signal ***
[runnervm1li68:09207] Signal: Aborted (6)
[runnervm1li68:09207] Signal code:  (-6)
[runnervm1li68:09207] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f9920445330]
[runnervm1li68:09207] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f992049eb2c]
[runnervm1li68:09207] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f992044527e]
[runnervm1li68:09207] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f99204288ff]
[runnervm1li68:09207] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f99208a5ff5]
[runnervm1li68:09207] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f99208bb0da]
[runnervm1li68:09207] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f99208a5a55]
[runnervm1li68:09207] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f99208a5a6f]
[runnervm1li68:09207] [ 8] plumed(+0x146dd)[0x55802a6d86dd]
[runnervm1li68:09207] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f992042a1ca]
[runnervm1li68:09207] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f992042a28b]
[runnervm1li68:09207] [11] plumed(+0x15365)[0x55802a6d9365]
[runnervm1li68:09207] *** End of error message ***
</pre>
{% endraw %}
