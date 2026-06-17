**Project ID:** [plumID:25.023]({{ '/' | absolute_url }}eggs/25/023/)  
Stderr for source:  update_2026/analysis/rewighting_2d_map_rmsd_cshape/monomer/plumed_rew.dat   
Download: [zipped raw stdout](plumed_rew.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_rew.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action HISTOGRAM with label @s16 : set NORMALIZATION=true/false when using LOGWEIGHTS as otherwise the weights are ignored. Alternatively, learn to use the new syntax for histograms with KDE/ACCUMULATE to have more control over what PLUMED is calculating
[runnervm1li68:04695] *** Process received signal ***
[runnervm1li68:04695] Signal: Aborted (6)
[runnervm1li68:04695] Signal code:  (-6)
[runnervm1li68:04695] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f374a645330]
[runnervm1li68:04695] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f374a69eb2c]
[runnervm1li68:04695] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f374a64527e]
[runnervm1li68:04695] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f374a6288ff]
[runnervm1li68:04695] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f374aaa5ff5]
[runnervm1li68:04695] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f374aabb0da]
[runnervm1li68:04695] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f374aaa5a55]
[runnervm1li68:04695] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f374aaa5a6f]
[runnervm1li68:04695] [ 8] plumed(+0x146dd)[0x55a600bce6dd]
[runnervm1li68:04695] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f374a62a1ca]
[runnervm1li68:04695] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f374a62a28b]
[runnervm1li68:04695] [11] plumed(+0x15365)[0x55a600bcf365]
[runnervm1li68:04695] *** End of error message ***
</pre>
{% endraw %}
