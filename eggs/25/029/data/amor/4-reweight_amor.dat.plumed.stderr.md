**Project ID:** [plumID:25.029]({{ '/' | absolute_url }}eggs/25/029/)  
Stderr for source:  ./amor/4-reweight_amor.dat   
Download: [zipped raw stdout](4-reweight_amor.dat.plumed.stdout.txt.zip) - [zipped raw stderr](4-reweight_amor.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action HISTOGRAM with label @s33 : set NORMALIZATION=true/false when using LOGWEIGHTS as otherwise the weights are ignored. Alternatively, learn to use the new syntax for histograms with KDE/ACCUMULATE to have more control over what PLUMED is calculating
[runnervm1li68:04439] *** Process received signal ***
[runnervm1li68:04439] Signal: Aborted (6)
[runnervm1li68:04439] Signal code:  (-6)
[runnervm1li68:04439] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fa3d7045330]
[runnervm1li68:04439] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fa3d709eb2c]
[runnervm1li68:04439] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fa3d704527e]
[runnervm1li68:04439] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fa3d70288ff]
[runnervm1li68:04439] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fa3d74a5ff5]
[runnervm1li68:04439] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fa3d74bb0da]
[runnervm1li68:04439] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fa3d74a5a55]
[runnervm1li68:04439] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fa3d74a5a6f]
[runnervm1li68:04439] [ 8] plumed(+0x146dd)[0x556f6d6d46dd]
[runnervm1li68:04439] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fa3d702a1ca]
[runnervm1li68:04439] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fa3d702a28b]
[runnervm1li68:04439] [11] plumed(+0x15365)[0x556f6d6d5365]
[runnervm1li68:04439] *** End of error message ***
</pre>
{% endraw %}
