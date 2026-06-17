**Project ID:** [plumID:25.023]({{ '/' | absolute_url }}eggs/25/023/)  
Stderr for source:  update_2026/analysis/rewighting_2d_map_rmsd_cshape/pentamer/plumed_rew.dat   
Download: [zipped raw stdout](plumed_rew.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_rew.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action HISTOGRAM with label @s30 : set NORMALIZATION=true/false when using LOGWEIGHTS as otherwise the weights are ignored. Alternatively, learn to use the new syntax for histograms with KDE/ACCUMULATE to have more control over what PLUMED is calculating
[runnervm1li68:04763] *** Process received signal ***
[runnervm1li68:04763] Signal: Aborted (6)
[runnervm1li68:04763] Signal code:  (-6)
[runnervm1li68:04763] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f3ce2c45330]
[runnervm1li68:04763] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f3ce2c9eb2c]
[runnervm1li68:04763] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f3ce2c4527e]
[runnervm1li68:04763] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f3ce2c288ff]
[runnervm1li68:04763] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f3ce30a5ff5]
[runnervm1li68:04763] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f3ce30bb0da]
[runnervm1li68:04763] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f3ce30a5a55]
[runnervm1li68:04763] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f3ce30a5a6f]
[runnervm1li68:04763] [ 8] plumed_master(+0x146dd)[0x55d1574bd6dd]
[runnervm1li68:04763] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f3ce2c2a1ca]
[runnervm1li68:04763] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f3ce2c2a28b]
[runnervm1li68:04763] [11] plumed_master(+0x15365)[0x55d1574be365]
[runnervm1li68:04763] *** End of error message ***
</pre>
{% endraw %}
