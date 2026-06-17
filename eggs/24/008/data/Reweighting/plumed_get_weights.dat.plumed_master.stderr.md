**Project ID:** [plumID:24.008]({{ '/' | absolute_url }}eggs/24/008/)  
Stderr for source:  Reweighting/plumed_get_weights.dat   
Download: [zipped raw stdout](plumed_get_weights.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_get_weights.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action READ with label rho : could not find file named rtp_coord.dat
[runnervm1li68:05966] *** Process received signal ***
[runnervm1li68:05966] Signal: Aborted (6)
[runnervm1li68:05966] Signal code:  (-6)
[runnervm1li68:05966] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f4298c45330]
[runnervm1li68:05966] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f4298c9eb2c]
[runnervm1li68:05966] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f4298c4527e]
[runnervm1li68:05966] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f4298c288ff]
[runnervm1li68:05966] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f42990a5ff5]
[runnervm1li68:05966] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f42990bb0da]
[runnervm1li68:05966] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f42990a5a55]
[runnervm1li68:05966] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f42990a5a6f]
[runnervm1li68:05966] [ 8] plumed_master(+0x146dd)[0x562047d066dd]
[runnervm1li68:05966] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f4298c2a1ca]
[runnervm1li68:05966] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f4298c2a28b]
[runnervm1li68:05966] [11] plumed_master(+0x15365)[0x562047d07365]
[runnervm1li68:05966] *** End of error message ***
</pre>
{% endraw %}
