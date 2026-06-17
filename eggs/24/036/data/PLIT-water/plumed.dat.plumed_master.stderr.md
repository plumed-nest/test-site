**Project ID:** [plumID:24.036]({{ '/' | absolute_url }}eggs/24/036/)  
Stderr for source:  PLIT-water/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @36 : keyword ARG is compulsory for this action
[runnervm1li68:05112] *** Process received signal ***
[runnervm1li68:05112] Signal: Aborted (6)
[runnervm1li68:05112] Signal code:  (-6)
[runnervm1li68:05112] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f7a93e45330]
[runnervm1li68:05112] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f7a93e9eb2c]
[runnervm1li68:05112] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f7a93e4527e]
[runnervm1li68:05112] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f7a93e288ff]
[runnervm1li68:05112] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f7a942a5ff5]
[runnervm1li68:05112] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f7a942bb0da]
[runnervm1li68:05112] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f7a942a5a55]
[runnervm1li68:05112] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f7a942a5a6f]
[runnervm1li68:05112] [ 8] plumed_master(+0x146dd)[0x55971bad86dd]
[runnervm1li68:05112] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f7a93e2a1ca]
[runnervm1li68:05112] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f7a93e2a28b]
[runnervm1li68:05112] [11] plumed_master(+0x15365)[0x55971bad9365]
[runnervm1li68:05112] *** End of error message ***
</pre>
{% endraw %}
