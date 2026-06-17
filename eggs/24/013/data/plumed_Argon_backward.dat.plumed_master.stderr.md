**Project ID:** [plumID:24.013]({{ '/' | absolute_url }}eggs/24/013/)  
Stderr for source:  plumed_Argon_backward.dat   
Download: [zipped raw stdout](plumed_Argon_backward.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_Argon_backward.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action COORDINATIONNUMBER with label @s11 : keyword MORE_THAN could not be read correctly
[runnervm1li68:05796] *** Process received signal ***
[runnervm1li68:05796] Signal: Aborted (6)
[runnervm1li68:05796] Signal code:  (-6)
[runnervm1li68:05796] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7efe0fa45330]
[runnervm1li68:05796] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7efe0fa9eb2c]
[runnervm1li68:05796] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7efe0fa4527e]
[runnervm1li68:05796] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7efe0fa288ff]
[runnervm1li68:05796] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7efe0fea5ff5]
[runnervm1li68:05796] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7efe0febb0da]
[runnervm1li68:05796] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7efe0fea5a55]
[runnervm1li68:05796] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7efe0fea5a6f]
[runnervm1li68:05796] [ 8] plumed_master(+0x146dd)[0x55b2bc8f16dd]
[runnervm1li68:05796] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7efe0fa2a1ca]
[runnervm1li68:05796] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7efe0fa2a28b]
[runnervm1li68:05796] [11] plumed_master(+0x15365)[0x55b2bc8f2365]
[runnervm1li68:05796] *** End of error message ***
</pre>
{% endraw %}
