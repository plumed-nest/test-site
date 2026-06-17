**Project ID:** [plumID:20.033]({{ '/' | absolute_url }}eggs/20/033/)  
Stderr for source:  PRODUCTION/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action WHOLEMOLECULES with label @5 : cannot understand the following words from the input line : REF0=16.995,21.964,24.520, REF1=26.253,18.440,24.5030, REF2=24.616,28.069,24.203
[runnervm1li68:09914] *** Process received signal ***
[runnervm1li68:09914] Signal: Aborted (6)
[runnervm1li68:09914] Signal code:  (-6)
[runnervm1li68:09914] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7ffaee045330]
[runnervm1li68:09914] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7ffaee09eb2c]
[runnervm1li68:09914] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7ffaee04527e]
[runnervm1li68:09914] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7ffaee0288ff]
[runnervm1li68:09914] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7ffaee4a5ff5]
[runnervm1li68:09914] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7ffaee4bb0da]
[runnervm1li68:09914] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7ffaee4a5a55]
[runnervm1li68:09914] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7ffaee4a5a6f]
[runnervm1li68:09914] [ 8] plumed(+0x146dd)[0x563b0a9d26dd]
[runnervm1li68:09914] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7ffaee02a1ca]
[runnervm1li68:09914] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7ffaee02a28b]
[runnervm1li68:09914] [11] plumed(+0x15365)[0x563b0a9d3365]
[runnervm1li68:09914] *** End of error message ***
</pre>
{% endraw %}
