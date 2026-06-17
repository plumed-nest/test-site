**Project ID:** [plumID:24.036]({{ '/' | absolute_url }}eggs/24/036/)  
Stderr for source:  DIDE-water/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @36 : keyword ARG is compulsory for this action
[runnervm1li68:04930] *** Process received signal ***
[runnervm1li68:04930] Signal: Aborted (6)
[runnervm1li68:04930] Signal code:  (-6)
[runnervm1li68:04930] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f6a0be45330]
[runnervm1li68:04930] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f6a0be9eb2c]
[runnervm1li68:04930] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f6a0be4527e]
[runnervm1li68:04930] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f6a0be288ff]
[runnervm1li68:04930] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f6a0c2a5ff5]
[runnervm1li68:04930] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f6a0c2bb0da]
[runnervm1li68:04930] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f6a0c2a5a55]
[runnervm1li68:04930] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f6a0c2a5a6f]
[runnervm1li68:04930] [ 8] plumed_master(+0x146dd)[0x55c88da816dd]
[runnervm1li68:04930] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f6a0be2a1ca]
[runnervm1li68:04930] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f6a0be2a28b]
[runnervm1li68:04930] [11] plumed_master(+0x15365)[0x55c88da82365]
[runnervm1li68:04930] *** End of error message ***
</pre>
{% endraw %}
