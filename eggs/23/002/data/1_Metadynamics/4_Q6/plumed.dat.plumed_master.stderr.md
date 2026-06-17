**Project ID:** [plumID:23.002]({{ '/' | absolute_url }}eggs/23/002/)  
Stderr for source:  1_Metadynamics/4_Q6/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action LOCAL_AVERAGE with label @s29 : cannot understand the following words from the input line : LOWMEM
[runnervm1li68:07793] *** Process received signal ***
[runnervm1li68:07793] Signal: Aborted (6)
[runnervm1li68:07793] Signal code:  (-6)
[runnervm1li68:07793] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f1f09645330]
[runnervm1li68:07793] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f1f0969eb2c]
[runnervm1li68:07793] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f1f0964527e]
[runnervm1li68:07793] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f1f096288ff]
[runnervm1li68:07793] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f1f09aa5ff5]
[runnervm1li68:07793] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f1f09abb0da]
[runnervm1li68:07793] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f1f09aa5a55]
[runnervm1li68:07793] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f1f09aa5a6f]
[runnervm1li68:07793] [ 8] plumed_master(+0x146dd)[0x561b436446dd]
[runnervm1li68:07793] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f1f0962a1ca]
[runnervm1li68:07793] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f1f0962a28b]
[runnervm1li68:07793] [11] plumed_master(+0x15365)[0x561b43645365]
[runnervm1li68:07793] *** End of error message ***
</pre>
{% endraw %}
