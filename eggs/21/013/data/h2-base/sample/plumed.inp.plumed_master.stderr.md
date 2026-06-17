**Project ID:** [plumID:21.013]({{ '/' | absolute_url }}eggs/21/013/)  
Stderr for source:  h2-base/sample/plumed.inp   
Download: [zipped raw stdout](plumed.inp.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @18 : keyword ARG is compulsory for this action
[runnervm1li68:08847] *** Process received signal ***
[runnervm1li68:08847] Signal: Aborted (6)
[runnervm1li68:08847] Signal code:  (-6)
[runnervm1li68:08847] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f7f5e245330]
[runnervm1li68:08847] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f7f5e29eb2c]
[runnervm1li68:08847] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f7f5e24527e]
[runnervm1li68:08847] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f7f5e2288ff]
[runnervm1li68:08847] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f7f5e6a5ff5]
[runnervm1li68:08847] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f7f5e6bb0da]
[runnervm1li68:08847] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f7f5e6a5a55]
[runnervm1li68:08847] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f7f5e6a5a6f]
[runnervm1li68:08847] [ 8] plumed_master(+0x146dd)[0x55960591a6dd]
[runnervm1li68:08847] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f7f5e22a1ca]
[runnervm1li68:08847] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f7f5e22a28b]
[runnervm1li68:08847] [11] plumed_master(+0x15365)[0x55960591b365]
[runnervm1li68:08847] *** End of error message ***
</pre>
{% endraw %}
