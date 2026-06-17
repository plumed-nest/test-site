**Project ID:** [plumID:19.080]({{ '/' | absolute_url }}eggs/19/080/)  
Stderr for source:  h3/explicit/plumed.inp   
Download: [zipped raw stdout](plumed.inp.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @36 : keyword ARG is compulsory for this action
[runnervm1li68:09819] *** Process received signal ***
[runnervm1li68:09819] Signal: Aborted (6)
[runnervm1li68:09819] Signal code:  (-6)
[runnervm1li68:09819] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fcd2ca45330]
[runnervm1li68:09819] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fcd2ca9eb2c]
[runnervm1li68:09819] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fcd2ca4527e]
[runnervm1li68:09819] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fcd2ca288ff]
[runnervm1li68:09819] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fcd2cea5ff5]
[runnervm1li68:09819] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fcd2cebb0da]
[runnervm1li68:09819] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fcd2cea5a55]
[runnervm1li68:09819] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fcd2cea5a6f]
[runnervm1li68:09819] [ 8] plumed_master(+0x146dd)[0x55c5db26b6dd]
[runnervm1li68:09819] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fcd2ca2a1ca]
[runnervm1li68:09819] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fcd2ca2a28b]
[runnervm1li68:09819] [11] plumed_master(+0x15365)[0x55c5db26c365]
[runnervm1li68:09819] *** End of error message ***
</pre>
{% endraw %}
