**Project ID:** [plumID:19.049]({{ '/' | absolute_url }}eggs/19/049/)  
Stderr for source:  plumed_urea.dat   
Download: [zipped raw stdout](plumed_urea.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_urea.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action CONTACT_MATRIX with label @s41 : missing SWITCH11 keyword
[runnervm1li68:11495] *** Process received signal ***
[runnervm1li68:11495] Signal: Aborted (6)
[runnervm1li68:11495] Signal code:  (-6)
[runnervm1li68:11495] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f4aec245330]
[runnervm1li68:11495] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f4aec29eb2c]
[runnervm1li68:11495] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f4aec24527e]
[runnervm1li68:11495] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f4aec2288ff]
[runnervm1li68:11495] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f4aec6a5ff5]
[runnervm1li68:11495] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f4aec6bb0da]
[runnervm1li68:11495] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f4aec6a5a55]
[runnervm1li68:11495] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f4aec6a5a6f]
[runnervm1li68:11495] [ 8] plumed(+0x146dd)[0x559e3d1a06dd]
[runnervm1li68:11495] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f4aec22a1ca]
[runnervm1li68:11495] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f4aec22a28b]
[runnervm1li68:11495] [11] plumed(+0x15365)[0x559e3d1a1365]
[runnervm1li68:11495] *** End of error message ***
</pre>
{% endraw %}
