**Project ID:** [plumID:20.033]({{ '/' | absolute_url }}eggs/20/033/)  
Stderr for source:  PRODUCTION/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action WHOLEMOLECULES with label @5 : cannot understand the following words from the input line : REF0, REF1, REF2
[runnervm1li68:09930] *** Process received signal ***
[runnervm1li68:09930] Signal: Aborted (6)
[runnervm1li68:09930] Signal code:  (-6)
[runnervm1li68:09930] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fa7bec45330]
[runnervm1li68:09930] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fa7bec9eb2c]
[runnervm1li68:09930] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fa7bec4527e]
[runnervm1li68:09930] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fa7bec288ff]
[runnervm1li68:09930] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fa7bf0a5ff5]
[runnervm1li68:09930] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fa7bf0bb0da]
[runnervm1li68:09930] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fa7bf0a5a55]
[runnervm1li68:09930] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fa7bf0a5a6f]
[runnervm1li68:09930] [ 8] plumed_master(+0x146dd)[0x55b39e6696dd]
[runnervm1li68:09930] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fa7bec2a1ca]
[runnervm1li68:09930] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fa7bec2a28b]
[runnervm1li68:09930] [11] plumed_master(+0x15365)[0x55b39e66a365]
[runnervm1li68:09930] *** End of error message ***
</pre>
{% endraw %}
