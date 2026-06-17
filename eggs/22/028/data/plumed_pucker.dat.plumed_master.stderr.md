**Project ID:** [plumID:22.028]({{ '/' | absolute_url }}eggs/22/028/)  
Stderr for source:  plumed_pucker.dat   
Download: [zipped raw stdout](plumed_pucker.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_pucker.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action READ with label puck1 : could not find file named COLVAR_theta.0
[runnervm1li68:08163] *** Process received signal ***
[runnervm1li68:08163] Signal: Aborted (6)
[runnervm1li68:08163] Signal code:  (-6)
[runnervm1li68:08163] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f56eac45330]
[runnervm1li68:08163] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f56eac9eb2c]
[runnervm1li68:08163] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f56eac4527e]
[runnervm1li68:08163] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f56eac288ff]
[runnervm1li68:08163] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f56eb0a5ff5]
[runnervm1li68:08163] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f56eb0bb0da]
[runnervm1li68:08163] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f56eb0a5a55]
[runnervm1li68:08163] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f56eb0a5a6f]
[runnervm1li68:08163] [ 8] plumed_master(+0x146dd)[0x55af6766b6dd]
[runnervm1li68:08163] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f56eac2a1ca]
[runnervm1li68:08163] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f56eac2a28b]
[runnervm1li68:08163] [11] plumed_master(+0x15365)[0x55af6766c365]
[runnervm1li68:08163] *** End of error message ***
</pre>
{% endraw %}
