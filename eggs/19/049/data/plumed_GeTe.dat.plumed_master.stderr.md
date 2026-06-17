**Project ID:** [plumID:19.049]({{ '/' | absolute_url }}eggs/19/049/)  
Stderr for source:  plumed_GeTe.dat   
Download: [zipped raw stdout](plumed_GeTe.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_GeTe.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action CONTACT_MATRIX_PROPER with label cc_cmat : it was not possible to interpret atom name flq6
[runnervm1li68:11421] *** Process received signal ***
[runnervm1li68:11421] Signal: Aborted (6)
[runnervm1li68:11421] Signal code:  (-6)
[runnervm1li68:11421] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f3974645330]
[runnervm1li68:11421] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f397469eb2c]
[runnervm1li68:11421] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f397464527e]
[runnervm1li68:11421] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f39746288ff]
[runnervm1li68:11421] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f3974aa5ff5]
[runnervm1li68:11421] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f3974abb0da]
[runnervm1li68:11421] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f3974aa5a55]
[runnervm1li68:11421] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f3974aa5a6f]
[runnervm1li68:11421] [ 8] plumed_master(+0x146dd)[0x558f5aac86dd]
[runnervm1li68:11421] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f397462a1ca]
[runnervm1li68:11421] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f397462a28b]
[runnervm1li68:11421] [11] plumed_master(+0x15365)[0x558f5aac9365]
[runnervm1li68:11421] *** End of error message ***
</pre>
{% endraw %}
