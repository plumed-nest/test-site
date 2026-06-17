**Project ID:** [plumID:25.023]({{ '/' | absolute_url }}eggs/25/023/)  
Stderr for source:  update_2026/analysis/rewighting_2d_map_rmsd_cshape/tetramer/plumed_rew.dat   
Download: [zipped raw stdout](plumed_rew.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_rew.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action HISTOGRAM with label @s27 : set NORMALIZATION=true/false when using LOGWEIGHTS as otherwise the weights are ignored. Alternatively, learn to use the new syntax for histograms with KDE/ACCUMULATE to have more control over what PLUMED is calculating
[runnervm1li68:04814] *** Process received signal ***
[runnervm1li68:04814] Signal: Aborted (6)
[runnervm1li68:04814] Signal code:  (-6)
[runnervm1li68:04814] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f99cb045330]
[runnervm1li68:04814] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f99cb09eb2c]
[runnervm1li68:04814] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f99cb04527e]
[runnervm1li68:04814] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f99cb0288ff]
[runnervm1li68:04814] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f99cb4a5ff5]
[runnervm1li68:04814] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f99cb4bb0da]
[runnervm1li68:04814] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f99cb4a5a55]
[runnervm1li68:04814] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f99cb4a5a6f]
[runnervm1li68:04814] [ 8] plumed_master(+0x146dd)[0x560b1020e6dd]
[runnervm1li68:04814] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f99cb02a1ca]
[runnervm1li68:04814] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f99cb02a28b]
[runnervm1li68:04814] [11] plumed_master(+0x15365)[0x560b1020f365]
[runnervm1li68:04814] *** End of error message ***
</pre>
{% endraw %}
