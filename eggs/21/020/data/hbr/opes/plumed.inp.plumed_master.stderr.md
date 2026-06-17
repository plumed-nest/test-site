**Project ID:** [plumID:21.020]({{ '/' | absolute_url }}eggs/21/020/)  
Stderr for source:  hbr/opes/plumed.inp   
Download: [zipped raw stdout](plumed.inp.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action HISTOGRAM with label @s28 : set NORMALIZATION=true/false when using LOGWEIGHTS as otherwise the weights are ignored. Alternatively, learn to use the new syntax for histograms with KDE/ACCUMULATE to have more control over what PLUMED is calculating
[runnervm1li68:09428] *** Process received signal ***
[runnervm1li68:09428] Signal: Aborted (6)
[runnervm1li68:09428] Signal code:  (-6)
[runnervm1li68:09428] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fd41b645330]
[runnervm1li68:09428] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fd41b69eb2c]
[runnervm1li68:09428] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fd41b64527e]
[runnervm1li68:09428] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fd41b6288ff]
[runnervm1li68:09428] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fd41baa5ff5]
[runnervm1li68:09428] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fd41babb0da]
[runnervm1li68:09428] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fd41baa5a55]
[runnervm1li68:09428] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fd41baa5a6f]
[runnervm1li68:09428] [ 8] plumed_master(+0x146dd)[0x5612a60b76dd]
[runnervm1li68:09428] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fd41b62a1ca]
[runnervm1li68:09428] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fd41b62a28b]
[runnervm1li68:09428] [11] plumed_master(+0x15365)[0x5612a60b8365]
[runnervm1li68:09428] *** End of error message ***
</pre>
{% endraw %}
