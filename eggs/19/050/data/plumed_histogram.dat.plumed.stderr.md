**Project ID:** [plumID:19.050]({{ '/' | absolute_url }}eggs/19/050/)  
Stderr for source:  plumed_histogram.dat   
Download: [zipped raw stdout](plumed_histogram.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_histogram.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action HISTOGRAM with label @s12 : set NORMALIZATION=true/false when using LOGWEIGHTS as otherwise the weights are ignored. Alternatively, learn to use the new syntax for histograms with KDE/ACCUMULATE to have more control over what PLUMED is calculating
[runnervm1li68:11882] *** Process received signal ***
[runnervm1li68:11882] Signal: Aborted (6)
[runnervm1li68:11882] Signal code:  (-6)
[runnervm1li68:11882] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7efed9445330]
[runnervm1li68:11882] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7efed949eb2c]
[runnervm1li68:11882] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7efed944527e]
[runnervm1li68:11882] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7efed94288ff]
[runnervm1li68:11882] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7efed98a5ff5]
[runnervm1li68:11882] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7efed98bb0da]
[runnervm1li68:11882] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7efed98a5a55]
[runnervm1li68:11882] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7efed98a5a6f]
[runnervm1li68:11882] [ 8] plumed(+0x146dd)[0x556064d966dd]
[runnervm1li68:11882] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7efed942a1ca]
[runnervm1li68:11882] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7efed942a28b]
[runnervm1li68:11882] [11] plumed(+0x15365)[0x556064d97365]
[runnervm1li68:11882] *** End of error message ***
</pre>
{% endraw %}
