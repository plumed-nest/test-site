**Project ID:** [plumID:24.013]({{ '/' | absolute_url }}eggs/24/013/)  
Stderr for source:  plumed_Argon_forward.dat   
Download: [zipped raw stdout](plumed_Argon_forward.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_Argon_forward.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action COORDINATIONNUMBER with label @s11 : keyword MORE_THAN could not be read correctly
[runnervm1li68:05833] *** Process received signal ***
[runnervm1li68:05833] Signal: Aborted (6)
[runnervm1li68:05833] Signal code:  (-6)
[runnervm1li68:05833] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fe8f9445330]
[runnervm1li68:05833] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fe8f949eb2c]
[runnervm1li68:05833] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fe8f944527e]
[runnervm1li68:05833] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fe8f94288ff]
[runnervm1li68:05833] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fe8f98a5ff5]
[runnervm1li68:05833] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fe8f98bb0da]
[runnervm1li68:05833] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fe8f98a5a55]
[runnervm1li68:05833] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fe8f98a5a6f]
[runnervm1li68:05833] [ 8] plumed(+0x146dd)[0x558a2f6a86dd]
[runnervm1li68:05833] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fe8f942a1ca]
[runnervm1li68:05833] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fe8f942a28b]
[runnervm1li68:05833] [11] plumed(+0x15365)[0x558a2f6a9365]
[runnervm1li68:05833] *** End of error message ***
</pre>
{% endraw %}
