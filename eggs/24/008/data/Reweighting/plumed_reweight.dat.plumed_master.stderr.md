**Project ID:** [plumID:24.008]({{ '/' | absolute_url }}eggs/24/008/)  
Stderr for source:  Reweighting/plumed_reweight.dat   
Download: [zipped raw stdout](plumed_reweight.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_reweight.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action READ with label rho : could not find file named rtp_coord.dat
[runnervm1li68:06018] *** Process received signal ***
[runnervm1li68:06018] Signal: Aborted (6)
[runnervm1li68:06018] Signal code:  (-6)
[runnervm1li68:06018] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f55f5845330]
[runnervm1li68:06018] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f55f589eb2c]
[runnervm1li68:06018] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f55f584527e]
[runnervm1li68:06018] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f55f58288ff]
[runnervm1li68:06018] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f55f5ca5ff5]
[runnervm1li68:06018] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f55f5cbb0da]
[runnervm1li68:06018] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f55f5ca5a55]
[runnervm1li68:06018] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f55f5ca5a6f]
[runnervm1li68:06018] [ 8] plumed_master(+0x146dd)[0x55da57e526dd]
[runnervm1li68:06018] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f55f582a1ca]
[runnervm1li68:06018] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f55f582a28b]
[runnervm1li68:06018] [11] plumed_master(+0x15365)[0x55da57e53365]
[runnervm1li68:06018] *** End of error message ***
</pre>
{% endraw %}
