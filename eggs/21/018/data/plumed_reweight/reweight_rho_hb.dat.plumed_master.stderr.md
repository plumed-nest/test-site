**Project ID:** [plumID:21.018]({{ '/' | absolute_url }}eggs/21/018/)  
Stderr for source:  plumed_reweight/reweight_rho_hb.dat   
Download: [zipped raw stdout](reweight_rho_hb.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](reweight_rho_hb.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: IFile closed in the middle of reading. seems strange!
WARNING: IFile closed in the middle of reading. seems strange!
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action HISTOGRAM with label @s13 : set NORMALIZATION=true/false when using LOGWEIGHTS as otherwise the weights are ignored. Alternatively, learn to use the new syntax for histograms with KDE/ACCUMULATE to have more control over what PLUMED is calculating
[runnervm1li68:08924] *** Process received signal ***
[runnervm1li68:08924] Signal: Aborted (6)
[runnervm1li68:08924] Signal code:  (-6)
[runnervm1li68:08924] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f9bd9045330]
[runnervm1li68:08924] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f9bd909eb2c]
[runnervm1li68:08924] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f9bd904527e]
[runnervm1li68:08924] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f9bd90288ff]
[runnervm1li68:08924] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f9bd94a5ff5]
[runnervm1li68:08924] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f9bd94bb0da]
[runnervm1li68:08924] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f9bd94a5a55]
[runnervm1li68:08924] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f9bd94a5a6f]
[runnervm1li68:08924] [ 8] plumed_master(+0x146dd)[0x5596cee0b6dd]
[runnervm1li68:08924] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f9bd902a1ca]
[runnervm1li68:08924] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f9bd902a28b]
[runnervm1li68:08924] [11] plumed_master(+0x15365)[0x5596cee0c365]
[runnervm1li68:08924] *** End of error message ***
</pre>
{% endraw %}
