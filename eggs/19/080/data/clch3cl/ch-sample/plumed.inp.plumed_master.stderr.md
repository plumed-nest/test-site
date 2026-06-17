**Project ID:** [plumID:19.080]({{ '/' | absolute_url }}eggs/19/080/)  
Stderr for source:  clch3cl/ch-sample/plumed.inp   
Download: [zipped raw stdout](plumed.inp.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @25 : keyword ARG is compulsory for this action
[runnervm1li68:09730] *** Process received signal ***
[runnervm1li68:09730] Signal: Aborted (6)
[runnervm1li68:09730] Signal code:  (-6)
[runnervm1li68:09730] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fe478045330]
[runnervm1li68:09730] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fe47809eb2c]
[runnervm1li68:09730] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fe47804527e]
[runnervm1li68:09730] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fe4780288ff]
[runnervm1li68:09730] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fe4784a5ff5]
[runnervm1li68:09730] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fe4784bb0da]
[runnervm1li68:09730] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fe4784a5a55]
[runnervm1li68:09730] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fe4784a5a6f]
[runnervm1li68:09730] [ 8] plumed_master(+0x146dd)[0x557cb15366dd]
[runnervm1li68:09730] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fe47802a1ca]
[runnervm1li68:09730] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fe47802a28b]
[runnervm1li68:09730] [11] plumed_master(+0x15365)[0x557cb1537365]
[runnervm1li68:09730] *** End of error message ***
</pre>
{% endraw %}
