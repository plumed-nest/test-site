**Project ID:** [plumID:19.080]({{ '/' | absolute_url }}eggs/19/080/)  
Stderr for source:  clch3cl/ccl-sample/plumed.inp   
Download: [zipped raw stdout](plumed.inp.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @22 : keyword ARG is compulsory for this action
[runnervm1li68:09666] *** Process received signal ***
[runnervm1li68:09666] Signal: Aborted (6)
[runnervm1li68:09666] Signal code:  (-6)
[runnervm1li68:09666] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f76f9445330]
[runnervm1li68:09666] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f76f949eb2c]
[runnervm1li68:09666] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f76f944527e]
[runnervm1li68:09666] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f76f94288ff]
[runnervm1li68:09666] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f76f98a5ff5]
[runnervm1li68:09666] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f76f98bb0da]
[runnervm1li68:09666] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f76f98a5a55]
[runnervm1li68:09666] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f76f98a5a6f]
[runnervm1li68:09666] [ 8] plumed_master(+0x146dd)[0x55a4ed9916dd]
[runnervm1li68:09666] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f76f942a1ca]
[runnervm1li68:09666] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f76f942a28b]
[runnervm1li68:09666] [11] plumed_master(+0x15365)[0x55a4ed992365]
[runnervm1li68:09666] *** End of error message ***
</pre>
{% endraw %}
