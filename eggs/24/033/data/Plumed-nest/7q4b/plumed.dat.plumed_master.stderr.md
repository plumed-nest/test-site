**Project ID:** [plumID:24.033]({{ '/' | absolute_url }}eggs/24/033/)  
Stderr for source:  Plumed-nest/7q4b/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action EMMI with label gmm : REWEIGHT can only be used in parallel with 2 or more replicas
[runnervm1li68:05214] *** Process received signal ***
[runnervm1li68:05214] Signal: Aborted (6)
[runnervm1li68:05214] Signal code:  (-6)
[runnervm1li68:05214] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f3680a45330]
[runnervm1li68:05214] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f3680a9eb2c]
[runnervm1li68:05214] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f3680a4527e]
[runnervm1li68:05214] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f3680a288ff]
[runnervm1li68:05214] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f3680ea5ff5]
[runnervm1li68:05214] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f3680ebb0da]
[runnervm1li68:05214] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f3680ea5a55]
[runnervm1li68:05214] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f3680ea5a6f]
[runnervm1li68:05214] [ 8] plumed_master(+0x146dd)[0x55bc8354f6dd]
[runnervm1li68:05214] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f3680a2a1ca]
[runnervm1li68:05214] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f3680a2a28b]
[runnervm1li68:05214] [11] plumed_master(+0x15365)[0x55bc83550365]
[runnervm1li68:05214] *** End of error message ***
</pre>
{% endraw %}
