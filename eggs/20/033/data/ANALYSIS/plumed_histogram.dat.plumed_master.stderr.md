**Project ID:** [plumID:20.033]({{ '/' | absolute_url }}eggs/20/033/)  
Stderr for source:  ANALYSIS/plumed_histogram.dat   
Download: [zipped raw stdout](plumed_histogram.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_histogram.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @20 : keyword ARG is compulsory for this action
[runnervm1li68:09879] *** Process received signal ***
[runnervm1li68:09879] Signal: Aborted (6)
[runnervm1li68:09879] Signal code:  (-6)
[runnervm1li68:09879] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f4ced645330]
[runnervm1li68:09879] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f4ced69eb2c]
[runnervm1li68:09879] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f4ced64527e]
[runnervm1li68:09879] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f4ced6288ff]
[runnervm1li68:09879] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f4cedaa5ff5]
[runnervm1li68:09879] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f4cedabb0da]
[runnervm1li68:09879] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f4cedaa5a55]
[runnervm1li68:09879] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f4cedaa5a6f]
[runnervm1li68:09879] [ 8] plumed_master(+0x146dd)[0x5587867066dd]
[runnervm1li68:09879] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f4ced62a1ca]
[runnervm1li68:09879] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f4ced62a28b]
[runnervm1li68:09879] [11] plumed_master(+0x15365)[0x558786707365]
[runnervm1li68:09879] *** End of error message ***
</pre>
{% endraw %}
