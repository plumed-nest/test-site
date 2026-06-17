**Project ID:** [plumID:24.013]({{ '/' | absolute_url }}eggs/24/013/)  
Stderr for source:  plumed_Argon_backward.dat   
Download: [zipped raw stdout](plumed_Argon_backward.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_Argon_backward.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action COORDINATIONNUMBER with label @s11 : keyword MORE_THAN could not be read correctly
[runnervm1li68:05781] *** Process received signal ***
[runnervm1li68:05781] Signal: Aborted (6)
[runnervm1li68:05781] Signal code:  (-6)
[runnervm1li68:05781] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f262e045330]
[runnervm1li68:05781] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f262e09eb2c]
[runnervm1li68:05781] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f262e04527e]
[runnervm1li68:05781] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f262e0288ff]
[runnervm1li68:05781] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f262e4a5ff5]
[runnervm1li68:05781] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f262e4bb0da]
[runnervm1li68:05781] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f262e4a5a55]
[runnervm1li68:05781] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f262e4a5a6f]
[runnervm1li68:05781] [ 8] plumed(+0x146dd)[0x56388b14d6dd]
[runnervm1li68:05781] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f262e02a1ca]
[runnervm1li68:05781] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f262e02a28b]
[runnervm1li68:05781] [11] plumed(+0x15365)[0x56388b14e365]
[runnervm1li68:05781] *** End of error message ***
</pre>
{% endraw %}
