**Project ID:** [plumID:25.023]({{ '/' | absolute_url }}eggs/25/023/)  
Stderr for source:  update_2026/analysis/rewighting_2d_map_rmsd_cshape/trimer/plumed_rew.dat   
Download: [zipped raw stdout](plumed_rew.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_rew.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action HISTOGRAM with label @s24 : set NORMALIZATION=true/false when using LOGWEIGHTS as otherwise the weights are ignored. Alternatively, learn to use the new syntax for histograms with KDE/ACCUMULATE to have more control over what PLUMED is calculating
[runnervm1li68:04865] *** Process received signal ***
[runnervm1li68:04865] Signal: Aborted (6)
[runnervm1li68:04865] Signal code:  (-6)
[runnervm1li68:04865] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f9f11445330]
[runnervm1li68:04865] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f9f1149eb2c]
[runnervm1li68:04865] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f9f1144527e]
[runnervm1li68:04865] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f9f114288ff]
[runnervm1li68:04865] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f9f118a5ff5]
[runnervm1li68:04865] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f9f118bb0da]
[runnervm1li68:04865] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f9f118a5a55]
[runnervm1li68:04865] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f9f118a5a6f]
[runnervm1li68:04865] [ 8] plumed_master(+0x146dd)[0x56050a2b26dd]
[runnervm1li68:04865] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f9f1142a1ca]
[runnervm1li68:04865] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f9f1142a28b]
[runnervm1li68:04865] [11] plumed_master(+0x15365)[0x56050a2b3365]
[runnervm1li68:04865] *** End of error message ***
</pre>
{% endraw %}
