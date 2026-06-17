**Project ID:** [plumID:21.001]({{ '/' | absolute_url }}eggs/21/001/)  
Stderr for source:  HS6ST/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action HISTOGRAM with label @s31 : set NORMALIZATION=true/false when using LOGWEIGHTS as otherwise the weights are ignored. Alternatively, learn to use the new syntax for histograms with KDE/ACCUMULATE to have more control over what PLUMED is calculating
[runnervm1li68:10463] *** Process received signal ***
[runnervm1li68:10463] Signal: Aborted (6)
[runnervm1li68:10463] Signal code:  (-6)
[runnervm1li68:10463] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7ff501045330]
[runnervm1li68:10463] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7ff50109eb2c]
[runnervm1li68:10463] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7ff50104527e]
[runnervm1li68:10463] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7ff5010288ff]
[runnervm1li68:10463] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7ff5014a5ff5]
[runnervm1li68:10463] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7ff5014bb0da]
[runnervm1li68:10463] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7ff5014a5a55]
[runnervm1li68:10463] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7ff5014a5a6f]
[runnervm1li68:10463] [ 8] plumed(+0x146dd)[0x55c7139b06dd]
[runnervm1li68:10463] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7ff50102a1ca]
[runnervm1li68:10463] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7ff50102a28b]
[runnervm1li68:10463] [11] plumed(+0x15365)[0x55c7139b1365]
[runnervm1li68:10463] *** End of error message ***
</pre>
{% endraw %}
