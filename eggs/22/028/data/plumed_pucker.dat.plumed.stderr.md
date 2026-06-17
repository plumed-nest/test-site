**Project ID:** [plumID:22.028]({{ '/' | absolute_url }}eggs/22/028/)  
Stderr for source:  plumed_pucker.dat   
Download: [zipped raw stdout](plumed_pucker.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_pucker.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action READ with label puck1 : could not find file named COLVAR_theta.0
[runnervm1li68:08147] *** Process received signal ***
[runnervm1li68:08147] Signal: Aborted (6)
[runnervm1li68:08147] Signal code:  (-6)
[runnervm1li68:08147] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f6921645330]
[runnervm1li68:08147] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f692169eb2c]
[runnervm1li68:08147] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f692164527e]
[runnervm1li68:08147] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f69216288ff]
[runnervm1li68:08147] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f6921aa5ff5]
[runnervm1li68:08147] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f6921abb0da]
[runnervm1li68:08147] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f6921aa5a55]
[runnervm1li68:08147] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f6921aa5a6f]
[runnervm1li68:08147] [ 8] plumed(+0x146dd)[0x55d9c3f5b6dd]
[runnervm1li68:08147] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f692162a1ca]
[runnervm1li68:08147] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f692162a28b]
[runnervm1li68:08147] [11] plumed(+0x15365)[0x55d9c3f5c365]
[runnervm1li68:08147] *** End of error message ***
</pre>
{% endraw %}
