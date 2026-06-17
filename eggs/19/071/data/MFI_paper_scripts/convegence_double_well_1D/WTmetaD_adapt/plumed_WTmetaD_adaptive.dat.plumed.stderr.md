**Project ID:** [plumID:19.071]({{ '/' | absolute_url }}eggs/19/071/)  
Stderr for source:  MFI_paper_scripts/convegence_double_well_1D/WTmetaD_adapt/plumed_WTmetaD_adaptive.dat   
Download: [zipped raw stdout](plumed_WTmetaD_adaptive.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_WTmetaD_adaptive.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action METAD with label metad : When using ADAPTIVE Gaussians on a grid SIGMA_MIN must be specified
[runnervm1li68:11265] *** Process received signal ***
[runnervm1li68:11265] Signal: Aborted (6)
[runnervm1li68:11265] Signal code:  (-6)
[runnervm1li68:11265] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f033ee45330]
[runnervm1li68:11265] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f033ee9eb2c]
[runnervm1li68:11265] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f033ee4527e]
[runnervm1li68:11265] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f033ee288ff]
[runnervm1li68:11265] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f033f2a5ff5]
[runnervm1li68:11265] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f033f2bb0da]
[runnervm1li68:11265] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f033f2a5a55]
[runnervm1li68:11265] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f033f2a5a6f]
[runnervm1li68:11265] [ 8] plumed(+0x146dd)[0x555c6be286dd]
[runnervm1li68:11265] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f033ee2a1ca]
[runnervm1li68:11265] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f033ee2a28b]
[runnervm1li68:11265] [11] plumed(+0x15365)[0x555c6be29365]
[runnervm1li68:11265] *** End of error message ***
</pre>
{% endraw %}
