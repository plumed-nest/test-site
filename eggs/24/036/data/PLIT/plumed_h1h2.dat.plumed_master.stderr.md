**Project ID:** [plumID:24.036]({{ '/' | absolute_url }}eggs/24/036/)  
Stderr for source:  PLIT/plumed_h1h2.dat   
Download: [zipped raw stdout](plumed_h1h2.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_h1h2.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @38 : keyword ARG is compulsory for this action
[runnervm1li68:05009] *** Process received signal ***
[runnervm1li68:05009] Signal: Aborted (6)
[runnervm1li68:05009] Signal code:  (-6)
[runnervm1li68:05009] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f2c57045330]
[runnervm1li68:05009] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f2c5709eb2c]
[runnervm1li68:05009] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f2c5704527e]
[runnervm1li68:05009] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f2c570288ff]
[runnervm1li68:05009] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f2c574a5ff5]
[runnervm1li68:05009] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f2c574bb0da]
[runnervm1li68:05009] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f2c574a5a55]
[runnervm1li68:05009] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f2c574a5a6f]
[runnervm1li68:05009] [ 8] plumed_master(+0x146dd)[0x5600a69016dd]
[runnervm1li68:05009] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f2c5702a1ca]
[runnervm1li68:05009] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f2c5702a28b]
[runnervm1li68:05009] [11] plumed_master(+0x15365)[0x5600a6902365]
[runnervm1li68:05009] *** End of error message ***
</pre>
{% endraw %}
